---
description: Marketo 配信停止チェック - Marketo ドキュメント - 製品ドキュメント
title: Marketo 配信停止チェック
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 45%

---

# [!UICONTROL Marketo 登録解除チェック] {#marketo-unsubscribe-check}

[!UICONTROL Marketo登録解除チェック ] は、チームのMarketoへの接続を使用して、Marketo Lead Management system の登録解除したユーザーにメールが送信されないようにします。 営業ユーザーが [!DNL Marketo Sales] を含むメールを送信すると、Marketoに対して API 呼び出しが行われ、メール ID が登録解除されているかどうかを確認します。 配信停止の場合、メール送信がブロックされます。

>[!NOTE]
>
>**管理者権限が必要**

## 有効にする {#turning-it-on}

1. 歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/marketo-unsubscribe-check-1.png)

1. [!UICONTROL  管理者設定 ] で、「**[!UICONTROL 購読解除]**」をクリックします。

   ![](assets/marketo-unsubscribe-check-2.png)

1. 「**[!UICONTROL 統合]**」タブをクリックします。「[!UICONTROL Marketo登録解除チェック ]」セクションで、スライダーをクリックしてチェックをアクティブにします。

   ![](assets/marketo-unsubscribe-check-3.png)

## 留意事項 {#things-to-know}

Marketo 配信停止チェックの留意事項は次のとおりです。

* API の制限に対してはカウントしません
* Marketo 接続が確立されている必要があります
* グローバル設定です
* Web アプリケーション、メールクライアントおよび [!DNL Salesforce] から送信されるメールをブロックします
