---
unique-page-id: 9437903
description: カスタムダイナミクス同期フィルターの作成 — Marketto Docs — 製品ドキュメント
title: カスタムダイナミクス同期フィルタを作成する
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 0%

---


# カスタムダイナミクス同期フィルタを作成する {#create-a-custom-dynamics-sync-filter}

Dynamics CRMのすべてをMarketorに同期したくない場合 心配するな！ Marketingでは、同期フィルターを設定し、レコードの一部のみを同期できます。

## 概要 {#overview}

ダイナミクス同期フィルタを設定するには：

1. 任意のオブジェクト（リード、連絡先、アカウント、オポチュニティ、その他のカスタムエンティティ）に対して、Dynamics CRMにnew_synctomktoという名前のカスタム2つのオプション（ブール型）フィールドを作成します。
1. このフィールドにはい/いいえの値を割り当てるか、空白のままにします。

>[!NOTE]
>
>これらの変更は、データベースやマーケティング担当者ではなく、Dynamics CRMで行う必要があります。

Marketorは、バックグラウンドでの自動同期中にこのフィールドを探し、次のロジックに基づいて、どのレコードを同期するかを決定します。

| フィールド値 | Marketoと同期しますか？ |
|---|---|
| フィールドが存在しません | はい |
| フィールドが空です | はい |
| フィールドに値Yesがある | はい |
| フィールドに値Noがある | いいえ |

>[!CAUTION]
>
>レコードをスキップするようにマーケティングツールに指示する唯一の方法は、フィールドの値を明示的に **「いいえ**」に設定することです。 フィールドの値が空でも、引き続きMarketorはレコードを同期します。

>[!PREREQUISITES]
>
>Marketo Plug-inの最新バージョン（3.0.0.1以降）をインストールします。 Marketor/管理者/Microsoft Dynamics/Markettor Solutionのダウンロードに移動します。

## SyncToMktoフィールドを作成 {#create-synctomkto-field}

1. Dynamics CRMにログインします。 「 **設定** 」をクリックし、「 **カスタマイズ」をクリックします**。

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. 「システムの **カスタマイズ**」をクリックします。

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. 「 ![](assets/image2015-8-10-21-3a44-3a23.png) エンティティ ****」の横のをクリックします。

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. 「**Lead **」の ![](assets/image2015-8-10-21-3a44-3a23.png) 横にあるをクリックし、「 **Fields**」を選択します。 次に、「 **新規**」をクリックします。

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. 「 **表示名** 」フィールドにSyncToMkto **と入力し、「データタイプ** 」として **「2つのオプション******」を選択します。 次に、「 **保存して閉じる**」をクリックします。

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >このフィールドには任意の表示名を選択しますが、[名前]フィールドは **new_synctomktoにする必要があります**。 デフォルトのプレフィックスとして **new** （新しい）を使用する必要があります。 デフォルトを変更した場合は、ここに移動してカスタムフィールド名のデフォルトのプレフィックスを [リセットします](create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md)。 新しいフィールドを作成した後で、変更を元に戻すことができます。

   >[!NOTE]
   >
   >非同期ワークフローが設定されている場合、レコードにはフィールドで設定したデフォルトのSyncToMkto値が取得され、ワークフローの実行が終了する数秒後に正しい値が取得されます。 デフォルト値が「はい」に設定されている場合、これらのレコードはマーケティング担当者に作成され、古いレコードになります。 これを避けるに **は** 、デフォルト値として「いいえ」を使用します。

1. このプロセスを繰り返し、連絡先、アカウント、オポチュニティ、カスタムエンティティなど、同期を制限する他のエンティティに対して **SyncToMkto** フィールドを作成します。

## マーケティングでのフィルターの選択 {#select-the-filter-in-marketo}

初回同期が既に完了している場合でも、に進み、Marketoと同期するフィールドを選択します。

1. [管理]に移動し、[マイクロソフト **ダイナミクス**]を選択します。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 「フィールドの同期の詳細を **編集** 」をクリックします。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. フィールドまで下にスクロールし、チェックします。 実際の名前はnew_synctomktoにする必要がありますが、表示名は任意の名前にすることができます。 「 **保存**」をクリックします。

   ![](assets/image2015-10-9-9-3a56-3a23.png)

これで、Marketoの同期フィルターが有効になりました。

## 同期フィルタ値を自動的に割り当てるDynamicsワークフローを作成する {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

レコードのSyncToMktoフィールドには、常に手動で値を割り当てることができます。 ただし、Dynamics Workflowの機能を利用し、レコードの作成時または更新時にSyncToMktoフィールドに値を自動割り当てしないでください。

>[!NOTE]
>
>データベースレベルでは実行できません。 CRMで手動で実行するか、ワークフローを使用する必要があります。
>
>Dynamicsワークフローは、今後作成される新しいレコードに対してのみ機能し、履歴データには機能しません。 バッチ更新を使用して、既存のレコードの上に移動します。

1. Dynamics CRMに移動します。 「 **設定** 」をクリックし、「 **プロセス**」をクリックします。

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. 「 **新規**」をクリックします。

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. ワークフローの名前を入力し、カテゴリとして「 **Workflow** 」を選択し、「 **Lead** 」を「エンティティ」として選択します。 次に、「 **OK**」をクリックします。

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. 組織の好みに応じて「SyncToMkto **** 」フィールドにtrueまたはfalseの値を割り当てるルールを作成します。 「 **保存して閉じる**」をクリックします。

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >「 **追加手順** 」をクリックしてCheck Conditionを追加した後に、デフォルトアクションを定義します。 同期しないレコードを **[いいえ**]に設定します。 それ以外の場合は、同期が実行されます。

1. ワークフローを選択し、「 **アクティブ化**」をクリックします。

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >電子メールアドレスを持つユーザーのレコードのみを同期するルールを設定するには、 [「電子メールアドレスのカスタム同期フィルタールール](create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md) 」を参照してください。

## 同期フィルターの詳細 {#sync-filter-details}

以下に、お知らせする必要があると思われる実装の詳細を示します。

1. 同期操作の開始

   SyncToMkto **の値が** No **から** Yes ****&#x200B;に変更されると、Dynamicsは、このレコードを同期する開始に即座に通知します。 レコードが既に存在する場合は、マーケティング担当者がそのレコードを更新します。 それ以外の場合は、Marketorはレコードを作成します。

   >[!TIP]
   >
   >これが発生すると、 **Create [StartSync]** 操作がマーケティングログに追加されます。

1. 同期操作の停止

   レコードのSyncToMkto値がYesからNoに変更されると、マーケティング担当者にこのレコードの同期を停止するよう通知されます。 ただし、レコードは削除されず、代わりに更新の取得が停止され、古くなります。

>[!NOTE]
>
>**関連記事**
>
>* [Microsoft Dynamics同期フィルタ：条件を満たす](create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md)
>* [Microsoft Dynamics同期フィルタ：結合](create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md)
>* [電子メールアドレスのカスタム同期フィルター規則](create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md)

>



