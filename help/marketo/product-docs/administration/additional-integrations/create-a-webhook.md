---
unique-page-id: 2360360
description: Webフックの作成 —Marketoドキュメント — 製品ドキュメント
title: Webフックの作成
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 3%

---

# Webフックの作成{#create-a-webhook}

Webフックを使用して、サードパーティのWebサービスを利用し、テキストメッセージの送信、個人データの拡張などを行います。

>[!AVAILABILITY]
>
>この機能を購入していないお客様もいます。  詳細は、営業取引先責任者にお問い合わせください。

1. 「**管理者**」に移動し、「**Webhooks**」をクリックします。

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. 「**New Webhook**」をクリックします。

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. Webフックに名前を付け、設定します。

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >これには、多くの場合、サードパーティのサービス資格情報をURLパラメーターとして、またはPOSTテンプレートに入力することが含まれます。

   * **URL**:Webサービスに対する要求のPOSTに使用するURLを入力します。ユーザーの電子メールアドレス(**`{{lead.Email Address}}`**)などのトークンをリクエストに挿入するには、「**トークンの挿入**」をクリックします。

   * **テンプレート**:POSTの本文に情報を送信する場合は、テンプレートを入力します。XML、JSON、SOAPなど、HTTPPOSTをサポートする任意のデータ形式を使用します。 テンプレートにトークンを挿入するには、**「トークンを挿入**」をクリックします。

   * **Request Token Encoding**:トークン値に特殊文字（アンパサンド、「&amp;」など）が含まれる場合は、リクエストの形式(**** JSONまたは **フォーム/URL**)を示します。

   * **応答タイプ**:サービスから受け取る応答の形式(**** JSONまたは **XML**)を選択します。

   「作成」をクリックします。

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>詳しくは、[webhooks](https://developers.marketo.com/documentation/webhooks/)深い潜水所を参照してください。
