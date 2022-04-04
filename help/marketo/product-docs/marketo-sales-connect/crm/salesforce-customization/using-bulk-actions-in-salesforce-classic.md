---
unique-page-id: 42762794
description: Salesforce Classic での一括アクションの使用 — Marketo ドキュメント — 製品ドキュメント
title: Salesforce Classic での一括アクションの使用
exl-id: f676ba65-6bc9-41e5-aa70-0f10bceedab7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '372'
ht-degree: 100%

---

# Salesforce Classic での一括アクションの使用 {#using-bulk-actions-in-salesforce-classic}

キャンペーンへのリードの追加、一括メールの送信、Salesforce から Sales Connect へのリードのプッシュなど、バルクアクションの実行方法を説明します。

>[!PREREQUISITES]
>
>Sales Connect パッケージの最新バージョンに更新し、リード／連絡先表示に一括アクションボタンをインストールします。[手順については、ここをクリックしてください](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf)

>[!NOTE]
>
>概要を説明する手順に従う前に、Marketo Sales Connect アカウントにログインしていることを確認してください。

## 一括メール {#bulk-email}

1. Salesforce で、「**リード**」タブ、「**移動**」ボタンをクリックします。

   ![](assets/one-5.png)

1. 目的のリードを選択し、「**MSC でのメール（クラシック）**」ボタンをクリックします。

   ![](assets/two-5.png)

1. MSC メールがポップアップ表示されます。次の機能が含まれます。

   a.「宛先」フィールドに「すべての領収書」が表示されます。これは、リードリスト表示で選択したリードのリストに対応します。\
   b.このリストは左側のパネル「一括作成」に表示されます。受信者はここで追加または削除できます\
   c.テンプレートを選択するか、独自のメールを作成できます。\
   d.メールに入力される動的フィールドをプレビューできます。\
   E. メールをすぐに送信したり、後で送信するようにスケジュールを設定したりできます。

   ![](assets/three-4.png)

## キャンペーンに追加 {#add-to-campaign}

1. Salesforce で、「**リード**」タブ、「**移動**」ボタンをクリックします。

   ![](assets/four-3.png)

1. 目的のリードを選択し、「**MSC キャンペーンに追加（クラシック）**」ボタンをクリックします。

   ![](assets/five-3.png)

1. 「キャンペーンにリードを追加」ポップアップが表示されます。「**次へ**」をクリックし、一般的なキャンペーンフローを調べて、MSC キャンペーンをトリガーします。

   ![](assets/six.png)

## Marketo セールスコネクトにプッシュ {#push-to-marketo-sales-connect}

1. Salesforce で、「**リード**」タブ、「**移動**」ボタンをクリックします。

   ![](assets/seven-1.png)

1. 目的のリードを選択し、「**MSC にプッシュ（クラシック）**」ボタンをクリックします。

   ![](assets/eight-1.png)

1. 「Salesforce Bridge」という新しいタブが開きます。「**グループに進む→**」ボタンをクリックします。

   ![](assets/nine-1.png)

1. MSC アカウントに送信され、日時スタンプを使用して作成されたグループが表示されます。同期が完了すると、通知が届き、Salesforce から同期されたリードがグループに含まれます。

   ![](assets/ten.png)

>[!NOTE]
>
>同じ手順に従って、連絡先リスト表示でバルクアクションを使用することもできます。

>[!MORELIKETHIS]
>
>* [グループメールによるメールの送信](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [「選択して送信」による一括メールの作成](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)

