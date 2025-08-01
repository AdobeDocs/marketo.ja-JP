---
description: Salesforce でのセールスキャンペーンへの一括追加の使用 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce でのセールスキャンペーンへの一括追加の使用
exl-id: e518fe82-e37d-4edd-8a31-19268f6fd4b1
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 95%

---

# Salesforce でのセールスキャンペーンへの一括追加の使用 {#using-bulk-add-to-sales-campaign-in-salesforce}

Sales Actions を使用したアウトバウンド通信の拡大に役立つ、Salesforce でのセールスキャンペーンへの一括追加方法を説明します。

>[!NOTE]
>
>Salesforce では、一度に選択できるレコード数が 200 に制限されます。

>[!PREREQUISITES]
>
>[ 最新の Sales Insight パッケージ ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} がSalesforce インスタンスにインストールされ、Salesforceの連絡先ビューとリードリストビューで [ アクションボタン ](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/add-action-buttons-to-salesforce-list-view.md){target="_blank"} が設定されていることを確認します。

## Salesforce Lightning でのセールスキャンペーンへの一括追加 {#bulk-add-to-sales-campaign-in-salesforce-lightning}

1. Salesforce で、「**リード／連絡先**」タブをクリックして、リード／連絡先ホームページに移動します。

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-1.png)

1. **表示**&#x200B;ドロップダウンで、メールを送信するリード／連絡先の目的の表示を選択します。

   >[!TIP]
   >
   >右側の歯車アイコンをクリックして、「**新規**」を選択することで、新しい表示を作成できます。表示に新しい名前を付けて保存したら、右側のフィルターアイコンをクリックして、メールを送信するリード／連絡先の目的のセットに絞り込むことができます。

1. 目的のリードまたは連絡先のリストを選択して、「**セールスキャンペーンに追加**」ボタンをクリックします。

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-2.png)

1. 選択した受信者が追加された、Actions セールスキャンペーンモーダルが表示されます。

1. 人物またはグループを削除するために必要な編集を行ったら、「**次へ**」をクリックします。

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-3.png)

1. カテゴリドロップダウンから使用したいセールスキャンペーンカテゴリを選択します。

1. 選択した人物を追加したいセールスキャンペーンを選択して、「**次へ**」をクリックします。

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-4.png)

1. キャンペーンの最初のステップに応じて、異なるオプションが表示される可能性があります。最初のステップがメールの場合は、以下のように、各受信者のメールを編集するオプションが表示されます。これが完了したら、「**次へ**」をクリックします。

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-5.png)

1. さらに、最初のステップがメールで、キャンペーンが開始される際に選択できるように設定されている場合は、「**今すぐ開始**」または「**新しい開始時刻をスケジュール**」オプションが表示されます。これが完了したら、「**開始**」をクリックします。

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-6.png)

「開始」をクリックすると、追加された人数を知らせる確認画面が表示されます。

![](assets/using-bulk-add-to-sales-campaign-in-salesforce-7.png)

## Salesforce Classic でのセールスキャンペーンへの一括追加 {#bulk-add-to-sales-campaign-in-salesforce-classic}

1. Salesforce で、「**リード／連絡先**」タブをクリックします。

1. 表示ドロップダウンで、メールを送信するリード／連絡先の目的の表示を選択して、「**移動**」をクリックします。

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-8.png)

   >[!TIP]
   >
   >「ビューの新規作成」をクリックして、メールを送信する受信者のリストを絞り込むための使用可能なフィルターを設定することで、新しい表示を作成できます。

1. 目的のリードまたは連絡先のリストを選択して、「**セールスキャンペーンに追加**」ボタンをクリックします。

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-9.png)

1. 選択した人物が追加された、Actions セールスキャンペーンモーダルが表示されます。

1. 人物またはグループを削除するために必要な編集を行ったら、「**次へ**」をクリックします。

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-10.png)

1. **カテゴリ**&#x200B;ドロップダウンから使用したいセールスキャンペーンカテゴリを選択します。

1. 選択した人物を追加したいセールスキャンペーンを選択して、「**次へ**」をクリックします。

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-11.png)

1. キャンペーンの最初のステップに応じて、異なるオプションが表示される可能性があります。最初のステップがメールの場合は、以下のように、各受信者のメールを編集するオプションが表示されます。これが完了したら、「**次へ**」をクリックします。

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-12.png)

1. さらに、最初のステップがメールで、キャンペーンが開始される際に選択できるように設定されている場合は、「**今すぐ開始**」または「**新しい開始時刻をスケジュール**」オプションが表示されます。これが完了したら、「**開始**」をクリックします。

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-13.png)

「開始」をクリックすると、追加された人数を知らせる確認画面が表示されます。

![](assets/using-bulk-add-to-sales-campaign-in-salesforce-14.png)
