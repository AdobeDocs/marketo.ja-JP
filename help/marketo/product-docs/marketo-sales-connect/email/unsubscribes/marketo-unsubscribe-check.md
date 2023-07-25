---
unique-page-id: 18317340
description: Marketo 配信停止チェック - Marketo ドキュメント - 製品ドキュメント
title: Marketo 配信停止チェック
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 100%

---

# Marketo 配信停止チェック {#marketo-unsubscribe-check}

Marketo 登録解除チェックは、チームの Marketo への接続を使用して、Marketo のリード管理システムで登録解除になっているユーザーにメールが送信されるのを防ぎます。セールスユーザーが Sales Connect でメールを送信すると、メール ID が登録解除されているかどうかを確認するために、Marketo に対して API が呼び出されます。登録解除されている場合、メールの送信がブロックされます。

>[!NOTE]
>
>**管理者権限が必要**

## オンにする {#turning-it-on}

1. Web アプリケーションで、歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/one-2.png)

1. 管理設定で、「**登録解除**」をクリックします。

   ![](assets/two-3.png)

1. 「**統合**」をクリックします。

   ![](assets/three-3.png)

1. Marketo 登録解除チェックセクションで、スライダーをクリックしてチェックを有効にします。

   ![](assets/four-2.png)

## 留意事項 {#things-to-know}

Marketo 配信停止チェックの留意事項は次のとおりです。

* API の制限に対してはカウントしません
* Marketo 接続が確立されている必要があります
* グローバル設定です
* Web アプリケーション、メールクライアント、Salesforce から送信されるメールをブロックします
* 失敗したメールをログに記録するか、ユーザーがすべてのワークフロー（メールプラグイン送信、個別送信、販売キャンペーン送信、複数選択および送信）で送信しようとすると、送信を阻止します。[グループメール](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md)の場合は、メールの送信を静かに阻止します
