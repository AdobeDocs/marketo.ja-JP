---
unique-page-id: 9437903
description: カスタム同期フィルタ  [!DNL Dynamics]  の作成 – Marketo ドキュメント – 製品ドキュメント
title: カスタム同期フィルタ  [!DNL Dynamics]  の作成
exl-id: 6b0d878a-9c55-4e73-9923-11140e83bb37
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 73%

---

# カスタム [!DNL Dynamics] 同期フィルターの作成 {#create-a-custom-dynamics-sync-filter}

Dynamics CRM 内のすべてをMarketo Engageに同期したくない場合は、 心配無用です。Marketo では、同期フィルターを設定して、レコードの一部のみを同期できます。

## 概要 {#overview}

[!DNL Dynamics] 同期フィルターを設定するには：

1. 任意のオブジェクト（リード、連絡先、アカウント、商談、その他のカスタムエンティティ）に対して、Dynamics CRM で new_synctomkto という名前のカスタム 2 つのオプション（ブール値）フィールドを作成します。
1. このフィールドに Yes/No 値を割り当てます。

これらの変更は、データベースや Marketo ではなく、Dynamics CRM でおこなう必要があります。

>[!CAUTION]
>
>フィールドを割り当てず、空白または NULL のままにすると、同期は行われますが、更新は行われません。 Dynamics CRM のフィールド値が空白または NULL のレコードでは、Marketoのこのフィールド値が「false」と表示されます。

Marketo は、自動バックグラウンド同期中にこのフィールドを探し、このロジックに基づいて同期するレコードを判定します。

| フィールド値 | Marketo に同期？ |
|---|---|
| フィールドが存在しない | はい |
| フィールドが空 | はい |
| フィールド値が Yes | はい |
| フィールド値が No | いいえ |

>[!CAUTION]
>
>レコードをスキップするように Marketo に伝える唯一の方法は、フィールドの値を明示的に **No** に設定することです。Marketo は、フィールドの値が空でもレコードを同期します。

>[!PREREQUISITES]
>
>最新バージョンのMarketo プラグイン（3.0.0.1 以降）をインストールします。 Marketo/[!UICONTROL &#x200B; 管理者 &#x200B;]/[!DNL Microsoft Dynamics]/[!UICONTROL Marketo ソリューションをダウンロード &#x200B;] に移動します。

## SyncToMkto フィールドの作成 {#create-synctomkto-field}

1. Dynamics CRM にログインします。 **設定** をクリックしてから、**カスタマイズ** をクリックします。

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. 「**[!UICONTROL システムをカスタマイズ]**」をクリックします。

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. 「**[!UICONTROL エンティティ]**」の横にある ![](assets/image2015-8-10-21-3a44-3a23.png) をクリックします。

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. 「**[!UICONTROL リード]**」の横にある ![](assets/image2015-8-10-21-3a44-3a23.png) をクリックし、「**[!UICONTROL フィールド]**」を選択します。次に、「**[!UICONTROL 新規]**」をクリックします。

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. **表示名** フィールドに **[!UICONTROL SyncToMkto]** と入力し、**[!UICONTROL データタイプ]** として **[!UICONTROL 2 つのオプション]** を選択します。 次に、「**[!UICONTROL 保存して閉じる]**」をクリックします。

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >このフィールドの表示名を任意に選択しますが、「名前」フィールドは正確に **new_synctomkto** にする必要があります。デフォルトの接頭辞として **new** を使用する必要があります。デフォルトを変更した場合は、ここに移動して、[&#128279;](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md){target="_blank"}カスタムフィールド名のデフォルトの接頭辞をリセットします。新しいフィールドを作成した後で、このフィールドを元に戻すことができます。

   >[!NOTE]
   >
   >非同期ワークフローを設定している場合、レコードは、フィールドで設定したデフォルトの SyncToMkto 値を取得し、ワークフローの実行が終了した数秒後に正しい値を取得します。デフォルト値が「はい」に設定されている場合、これらのレコードは Marketo で作成されて古くなります。これを回避するには、**いいえ**&#x200B;をデフォルト値として使用します。

1. このプロセスを繰り返し、連絡先、アカウント、商談、カスタムエンティティなど、同期を制限する他のエンティティ用に **SyncToMkto** フィールドを作成します。

## Marketo でフィルターを選択する {#select-the-filter-in-marketo}

初期同期が既に完了している場合は、中に移動し、Marketo と同期するフィールドを選択します。

1. 「管理者」に移動し、「**[!UICONTROL Microsoft Dynamics]**」を選択します。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 「フィールド同期の詳細」で「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 下にスクロールしてフィールドを確認します。実際の名前は new_synctomkto にする必要がありますが、表示名は任意の名前にすることができます。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-10-9-9-3a56-3a23.png)

これで、Marketo の同期フィルターが有効になりました。

## 同期フィルター値を自動的に割り当てる [!DNL Dynamics] ワークフローの作成 {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

レコードの SyncToMkto フィールドには、いつでも手動で値を割り当てることができます。しかし、レコードの作成時や更新時に、[!DNL Dynamics] ワークフローの機能を活用して、SyncToMkto フィールドに値を自動割り当ててみませんか？

>[!NOTE]
>
>データベースレベルでは、この操作はできません。CRM では、これは手動でおこなうか、ワークフローを使用する必要があります。
>
>[!DNL Dynamics] ワークフローは、履歴データではなく、今後作成される新しいレコードに対してのみ機能します。 バッチアップデートを使用して、既存のレコードを移動します。

1. Dynamics CRM に移動します。 **設定**/**プロセス** をクリックします。

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. 「**[!UICONTROL 新規]**」をクリックします。

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. ワークフローの名前を入力し、**[!UICONTROL カテゴリ]** として [!UICONTROL &#x200B; ワークフロー &#x200B;] を選択し、**[!UICONTROL エンティティ]** として [!UICONTROL &#x200B; リード &#x200B;] を選択します。 次に、「**OK**」をクリックします。

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. 組織の好みに応じて、**SyncToMkto** フィールドに true または false の値を割り当てるルールを作成します。「**[!UICONTROL 保存して閉じる]**」をクリックします。

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >「**[!UICONTROL ステップの追加]**」をクリックしてチェック条件を追加した後に、デフォルトのアクションを定義します。同期しないレコードを&#x200B;**いいえ**&#x200B;と設定します。それ以外の場合は、同期されます。

1. ワークフローを選択し、「**[!UICONTROL アクティブ化]**」をクリックします。

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >メールアドレスを持つユーザーのレコードのみを同期するルールを設定するには、「[メールアドレスのカスタム同期フィルタールール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"}」を参照してください。

## 同期フィルターの詳細 {#sync-filter-details}

以下に、必要な実装の詳細を示します。

* 同期操作の開始

  **SyncToMkto** の値が **いいえ** から **はい** に変わると、[!DNL Dynamics] はMarketoにこのレコードの同期を開始するように直ちに通知します。 レコードが既に存在する場合は、Marketo によってアップデートされます。それ以外の場合は、レコードが作成されます。

  >[!TIP]
  >
  >これが発生すると、`Create [StartSync]`操作が Marketo ログに追加されます。

* 同期操作の停止

  レコードの SyncToMkto 値が Yes から No に変更されると、Marketo にこのレコードの同期を停止するよう通知されます。ただし、レコードは削除されず、アップデートの取得が停止され、古くなります。

>[!MORELIKETHIS]
>
>* [Microsoft Dynamics Sync フィルター：認定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md){target="_blank"}
>* [Microsoft Dynamics 同期フィルター：結合](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md){target="_blank"}
>* [メールアドレスのカスタム同期フィルタールール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"}
