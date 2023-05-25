---
unique-page-id: 2360360
description: の作成 [!DNL Webhook] - Marketoドキュメント — 製品ドキュメント
title: の作成 [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
source-git-commit: 1f10e1fcdbd5cf91481f749236fd37050ade29f8
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 66%

---

# の作成 [!DNL Webhook] {#create-a-webhook}

用途 [!DNL Webhooks] サードパーティの web サービスを活用して、テキストメッセージを送信したり、個人データを拡張したりできます。

>[!AVAILABILITY]
>
>すべてのお客様がこの機能を購入しているわけではありません。詳細は、セールス担当者にお問い合わせください。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/create-a-webhook-1.png)

1. 「**[!UICONTROL Webhook]**」をクリックします。

   ![](assets/create-a-webhook-2.png)

1. 「**[!UICONTROL 新規 Webhook]**」をクリックします。

   ![](assets/create-a-webhook-3.png)

1. に名前を付けて設定します。 [!DNL Webhook].

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >多くの場合、使用するサードパーティのサービス証明書を、URL パラメーターまたは POST テンプレートとして入力します。

   * **[!UICONTROL URL]**：Web サービスに対するリクエストで使用する URL を入力します。リードのメールアドレス（**`{{lead.Email Address}}`**）などのトークンをリクエストに挿入するには、「**[!UICONTROL トークンを挿入]**」をクリックします。

   * **[!UICONTROL テンプレート]**:リクエストの本文で情報を送信する場合は、ペイロードテンプレートを使用してを入力します。 次のリクエストタイプに対して許可されているテンプレート：POST、DELETE、PATCHまたはPUT。 JSON や XML などのデータ形式を使用できます。 テンプレートにトークンを挿入するには、「**[!UICONTROL トークンを挿入]**」をクリックします。

   * **[!UICONTROL リクエストトークンのエンコード]**：トークンの値に特殊文字（アンパサンド「&amp;」など）が含まれる場合は、リクエストの形式（**JSON** または&#x200B;**フォーム／URL**）を指定します。

   * **[!UICONTROL 応答タイプ]**：サービスから受け取る応答の形式（**JSON** または **XML**）を選択します。

   * **[!UICONTROL リクエストタイプ]**：使用する HTTP メソッド（DELETE、GET、PATCH、POST、PUT）を選択します。

1. 「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>詳しくは、[[!DNL Webhooks]](https://developers.marketo.com/documentation/webhooks/) の詳細を参照してください。{target="_blank"}
