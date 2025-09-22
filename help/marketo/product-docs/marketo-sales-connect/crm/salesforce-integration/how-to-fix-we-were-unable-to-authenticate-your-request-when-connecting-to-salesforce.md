---
unique-page-id: 14352484
description: Salesforce に接続する際の「リクエストを認証できませんでした」の修正方法 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce に接続する際の「リクエストを認証できませんでした」の修正方法
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
feature: Marketo Sales Connect
source-git-commit: 65d607e279fb86b0816ccaec2f4bf3c69e309cb9
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 100%

---

# [!DNL Salesforce] に接続する際の「リクエストを認証できませんでした」の修正方法 {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

[!DNL Sales Connect] を [!DNL Salesforce] に接続しようとしたときに「リクエストを認証できませんでした」というエラーメッセージが表示された場合は、[!DNL Salesforce] の API へのアクセスに制約がある可能性があります。[!DNL Salesforce] 管理者に次の点を確認してください。

## ユーザ権限での API の有効化 {#enable-api-in-user-permissions}

1. [!DNL Salesforce] 管理者に SFDC にログインしてもらいます。
1. 「**[!UICONTROL 設定]**」を選択します。
1. 「**[!UICONTROL ユーザを管理]**」を選択します。
1. 「**[!UICONTROL プロファイル]**」を選択します。
1. ToutApp ユーザが属するプロファイルを探し、「**[!UICONTROL 編集]**」をクリックします。
1. 下の「**[!UICONTROL 管理権限]**」までスクロールし、「**[!UICONTROL API 有効]**」がオンになっていることを確認します。

## [!DNL Salesforce] が [!DNL Sales Connect] の接続をブロックしているかどうかを確認 {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. [!DNL Salesforce] 管理者に SFDC にログインしてもらいます。
1. 「**[!UICONTROL 設定]**」を選択します。
1. 「**[!UICONTROL アプリの管理]**」を選択します。
1. 「**[!UICONTROL 接続済みのアプリケーションの OAuth 使用状況]**」を選択します。
1. [!DNL Sales Connect] の横に「[!UICONTROL ブロック]」と表示されていることを確認します。「[!UICONTROL ブロック解除]」が表示されたらボタンをクリックして、[!DNL Sales Connect] の [!DNL Salesforce] へのアクセスのブロックを解除します。
