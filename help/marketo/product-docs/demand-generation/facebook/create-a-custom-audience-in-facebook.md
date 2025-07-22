---
unique-page-id: 4720275
description: Facebook でのカスタムオーディエンスの作成- Marketo ドキュメント - 製品ドキュメント
title: Facebook でのカスタムオーディエンスの作成
exl-id: a2c8d89c-16b3-44f6-a2c6-c52fe78ab39c
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 61%

---

# [!DNL Facebook] でのカスタムオーディエンスの作成 {#create-a-custom-audience-in-facebook}

>[!PREREQUISITES]
>
>* [LaunchPoint サ  [!DNL Facebook]  ビスとしてのカスタムオーディエンスの追加 ](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md){target="_blank"} 「管理者」セクション
>* [ アカウント内の  [!DNL Facebook]](https://www.facebook.com/ads/manage/customaudiences/tos.php){target="_blank"} のカスタムオーディエンス条件に同意 [!DNL Facebook] ます。

>[!TIP]
>
>詳しくは、[ カスタムオーディエンス  [!DNL Facebook]](https://www.facebook.com/help/341425252616329){target="_blank"} を参照してください。

1. オーディエンスを作成するリードを含むスマートリストまたは静的リストを探して選択します。

   ![](assets/create-a-custom-audience-in-facebook-1.png)

1. 「**[!UICONTROL リード]**」タブを選択し、下部にある「**Ad Bridge を介して送信**」アイコンをクリックします。

   ![](assets/create-a-custom-audience-in-facebook-2.png)

1. 「**[!UICONTROL Facebook]**」を選択し、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/create-a-custom-audience-in-facebook-3.png)

1. 「**[!UICONTROL オーディエンス]**」ドロップダウンをクリックし、「**[!UICONTROL + 新規オーディエンス]**」を選択します。

   ![](assets/create-a-custom-audience-in-facebook-4.png)

   >[!IMPORTANT]
   >
   >Facebook API を使用すると、Facebook 広告アカウントあたり最大 500 個のカスタムオーディエンスを利用できます。

1. 「**[!UICONTROL オーディエンス名]**」を入力します。「**[!UICONTROL 更新]**」をクリックします。

   ![](assets/create-a-custom-audience-in-facebook-5.png)

   >[!NOTE]
   >
   >複数の [!DNL Facebook] 広告アカウントがある場合は、追加のドロップダウンが表示され、このオーディエンスを作成する広告アカウントを選択できます。

   >[!TIP]
   >
   >広告セットまたはグループと現在関連付けられている既存のオーディエンスを、新しいオーディエンスに入れ替える場合は、「**[!UICONTROL 既存のオーディエンスを置換]**」チェックボックスを選択します。これを行っても、置換されるオーディエンスは&#x200B;**削除されません**。

1. 完了すると、ステータスダイアログが更新されます。

   ![](assets/create-a-custom-audience-in-facebook-6.png)

   これで完了です。Facebook では、**広告マネージャ**／**オーディエンス**&#x200B;に新しいオーディエンスが表示されます。

   ![](assets/create-a-custom-audience-in-facebook-7.png)

   >[!NOTE]
   >
   >[!DNL Facebook] にプッシュするすべてのリストが静的になります。 Marketoのスマートリストは、転送後に加えられた変更を反映するために [!DNL Facebook] のオーディエンスリストを自動更新しません。

   >[!MORELIKETHIS]
   >
   >[ でのカスタムオーディエンスへのリードの追加  [!DNL Facebook]](/help/marketo/product-docs/demand-generation/facebook/add-leads-to-a-custom-audience-in-facebook.md)
