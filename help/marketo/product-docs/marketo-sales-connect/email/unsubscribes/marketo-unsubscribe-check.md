---
unique-page-id: 18317340
description: Marketo配信停止の確認 — Marketoドキュメント — 製品ドキュメント
title: Marketo 配信停止チェック
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
source-git-commit: 82c75d52caf3a0320cd3e8534b3b0870cf12d660
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 11%

---

# Marketo 配信停止チェック {#marketo-unsubscribe-check}

Marketo配信停止チェックは、チームのMarketoへの接続を使用して、Marketoのリード管理システムで配信停止になったユーザーにメールが送信されるのを防ぎます。 セールスユーザーが Sales Connect の電子メールを送信すると、電子メール ID が配信停止になっているかどうかを確認するために、Marketoに対する API 呼び出しがおこなわれます。 その場合、E メールの送信がブロックされます。

>[!NOTE]
>
>**管理者権限が必要**

## オンにする {#turning-it-on}

1. Web アプリケーションで、歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/one-2.png)

1. 管理者設定で、 **配信停止**.

   ![](assets/two-3.png)

1. クリック **統合**.

   ![](assets/three-3.png)

1. 「 Marketo Unsubscribe Check 」セクションで、スライダーをクリックしてチェックを有効にします。

   ![](assets/four-2.png)

## 留意事項 {#things-to-know}

Marketo配信停止の確認…

* API の制限に対してはカウントされません
* Marketo接続が確立されている必要があります
* グローバル設定です
* Web アプリケーション、メールクライアント、Salesforce から送信されるメールをブロックします
* 失敗した電子メールをログに記録するか、以外のすべてのワークフロー（電子メールプラグインの送信、個別の送信、セールスキャンペーンの送信、複数の選択と送信）でユーザーが送信しようとした場合に送信を防ぎます。 [グループメール](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md):E メールが黙って送信されるのを防ぎます。
