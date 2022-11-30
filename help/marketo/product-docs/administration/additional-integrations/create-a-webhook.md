---
unique-page-id: 2360360
description: Webhook の作成 - Marketo ドキュメント - 製品ドキュメント
title: Webhook の作成
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 86%

---

# Webhook の作成 {#create-a-webhook}

Webhook を使用すると、サードパーティの web サービスを活用して、テキストメッセージの送信、リードデータの拡張などを行うことができます。

>[!AVAILABILITY]
>
>すべてのお客様がこの機能を購入しているわけではありません。詳細は、セールス担当者にお問い合わせください。

1. 「**管理者**」領域に移動します。

   ![](assets/create-a-webhook-1.png)

1. クリック **ウェブフック**.

   ![](assets/create-a-webhook-2.png)

1. 「**新規 Webhook**」をクリックします。

   ![](assets/create-a-webhook-3.png)

1. Webhook に名前を付け、設定します。

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >多くの場合、使用するサードパーティのサービス証明書を、URL パラメーターまたは POST テンプレートとして入力します。

   * **URL**:Web サービスへのリクエストで使用する URL を入力します。 リードのメールアドレス（**`{{lead.Email Address}}`**）などのトークンをリクエストに挿入するには、「**トークンを挿入**」をクリックします。

   * **テンプレート**：POST の本文で情報を送信する場合は、テンプレートを入力します。XML、JSON、SOAP など、HTTP POST をサポートする任意のデータ形式を使用します。テンプレートにトークンを挿入するには、「**トークンを挿入**」をクリックします。

   * **リクエストトークンのエンコード**：トークンの値に特殊文字（アンパサンド「&amp;」など）が含まれる場合は、リクエストの形式（**JSON** または&#x200B;**フォーム／URL**）を指定します。

   * **応答タイプ**：サービスから受け取る応答の形式（**JSON** または **XML**）を選択します。

   * **リクエストタイプ**:使用する HTTP メソッド (DELETE、GET、PATCH、POST、PUT) を選択します。

1. 「**作成**」をクリックします。

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>詳しくは、[Webhooks](https://developers.marketo.com/documentation/webhooks/) の詳細を参照してください。
