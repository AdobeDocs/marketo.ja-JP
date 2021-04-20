---
unique-page-id: 18317340
description: Marketo登録解除チェック —Marketoドキュメント — 製品ドキュメント
title: Marketo 配信停止チェック
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 4%

---

# Marketo 配信停止チェック {#marketo-unsubscribe-check}

Marketo登録解除チェックは、チームのMarketoへの接続を使用して、Marketoのリード管理システムで登録解除されたユーザーに電子メールが送信されるのを防ぎます。 販売ユーザーがSales Connectの電子メールを送信すると、電子メールIDが登録解除されたかどうかを確認するために、MarketoにAPI呼び出しが行われます。 メールが送信されている場合は、メールの送信をブロックします。

>[!NOTE]
>
>**必要な管理者権限**

## {#turning-it-on}をオンにする

1. Webアプリケーションで、歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/one-2.png)

1. 「管理者設定」で、「**購読解除**」をクリックします。

   ![](assets/two-3.png)

1. 「**統合**」をクリックします。

   ![](assets/three-3.png)

1. [Marketo登録解除チェック]セクションで、スライダをクリックしてチェックをアクティブにします。

   ![](assets/four-2.png)

## {#things-to-know}の知り合い

Marketoの登録解除のチェック…

* APIの制限に対してカウントされません。
* Marketo接続の確立が必要です
* グローバル設定です
* Webアプリケーション、電子メールクライアントおよびSalesforceから送信される電子メールをブロックします。
