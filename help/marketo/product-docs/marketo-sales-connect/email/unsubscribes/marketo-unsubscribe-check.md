---
unique-page-id: 18317340
description: Marketo 配信停止チェック - Marketo ドキュメント - 製品ドキュメント
title: Marketo 配信停止チェック
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 64%

---

# Marketo 配信停止チェック {#marketo-unsubscribe-check}

[!UICONTROL Marketo登録解除チェック ] は、チームのMarketoへの接続を使用して、Marketo Lead Management system の登録解除したユーザーにメールが送信されないようにします。 営業ユーザーが [!DNL Sales Connect] を含むメールを送信すると、Marketoに対して API 呼び出しが行われ、メール ID が登録解除されているかどうかを確認します。 配信停止の場合、メール送信がブロックされます。

>[!NOTE]
>
>**管理者権限が必要**

## オンにする {#turning-it-on}

1. Web アプリケーションで、歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/one-2.png)

1. [!UICONTROL  管理者設定 ] で、「**[!UICONTROL 購読解除]**」をクリックします。

   ![](assets/two-3.png)

1. 「**[!UICONTROL 統合]**」をクリックします。

   ![](assets/three-3.png)

1. 「[!UICONTROL Marketo登録解除チェック ]」セクションで、スライダーをクリックしてチェックをアクティブにします。

   ![](assets/four-2.png)

## 留意事項 {#things-to-know}

Marketo 配信停止チェックの留意事項は次のとおりです。

* API の制限に対してはカウントしません
* Marketo 接続が確立されている必要があります
* グローバル設定です
* Web アプリケーション、メールクライアント、Salesforce から送信されるメールをブロックします
* 失敗したメールをログに記録するか、ユーザーがすべてのワークフロー（メールプラグイン送信、個別送信、販売キャンペーン送信、複数選択および送信）で送信しようとすると、送信を阻止します。[グループメール](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md)の場合は、メールの送信を静かに阻止します
