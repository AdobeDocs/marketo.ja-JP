---
unique-page-id: 2360360
description: Webhook の作成 - Marketo ドキュメント - 製品ドキュメント
title: Webhook の作成
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
source-git-commit: a498dcc5dc95bd7f732481d30db021485cf052c0
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 81%

---

# Webhook の作成 {#create-a-webhook}

Webhook を使用すると、サードパーティの web サービスを活用して、テキストメッセージの送信、リードデータの拡張などを行うことができます。

>[!AVAILABILITY]
>
>すべてのお客様がこの機能を購入しているわけではありません。詳細は、セールス担当者にお問い合わせください。

1. 「**管理者**」領域に移動します。

   ![](assets/create-a-webhook-1.png)

1. 「**Webhook**」をクリックします。

   ![](assets/create-a-webhook-2.png)

1. 「**新規 Webhook**」をクリックします。

   ![](assets/create-a-webhook-3.png)

1. Webhook に名前を付け、設定します。

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >多くの場合、使用するサードパーティのサービス証明書を、URL パラメーターまたは POST テンプレートとして入力します。

   * **URL**：Web サービスに対するリクエストで使用する URL を入力します。リードのメールアドレス（**`{{lead.Email Address}}`**）などのトークンをリクエストに挿入するには、「**トークンを挿入**」をクリックします。

   * **テンプレート**:リクエストの本文で情報を送信する場合は、ペイロードテンプレートを使用してを入力します。 次のリクエストタイプに対して許可されているテンプレート：POST、DELETE、PATCHまたはPUT。 JSON や XML などのデータ形式を使用できます。 テンプレートにトークンを挿入するには、「**トークンを挿入**」をクリックします。

   * **リクエストトークンのエンコード**：トークンの値に特殊文字（アンパサンド「&amp;」など）が含まれる場合は、リクエストの形式（**JSON** または&#x200B;**フォーム／URL**）を指定します。

   * **応答タイプ**：サービスから受け取る応答の形式（**JSON** または **XML**）を選択します。

   * **リクエストタイプ**：使用する HTTP メソッド（DELETE、GET、PATCH、POST、PUT）を選択します。

1. 「**作成**」をクリックします。

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>詳しくは、[Webhooks](https://developers.marketo.com/documentation/webhooks/) の詳細を参照してください。
