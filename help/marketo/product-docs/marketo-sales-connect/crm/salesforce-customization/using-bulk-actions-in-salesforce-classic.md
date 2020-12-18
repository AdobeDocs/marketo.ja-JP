---
unique-page-id: 42762794
description: Salesforce Classic - Marketto Docs — 製品ドキュメントでのバルクアクションの使用
title: Salesforce Classicでのバルクアクションの使用
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---


# Salesforce Classicでのバルクアクションの使用{#using-bulk-actions-in-salesforce-classic}

キャンペーンへのリードの追加、バルク電子メールの送信、SalesforceからSales Connectへのリードのプッシュなど、バルクアクションの実行方法を説明します。

>[!PREREQUISITES]
>
>Sales Connectパッケージの最新バージョンに更新し、リード/コンタクト表示にバルクアクションボタンをインストールします。 [手順については、ここをクリックしてください](http://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf)。

>[!NOTE]
>
>概要を説明した手順に従う前に、Marketo Sales Connectアカウントにログインしていることを確認します。

## バルク電子メール{#bulk-email}

1. Salesforceで、「**Leads**」タブをクリックし、「**Go**」ボタンをクリックします。

   ![](assets/one-5.png)

1. 目的のリードを選択し、「**Email with MSC (Classic)**」ボタンをクリックします。

   ![](assets/two-5.png)

1. MSC電子メールがポップアップします。 次の機能が含まれます。

   a.「至」フィールドに「すべての入金」が表示されます。これは、リードリスト表示で選択したリードのリストに対応します。\
   b.このリストは、「バルク構成」と呼ばれる左側のパネルに表示されます。受信者はここで追加または削除できます\
   c.テンプレートを選択するか、独自の電子メールを作成できます\
   d.電子メールに入力される動的フィールドをプレビューできます\
   e.電子メールはすぐに送信することも、後で送信するようにスケジュールすることもできます

   ![](assets/three-4.png)

## 追加キャンペーン{#add-to-campaign}へ

1. Salesforceで、「**Leads**」タブをクリックし、「**Go**」ボタンをクリックします。

   ![](assets/four-3.png)

1. 目的のリードを選択し、「**MSCキャンペーン追加（クラシック）**」ボタンをクリックします。

   ![](assets/five-3.png)

1. 「追加キャンペーンに登録したユーザー」ポップアップが表示されます。 「**次へ**」をクリックし、一般的なキャンペーン・フローを実行して、MSCキャンペーンをトリガーします。

   ![](assets/six.png)

## Marketo Sales Connectへのプッシュ{#push-to-marketo-sales-connect}

1. Salesforceで、「**Leads**」タブをクリックし、「**Go**」ボタンをクリックします。

   ![](assets/seven-1.png)

1. 目的のリードを選択し、「**MSCにプッシュ（クラシック）**」ボタンをクリックします。

   ![](assets/eight-1.png)

1. 「Salesforce Bridge」という新しいタブが開きます。 「**グループに進む→**」ボタンをクリックします。

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



