---
unique-page-id: 42762794
description: Salesforce Classic - Marketto Docs — 製品ドキュメントでのバルクアクションの使用
title: Salesforce Classicでのバルクアクションの使用
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---


# Salesforce Classicでのバルクアクションの使用 {#using-bulk-actions-in-salesforce-classic}

キャンペーンへのリードの追加、バルク電子メールの送信、SalesforceからSales Connectへのリードのプッシュなど、バルクアクションの実行方法を説明します。

>[!NOTE]
>
>**前提条件**
>
>Sales Connectパッケージの最新バージョンに更新し、リード/コンタクト表示にバルクアクションボタンをインストールします。 [手順については、ここをクリックしてください](http://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf)。

>[!NOTE]
>
>概要を説明した手順に従う前に、Marketo Sales Connectアカウントにログインしていることを確認します。

## 一括電子メール {#bulk-email}

1. Salesforceで、「 **Leads** 」タブをクリックし、「 **Go** 」ボタンをクリックします。

   ![](assets/one-5.png)

1. 目的のリードを選択し、「 **Email with MSC(Classic)** 」ボタンをクリックします。

   ![](assets/two-5.png)

1. MSC電子メールがポップアップします。 次の機能が含まれます。

   a.「至」フィールドに「すべての入金」が表示されます。これは、リードリスト表示で選択したリードのリストに対応します。\
   b.このリストは、「バルク構成」と呼ばれる左側のパネルに表示されます。受信者はここで追加または削除できます\
   c.テンプレートを選択するか、独自の電子メールを作成できます\
   d.電子メールに入力される動的フィールドをプレビューできます\
   e.電子メールはすぐに送信することも、後で送信するようにスケジュールすることもできます

   ![](assets/three-4.png)

## キャンペーン追加へ {#add-to-campaign}

1. Salesforceで、「 **Leads** 」タブをクリックし、「 **Go** 」ボタンをクリックします。

   ![](assets/four-3.png)

1. 目的のリードを選択し、「MSCキャンペーン **追加へ」（クラシック）ボタンをクリックし** ます。

   ![](assets/five-3.png)

1. 「追加キャンペーンに登録したユーザー」ポップアップが表示されます。 「 **次へ** 」をクリックし、一般的なキャンペーン・フローに従ってMSCキャンペーンをトリガーします。

   ![](assets/six.png)

## Marketor Sales Connectへのプッシュ {#push-to-marketo-sales-connect}

1. Salesforceで、「 **Leads** 」タブをクリックし、「 **Go** 」ボタンをクリックします。

   ![](assets/seven-1.png)

1. 目的のリードを選択し、「 **MSCにプッシュ（クラシック）** 」ボタンをクリックします。

   ![](assets/eight-1.png)

1. 「Salesforce Bridge」という新しいタブが開きます。 「グループに **進む」ボタンをクリックし** ます。

   ![](assets/nine-1.png)

1. MSCアカウントに送信され、日付/時間スタンプで作成されたグループが表示されます。 同期が完了し、Salesforceから同期されたリードがグループに含まれると、通知が受信されます。

   ![](assets/ten.png)

>[!NOTE]
>
>同じ手順に従って、連絡先リスト表示でバルクアクションを使用することもできます。

>[!NOTE]
>
>**関連記事**
>
>* [グループ電子メールを使用した電子メールの送信](http://docs.marketo.com/x/KAQ6Ag)
>* [選択と送信を使用したバルク電子メールの構成](http://docs.marketo.com/display/public/DOCS/Composing+Bulk+Emails+with+Select+and+Send#ComposingBulkEmailswithSelectandSend-SendingEmails)

>



