---
description: Marketo 配信停止チェック - Marketo ドキュメント - 製品ドキュメント
title: Marketo 配信停止チェック
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 100%

---

# Marketo 配信停止チェック {#marketo-unsubscribe-check}

Marketo 配信停止チェックは、チームの Marketo への接続を使用して、Marketo のリード管理システムで配信停止になっているユーザーにメールが送信されるのを防ぎます。セールスユーザーが Marketo Sales を使用してメールを送信すると、そのメール ID が配信停止されているかどうかを確認するために、Marketo に対する API 呼び出しが実行されます。配信停止の場合、メール送信がブロックされます。

>[!NOTE]
>
>**管理者権限が必要**

## 有効にする {#turning-it-on}

1. 歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/marketo-unsubscribe-check-1.png)

1. 「管理設定」で、「**配信停止**」をクリックします。

   ![](assets/marketo-unsubscribe-check-2.png)

1. 「**統合**」タブをクリックします。「Marketo 配信停止チェック」セクションで、スライダーをクリックしてチェックを有効にします。

   ![](assets/marketo-unsubscribe-check-3.png)

## 留意事項 {#things-to-know}

Marketo 配信停止チェックの留意事項は次のとおりです。

* API の制限に対してはカウントしません
* Marketo 接続が確立されている必要があります
* グローバル設定です
* Web アプリケーション、メールクライアント、Salesforce から送信されるメールをブロックします
