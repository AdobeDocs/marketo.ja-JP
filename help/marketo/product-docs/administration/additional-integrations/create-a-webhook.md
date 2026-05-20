---
unique-page-id: 2360360
description: 管理画面でWebhookを作成して、SMSや人物データなどのサードパーティのweb サービスに電話できます。
title: ' [!DNL Webhook] の作成'
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
feature: Administration, Webhooks
TQID: https://experienceleague.adobe.com/O4xw1wSvFeTJ2xqZn4Eo7JbrUBQQmKcl7mvLkduFXGc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: fc9b09fe-b844-4544-887b-e420c3b82065
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 220
ht-degree: 81%

---

# [!DNL Webhook] の作成 {#create-a-webhook}

[!DNL Webhooks] を使用すると、サードパーティの web サービスを活用して、テキストメッセージの送信、人物データの拡張などを行うことができます。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/create-a-webhook-1.png)

1. 「**[!UICONTROL Webhook]**」をクリックします。

   ![](assets/create-a-webhook-2.png)

1. 「**[!UICONTROL 新規 Webhook]**」をクリックします。

   ![](assets/create-a-webhook-3.png)

1. [!DNL Webhook] に名前を付けて、設定します。

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >多くの場合、使用するサードパーティのサービス資格情報を、URL パラメーターとして、または POST テンプレートに入力して含めます。

   * **[!UICONTROL URL]**：Web サービスに対するリクエストで使用する URL を入力します。 人物のメールアドレス（**`{{lead.Email Address}}`**）などのトークンをリクエストに挿入するには、「**[!UICONTROL トークンを挿入]**」をクリックします。

   * **[!UICONTROL テンプレート]**: リクエストの本文に情報を送信する場合は、ペイロードテンプレートを使用して入力します。 リクエストタイプ POST、DELETE、PATCH または PUT に対して許可されたテンプレート。 JSON や XML などのデータ形式を使用できます。 テンプレートにトークンを挿入するには、「**[!UICONTROL トークンを挿入]**」をクリックします。

   * **[!UICONTROL リクエストトークンのエンコード]**：トークンの値に特殊文字（アンパサンド「&amp;」など）が含まれる場合は、リクエストの形式（**JSON** または&#x200B;**フォーム／URL**）を指定します。

   * **[!UICONTROL 応答タイプ]**：サービスから受け取る応答の形式（**JSON** または **XML**）を選択します。

   * **[!UICONTROL リクエストタイプ]**：使用する HTTP メソッド（DELETE、GET、PATCH、POST、PUT）を選択します。

1. 「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>詳しくは、[[!DNL Webhooks]](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/webhooks/webhooks){target="_blank"}の詳細をご覧ください。
