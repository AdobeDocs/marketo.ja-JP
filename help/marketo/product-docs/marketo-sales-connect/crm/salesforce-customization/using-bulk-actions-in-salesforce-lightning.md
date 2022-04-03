---
unique-page-id: 42762825
description: Salesforce Lightning での一括アクションの使用 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce Lightning での一括アクションの使用
exl-id: 72022507-6568-4cc2-b3b5-c1703a1493ad
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '416'
ht-degree: 100%

---

# Salesforce Lightning での一括アクションの使用 {#using-bulk-actions-in-salesforce-lightning}

キャンペーンへのリードの追加、一括メールの送信、Salesforce から Sales Connect へのリードのプッシュなど、一括アクションの実行方法を説明します。

>[!PREREQUISITES]
>
>Sales Connect パッケージの最新バージョンに更新し、リード／連絡先ビューに一括アクションボタンをインストールします。[手順については、ここをクリックしてください](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)。

>[!NOTE]
>
>以下の手順に従う前に、Marketo Sales Connect アカウントにログインしていることを確認してください。

## 一括メール {#bulk-email}

1. Salesforce で、「**リード**」タブをクリックし、目的のリードのリストを選択します。

   ![](assets/one-6.png)

   >[!NOTE]
   >
   >既に使用するリストに存在する場合は、「MSC 一括アクション」ボタンが表示されるように、ドロップダウンからリストを選択して再実行する必要があります。これは、変更できない Salesforce の動作です。

1. （画面の右端にある）矢印ドロップダウンをクリックし、「**MSC でのメール**」を選択します。

   ![](assets/two-6.png)

1. MSC メールがポップアップ表示されます。次の機能が含まれます。

   a.「宛先」フィールドに「すべての領収書」が表示されます。これは、リードリスト表示で選択したリードのリストに対応します。\
   b. このリストは左側の一括作成パネルに表示されます。受信者はここで追加または削除できます。\
   c. テンプレートを選択するか、独自のメールを作成できます。\
   d. メールをすぐに送信したり、後で送信するようにスケジュールを設定したりできます。

   ![](assets/three-5.png)

##  キャンペーンに追加 {#add-to-campaign}

1. Salesforce で、「**リード**」タブをクリックし、目的のリードのリストを選択します。

   ![](assets/four-4.png)

1. （画面の右端にある）矢印ドロップダウンをクリックし、「**MSC キャンペーンに追加**」を選択します。

   ![](assets/five-4.png)

1. キャンペーンにリードを追加ポップアップが表示されます。「**次へ**」をクリックし、通常のキャンペーンフローを実行して、MSC キャンペーンをトリガーします。

   ![](assets/six-1.png)

## Marketo セールスコネクトにプッシュ {#push-to-marketo-sales-connect}

1. Salesforce で、「**リード**」タブをクリックし、目的のリードのリストを選択します。

   ![](assets/seven-2.png)

1. （画面の右端にある）矢印ドロップダウンをクリックし、「**MSC にプッシュ**」を選択します。

   ![](assets/eight-2.png)

1. 「Salesforce Bridge」という新しいタブが開きます。「**グループに進む→**」ボタンをクリックします。

   ![](assets/nine-2.png)

1. MSC アカウントに送信され、日時スタンプを使用して作成されたグループが表示されます。同期が完了すると、通知が届き、Salesforce から同期されたリードがグループに含まれます。

   ![](assets/ten-1.png)

>[!NOTE]
>
>同じ手順に従って、連絡先リスト表示でバルクアクションを使用することもできます。

>[!MORELIKETHIS]
>
>* [グループメールによるメールの送信](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [「選択して送信」による一括メールの作成](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)

