---
unique-page-id: 2360360
description: Webフックの作成 — Marketto Docs — 製品ドキュメント
title: Webフックの作成
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---


# Webフックの作成 {#create-a-webhook}

Webフックを使用して、サードパーティのWebサービスを利用し、テキストメッセージの送信、個人データの拡張などを行います。

>[!NOTE]
>
>**可用性**
>
>この機能を購入していないお客様もいます。 詳細については、セールス担当者にお問い合わせください。

1. 「**Admin **」に移動し、「 **Webhooks**」をクリックします。

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. 「 **新規Webフック**」をクリックします。

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. Webフックに名前を付け、設定します。

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >これには、多くの場合、サードパーティのサービス資格情報をURLパラメーターとして、またはPOSTテンプレートに入力することが含まれます。

   * **URL**:Webサービスに対する要求のPOSTに使用するURLを入力します。 ユーザーの電子メールアドレス(**`{{lead.Email Address}}`**)などのトークンをリクエストに挿入するには、「トークンの **挿入**」をクリックします。

   * **テンプレート**:POSTの本文に情報を送信する場合は、テンプレートを入力します。 XML、JSON、SOAPなど、HTTPPOSTをサポートする任意のデータ形式を使用します。 テンプレートにトークンを挿入するには、「トークンの **挿入**」をクリックします。

   * **Request Token Encoding**:トークン値に特殊文字（アンパサンド、「&amp;」など）が含まれる場合は、リクエストの形式(**JSON** 、 **フォーム**/URL)を示します。

   * **応答タイプ**:サービスから受け取る応答の形式(**JSON** または **XML**)を選択します。

   「作成」をクリックします。

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>**ディープダイブ**
>
>詳しくは、 [Webhooks](http://developers.marketo.com/documentation/webhooks/) deep diveを参照してください。

