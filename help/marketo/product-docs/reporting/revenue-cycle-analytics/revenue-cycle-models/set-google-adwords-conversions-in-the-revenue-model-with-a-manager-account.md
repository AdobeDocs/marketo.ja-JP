---
unique-page-id: 7504923
description: 管理者アカウントを持つ収益モデルの Set [!DNL Google AdWords] Conversions - Marketo ドキュメント – 製品ドキュメント
title: Set [!DNL Google AdWords] Conversions in the Revenue Model with a Manager Account
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 30%

---

# マネージャ [!DNL Google AdWords] アカウントを持つ収益モデルでのコンバージョンの設定 {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

[!DNL Google AdWords] アカウントを Marketo にリンクして、オフラインのコンバージョンデータを Marketo から [!DNL Google AdWords] に自動的にアップロードします。その後、[!DNL AdWords] UI から、[ で ](https://support.google.com/adwords/answer/3073556) カスタム列を追加 [!DNL AdWords] した後、どのクリックが適格なリード、商談、新規顧客（または追跡したい収益ステージ）につながったかを簡単に確認できます。

複数の [!DNL Google Adwords] アカウントがある場合は、[[!DNL Google AdWords] Manager アカウント ](https://www.google.com/adwords/manager-accounts/) （旧称：My Client Center）を使用して、それらをMarketoと統合できます。

[!DNL AdWords] のオフラインコンバージョンを収益モデルの 1 つ以上のステージにマッピングできます。 次の 2 つの方法があります。

* ステージアクション
* [!DNL AdWords] マッピング

>[!PREREQUISITES]
>
>[ マネージャ  [!DNL Google AdWords]  アカウントを持つ Launchpoint Service として追加 ](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## ステージアクションを使用する {#use-stage-action}

「ステージアクション」の下で [!DNL AdWords] コンバージョンをマッピングします。

1. [!DNL AdWords] 変換にマッピングするステップを選択します。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. **[!UICONTROL ステージアクション]**&#x200B;ドロップダウンで、「**[!UICONTROL AdWords コンバージョンを設定]**」を選択します。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. **[!DNL AdWords]変換を設定**.

   >[!NOTE]
   >
   >子アカウントごとに異なる [!DNL AdWords] コンバージョンを選択できます。

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   ヒント：[!DNL AdWords] しいコンバージョンがない場合は、「**[!UICONTROL +新規コンバージョン]**」をクリックして作成します。

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-3-27-17-3a21-3a15.png)

1. すべての [!DNL AdWords] コンバージョンの売上高ステージへのマッピングが完了したら、概要ページに戻ります。 「**[!UICONTROL モデルアクション]**」を選択し、「**[!UICONTROL ステージの承認]**」を選択します。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## 上級ヒント：新しいコンバージョンを追加する {#pro-tip-add-a-new-conversion}

上級向けのヒントです。新しい [!DNL AdWords] オフラインコンバージョンをMarketoから作成できます。

>[!CAUTION]
>
>Marketo から作成された新しいコンバージョンでは、「最適化」設定が有効になっています。つまり、入札戦略 [!DNL AdWords] よって、これらのコンバージョンに対する入札を最適化できます。 この設定は [!DNL AdWords] アカウントから変更できます。

1. **[!UICONTROL ステージアクション]**&#x200B;ドロップダウンで、「**[!UICONTROL AdWords コンバージョンを設定]**」を選択します。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 「**[!UICONTROL 新しいコンバージョン]**」を選択します。

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. **コンバージョン名**&#x200B;を入力します。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   これで完了です。この新しいコンバージョンは、[!DNL AdWords] アカウントに表示されます。

## [!DNL AdWords] マッピングの使用 {#use-adwords-mapping}

[!DNL AdWords] マッピングを使用すると、すべてのモデルステージを [!DNL AdWords] コンバージョンに 1 か所で関連付けることができます。

1. 「**[!UICONTROL AdWords マッピングの編集]**」を選択します。

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. 追跡するステージごとに **[!DNL AdWords]目的の** アカウントと目的の **[!DNL AdWords]コンバージョン** を選択します。

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. ステージをマッピングしたら、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. すべての [!DNL AdWords] コンバージョンの売上高ステージへのマッピングが完了したら、概要ページに戻ります。 「**[!UICONTROL モデルアクション]**」を選択し、「**[!UICONTROL ステージの承認]**」を選択します。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

オフラインコンバージョンデータを表示するには、[!DNL AdWords] アカウントにログインする必要があります。 [カスタム列機能](https://support.google.com/adwords/answer/3073556)を使用して、Marketo にインポートするオフラインコンバージョンごとにコンバージョン数の列を作成することをお勧めします。
