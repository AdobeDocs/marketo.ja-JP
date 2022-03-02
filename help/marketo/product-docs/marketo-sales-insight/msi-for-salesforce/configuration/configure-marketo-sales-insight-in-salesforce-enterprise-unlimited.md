---
unique-page-id: 2360368
description: Salesforce Enterprise／Unlimited での Marketo Sales Insight の設定 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce Enterprise／Unlimited での Marketo Sales Insight の設定
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
source-git-commit: 6ef1ff6f417cc3118e0c573896e1d232a5b97e70
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 93%

---

# Salesforce Enterprise／Unlimited での Marketo Sales Insight の設定 {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Salesforce Enterprise／Unlimited Editions で Marketo Sales Insight を設定するために必要な手順を次に示します。それでは始めましょう。

>[!PREREQUISITES]
>
>[Salesforce AppExchange での Marketo Sales Insight パッケージのインストール](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**管理者権限が必要**

## Marketo での Sales Insight の設定 {#configure-sales-insight-in-marketo}

1. Marketo で MSI 資格情報を取得します。管理エリアに移動し、「**Sales Insight**」を選択します。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. 「**API 設定を編集**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. 任意の API 秘密鍵を入力し、「**保存**」をクリックします。API 秘密鍵にアンパサンド（&amp;）を使用しないでください。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >API 秘密鍵は組織のパスワードと同じです。安全に保管してください。

1. Rest API 設定パネルの「**表示**」をクリックして、認証情報を設定します。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. 確認ポップアップが表示されます。「**OK**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >このウィンドウは開いたままにしておきます。この情報は、後で Salesforce で必要になります。

## Salesforce での Sales Insight の設定 {#configure-sales-insight-in-salesforce}

1. Salesforce で、「**設定**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. 「リモートサイト」を検索し、「**リモートサイトの設定**」を選択します。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. 「**新規リモートサイト**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. リモートサイト名を入力します（「MarketoSoapAPI」など）。Marketo の Soap API 設定パネルから、「リモートサイト URL」に「Marketo ホスト URL」と入力します。「**保存**」をクリックします。これで、Soap API 用のリモートサイト設定が作成されました。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. もう一度「**新規リモートサイト**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. リモートサイト名を入力します（「MarketoAPI」など）。「リモートサイト URL」に、Marketo の Rest API 設定パネルの API URL を入力します。「**保存**」をクリックします。Rest API 用のリモートサイト設定が作成されました。

   >[!NOTE]
   >
   >__「**リモートサイト名**」を選択します（MarketoAPI はここで使用されます）。**リモートサイト URL** は、「Marketo での Sales Insight の設定」節の手順 3、API 設定を編集ダイアログボックスの「Marketo ホスト」フィールドにあります。

## ページレイアウトのカスタマイズ {#customize-page-layouts}

1. 「**設定**」をクリックします。

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 「ページレイアウト」を検索し、「**リード**」の下の「**ページレイアウト**」を選択します。

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. 左側の「**Visualforce Pages**」をクリックします。「**セクション**」をカスタムリンクセクションの下のレイアウトにドラッグします。

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. 「**セクション名**」に「Marketo Sales Insight」と入力します。「**1 列**」を選択し、「**OK**」をクリックします。

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. 「**リード**」を新しいセクションにドラッグ＆ドロップします。

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >このボックスの名前は、オブジェクトの種類に基づいて変更されます。例えば、連絡先のページレイアウトを変更する場合、「連絡先」と表示されます。

1. 先ほど追加した「**リード**」ブロックをダブルクリックします。

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. 高さを **450** ピクセルに編集し、「**OK**」をクリックします。

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!TIP]
   >
   >オブジェクトがアカウントと商談の場合、推奨値は 410 ピクセルです。

1. 左側の「**フィールド**」をクリックします。次に、 **緊急度** ラベルを **Marketo Sales Insight** レイアウト。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. 以下のフィールドについても、上記の手順を繰り返します。

   <table> 
    <tbody> 
     <tr> 
      <td>最新の注目のアクション</td> 
     </tr> 
     <tr> 
      <td>最新の注目のアクション発生日</td> 
     </tr> 
     <tr> 
      <td>最新の注目のアクションの詳細</td> 
     </tr> 
     <tr> 
      <td>最新の注目のアクションのソース</td> 
     </tr> 
     <tr> 
      <td>最新の注目のアクションのタイプ</td> 
     </tr> 
     <tr> 
      <td>セールスによる最後の Marketo アクティビティ</td> 
     </tr> 
     <tr> 
      <td>セールスによる最後の Marketo エンゲージメント</td> 
     </tr> 
     <tr> 
      <td>MSI 連絡先 ID</td> 
     </tr> 
     <tr> 
      <td>相対スコア</td> 
     </tr> 
     <tr> 
      <td>相対スコア値</td> 
     </tr> 
     <tr> 
      <td>緊急度</td> 
     </tr> 
     <tr> 
      <td>緊急度の値</td> 
     </tr> 
     <tr> 
      <td>Marketo 内に表示  </td> 
     </tr> 
    </tbody> 
   </table>

1. 終了したら「**保存**」をクリックします。

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. 手順 5～7 を繰り返して、次の用の Visualforce ページセクションと Sales Insight フィールドを追加します。 **連絡先**, **アカウント** および **商談**.

1. 手順 8 ～ 10 を繰り返して、以下のリストから Sales Insight フィールドを追加し、 **連絡先**. 必ず変更を保存してください。

<table> 
    <tbody> 
     <tr> 
      <td>最新の注目のアクション</td> 
     </tr> 
     <tr> 
      <td>最新の注目のアクション発生日</td> 
     </tr> 
     <tr> 
      <td>最新の注目のアクションの詳細</td> 
     </tr> 
     <tr> 
      <td>最新の注目のアクションのソース</td> 
     </tr> 
     <tr> 
      <td>最新の注目のアクションのタイプ</td> 
     </tr> 
     <tr> 
      <td>セールスによる最後の Marketo アクティビティ</td> 
     </tr> 
     <tr> 
      <td>セールスによる最後の Marketo エンゲージメント</td> 
     </tr> 
     <tr> 
      <td>MKTO リードスコア</td> 
     </tr> 
     <tr> 
      <td>相対スコア</td> 
     </tr> 
     <tr> 
      <td>相対スコア値</td> 
     </tr> 
     <tr> 
      <td>Sales Insight - 取引先責任者の完全なリストページを開きます</td> 
     </tr> 
     <tr> 
      <td>緊急度</td> 
     </tr> 
     <tr> 
      <td>緊急度の値</td> 
     </tr> 
    </tbody> 
   </table>

## カスタムユーザーフィールドのマッピング {#map-custom-person-fields}

コンバージョンの際にデータが失われないように、Marketo の「リード」フィールドを Salesforce の「連絡先」フィールドにマッピングする必要があります。手順は以下のとおりです。

1. 「**設定**」をクリックします。

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 検索バーで「フィールド」を検索し、「**リード**」の下の「**フィールド**」をクリックします。

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. 「**リードフィールドをマッピング**」をクリックします。

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. 右側のドロップダウンをクリックし、「**エンゲージメント**」を選択します。

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. リストから「**連絡先、エンゲージメント**」を選択します。

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. 上の手順を繰り返して、以下のフィールドもマッピングします。

   <table> 
    <tbody> 
     <tr> 
      <th colspan="1" rowspan="1">Marketo のリードのカスタムフィールド</th> 
      <th colspan="1" rowspan="1">Salesforce の連絡先のカスタムフィールド</th> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>エンゲージメント</p></td> 
      <td colspan="1" rowspan="1"><p>連絡先、エンゲージメント</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>相対スコア値</p></td> 
      <td colspan="1" rowspan="1"><p>連絡先、相対スコア値</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>緊急度の値</p></td> 
      <td colspan="1" rowspan="1"><p>連絡先、緊急度の値</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>最新の注目のアクション発生日</p></td> 
      <td colspan="1" rowspan="1"><p>連絡先、最新の注目のアクション発生日</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>最新の注目のアクションの詳細</p></td> 
      <td colspan="1" rowspan="1"><p>連絡先、最新の注目のアクションの詳細</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>最新の注目のアクションのソース</p></td> 
      <td colspan="1" rowspan="1"><p>連絡先、最新の注目のアクションのソース</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>最新の注目のアクションのタイプ</p></td> 
      <td colspan="1" rowspan="1"><p>連絡先、最新の注目のアクションのタイプ</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 完了したら、「**保存**」をクリックします。

## Marketo Sales Insight の設定 {#marketo-sales-insight-config}

1. 「**+**」をクリックし、「**Marketo Sales Insight の設定**」を選択します。

   ![](assets/image2014-9-24-17-3a37-3a45.png)

1. 「**Marketo API** を有効にする」をオンにします。次に、[Marketo Admin の API 設定情報](#set-up-marketo-sales-insight)を入力します。完了したら、「**変更を保存**」をクリックします。

   ![](assets/image2014-9-24-17-3a38-3a0.png)

   >[!NOTE]
   >
   >診断テストに失敗した場合は、[ページレイアウトにフィールドを追加](https://nation.marketo.com/docs/DOC-1115)する必要が生じる場合があります。

これで完了です。Marketo Sales Insight セクションで、リード、連絡先、アカウント、商談の詳細を確認できます。

![](assets/twenty-six.png)

>[!NOTE]
>
>アカウントの場合、Sales Insight にはすべての電子メールが含まれますが、最新の注目のアクション、web アクティビティ、スコアの変更のみが含まれます。

## Marketo Sales Insight へのアクセス {#access-marketo-sales-insight}

1. Salesforce で、タブバーの最後にある「**+**」をクリックし、「**Marketo Sales Insight の設定**」をクリックします。

1. 「**Marketo API を有効にする**」チェックボックスをオンにします。

1. Marketo の Sales Insight 管理ページの Soap API パネルから認証情報をコピーし、Salesforce Sales Insight の設定ページの Soap API セクションに貼り付けます。

1. Marketo の Sales Insight 管理ページの Rest API パネルから認証情報をコピーし、Salesforce Sales Insight の設定ページの Rest API セクションに貼り付けます。

   ![](assets/access-msi.png)

>[!MORELIKETHIS]
>
>* [優先度、緊急度、相対スコア、最有望見込客](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Salesforce への「Marketo」タブの追加](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [チーム向け Sales Insight の設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/setting-up-sales-insight-for-your-team.md)

