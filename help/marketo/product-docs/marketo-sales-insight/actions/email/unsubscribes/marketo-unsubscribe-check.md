---
description: Marketo配信停止の確認 — Marketoドキュメント — 製品ドキュメント
title: Marketo 配信停止チェック
hide: true
hidefromtoc: true
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 13%

---

# Marketo 配信停止チェック {#marketo-unsubscribe-check}

Marketo配信停止チェックは、チームのMarketoへの接続を使用して、Marketoのリード管理システムで配信停止になったユーザーにメールが送信されるのを防ぎます。 セールスユーザーがMarketo Sales と共に電子メールを送信すると、電子メール ID が購読解除されているかどうかを確認するために、Marketoに対する API 呼び出しが実行されます。 その場合、E メールの送信がブロックされます。

>[!NOTE]
>
>**管理者権限が必要**

## オンにする {#turning-it-on}

1. 歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/marketo-unsubscribe-check-1.png)

1. 管理者設定で、 **配信停止**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. 次をクリック： **統合** タブをクリックします。 「 Marketo Unsubscribe Check 」セクションで、スライダーをクリックしてチェックを有効にします。

   ![](assets/marketo-unsubscribe-check-3.png)

## 留意事項 {#things-to-know}

Marketo配信停止の確認…

* API の制限に対してはカウントされません
* Marketo接続が確立されている必要があります
* グローバル設定です
* Web アプリケーション、メールクライアント、Salesforce から送信されるメールをブロックします
