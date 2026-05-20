---
unique-page-id: 14352484
description: Sales ConnectをSalesforceに接続する際に、「リクエストを認証できませんでした」エラーを修正する方法について説明します。 認証の問題のトラブルシューティング。
title: Salesforce に接続する際の「リクエストを認証できませんでした」の修正方法
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/51pd-hGwspmp6ZuOShb3z3wRdQ0PZ-pCIY-BeV4Q5ho
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 175
ht-degree: 88%

---

# [!DNL Salesforce] に接続する際の「リクエストを認証できませんでした」の修正方法 {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

[!DNL Sales Connect] を [!DNL Salesforce] に接続しようとしたときに「リクエストを認証できませんでした」というエラーメッセージが表示された場合は、[!DNL Salesforce] の API へのアクセスに制約がある可能性があります。 [!DNL Salesforce] 管理者に次の点を確認してください。

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
1. [!DNL Sales Connect] の横に「[!UICONTROL ブロック]」と表示されていることを確認します。 「[!UICONTROL ブロック解除]」が表示されたらボタンをクリックして、[!DNL Sales Connect] の [!DNL Salesforce] へのアクセスのブロックを解除します。
