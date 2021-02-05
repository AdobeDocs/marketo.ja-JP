---
unique-page-id: 42762825
description: Salesforce Lightning - Marketto Docs — 製品ドキュメントでのバルクアクションの使用
title: Salesforce Lightningでのバルクアクションの使用
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---


# Salesforce Lightningでのバルクアクションの使用{#using-bulk-actions-in-salesforce-lightning}

キャンペーンへのリードの追加、バルク電子メールの送信、SalesforceからSales Connectへのリードのプッシュなど、バルクアクションの実行方法を説明します。

>[!PREREQUISITES]
>
>Sales Connectパッケージの最新バージョンに更新し、リード/コンタクト表示にバルクアクションボタンをインストールします。 [手順については、ここをクリックしてください](http://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)。

>[!NOTE]
>
>次の手順に従う前に、Marketo Sales Connectアカウントにログインしていることを確認してください。

## バルク電子メール{#bulk-email}

1. Salesforceで、「**Leads**」タブをクリックし、目的のリードのリストを選択します。

   ![](assets/one-6.png)

   >[!NOTE]
   >
   >使用するリストに既に存在する場合は、ドロップダウンから選択して再実行し、MSCバルクアクションボタンが表示されることを確認する必要があります。 これは、変更できないSalesforceの動作です。

1. （画面の右端にある）矢印ドロップダウンをクリックし、「**Email with MSC**」を選択します。

   ![](assets/two-6.png)

1. MSC電子メールがポップアップします。 次の機能が含まれます。

   a.「至」フィールドに「すべての入金」が表示されます。これは、リードリスト表示で選択したリードのリストに対応します。\
   b.このリストは、「バルク構成」と呼ばれる左側のパネルに表示されます。受信者はここで追加または削除できます\
   c.テンプレートを選択するか、独自の電子メールを作成できます\
   d.電子メールはすぐに送信することも、後で送信するようにスケジュールすることもできます

   ![](assets/three-5.png)

## 追加キャンペーン{#add-to-campaign}へ

1. Salesforceで、「**Leads**」タブをクリックし、目的のリードのリストを選択します。

   ![](assets/four-4.png)

1. （画面の右端にある）矢印のドロップダウンをクリックし、「**追加 to MSCキャンペーン**」を選択します。

   ![](assets/five-4.png)

1. 「追加キャンペーンに登録したユーザー」ポップアップが表示されます。 「**次へ**」をクリックし、通常のキャンペーンフローを実行して、MSCキャンペーンをトリガーします。

   ![](assets/six-1.png)

## Marketo Sales Connectへのプッシュ{#push-to-marketo-sales-connect}

1. Salesforceで、「**Leads**」タブをクリックし、目的のリードのリストを選択します。

   ![](assets/seven-2.png)

1. （画面の右端にある）矢印ドロップダウンをクリックし、「**MSCにプッシュ**」を選択します。

   ![](assets/eight-2.png)

1. 「Salesforce Bridge」という新しいタブが開きます。 「**グループに進む→**」ボタンをクリックします。

   ![](assets/nine-2.png)

1. MSCアカウントに送信され、日付/時間スタンプで作成されたグループが表示されます。 同期が完了し、Salesforceから同期されたリードがグループに含まれると、通知が受信されます。

   ![](assets/ten-1.png)

>[!NOTE]
>
>同じ手順に従って、連絡先リスト表示でバルクアクションを使用することもできます。

>[!MORELIKETHIS]
>
>* [グループ電子メールを使用した電子メールの送信](http://docs.marketo.com/x/KAQ6Ag)
>* [選択と送信を使用したバルク電子メールの構成](http://docs.marketo.com/display/public/DOCS/Composing+Bulk+Emails+with+Select+and+Send#ComposingBulkEmailswithSelectandSend-SendingEmails)

>



