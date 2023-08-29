---
unique-page-id: 3571743
description: Salesforce Professional Edition での Marketo Sales Insight の設定 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce Professional Edition での Marketo Sales Insight の設定
exl-id: fae63560-0bb3-46a9-94a3-cc27c1aa363e
feature: Marketo Sales Insights
source-git-commit: c85f544f2c06a2f5bb92d6e7cad5f801e73fdaed
workflow-type: tm+mt
source-wordcount: '962'
ht-degree: 81%

---

# Salesforce Professional Edition での Marketo Sales Insight の設定 {#configure-marketo-sales-insight-in-salesforce-professional-edition}

Salesforce Professional Edition で Marketo Sales Insight を設定するために必要な手順を次に示します。それでは始めましょう。

>[!PREREQUISITES]
>
>* Salesforce Professional Edition に Marketo をインストールします。
>
>* [Salesforce AppExchange での Marketo Sales Insight パッケージのインストール](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}

>[!NOTE]
>
>**管理者権限が必要**

## Marketo での Sales Insight の設定 {#configure-sales-insight-in-marketo}

1. 新しいブラウザーウィンドウを開き、Marketo アカウントから Marketo Sales Insight の認証情報を取得します。
1. 管理者領域に移動し、「**Sales Insight**」を選択します。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. 「**API 設定を編集**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. 任意の API 秘密鍵を入力し、「**保存**」をクリックします。API 秘密鍵にアンパサンド（&amp;）を使用しないでください。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >API 秘密鍵は組織のパスワードと同じです。安全に保管してください。

1. Rest API 設定パネルの「**表示**」をクリックして、認証情報を設定します。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. 確認ポップアップが表示されます。「**OK**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## Salesforce での Sales Insight の設定 {#configure-sales-insight-in-salesforce}

1. Salesforce で、「**設定**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. 「リモートサイト」を検索し、「**リモートサイトの設定**」を選択します。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. 「**新規リモートサイト**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. リモートサイト名を入力します（「MarketoSoapAPI」など）。 Marketo の Soap API 設定パネルから、「リモートサイト URL」に「Marketo ホスト URL」と入力します。「**保存**」をクリックします。これで、Soap API 用のリモートサイト設定が作成されました。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. もう一度「**新規リモートサイト**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. リモートサイト名を入力します（「MarketoRestAPI」など）。 「リモートサイト URL」に、Marketo の Rest API 設定パネルの API URL を入力します。「**保存**」をクリックします。Rest API 用のリモートサイト設定が作成されました。

## Marketo Sales Insight の設定 {#set-up-marketo-sales-insight}

1. Marketo インスタンスにログインし、**管理**&#x200B;をクリックします。

   ![](assets/login-admin-1.png)

1. 「**Sales Insight**」をクリックします。

   ![](assets/image2015-5-22-15-3a12-3a33-1.png)

1. 「**API 設定を編集**」をクリックします。

   ![](assets/image2015-5-22-15-3a15-3a0-1.png)

1. **API 秘密鍵**&#x200B;を入力し、「**保存**」をクリックします。

   >[!CAUTION]
   >
   >API 秘密鍵にはアンパサンド（&amp;）を使用しないでください。

   ![](assets/image2015-5-27-16-3a36-3a56-1.png)

   >[!TIP]
   >
   >このウィンドウは開いたままにしておきます。この情報は、後で Salesforce で必要になります。

1. Salesforce に戻り、「**設定**」をクリックします。

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. 「リモートサイト」を検索し、「**セキュリティコントロール**」の下の「**リモートサイト設定**」をクリックします。

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. 「**新規リモートサイト**」をクリックします。

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. 「**リモートサイト名**」と「**リモートサイト URL**」を入力し、「**保存**」をクリックします。

   ![](assets/remote-site-1.png)

   >[!NOTE]
   >
   >「**リモートサイト名**」を選択します（MarketoAPI はここで使用されます）。「**リモートサイトの URL**」は、手順 4 の、API 設定を編集ダイアログボックスの「Marketo ホスト」フィールドにあります。

## Sales Insight ユーザーに標準 Salesforce オブジェクトへのプロファイルアクセスを許可する {#grant-sales-insight-users-profile-access}

Saleforce のセキュリティ強化により、App Exchange パッケージは標準オブジェクトに権限を付与できなくなり、Salesforce ユーザーのプロファイルから関連する Salesforce オブジェクトにアクセス権を付与する必要があります。 次の手順に従って、必要な権限を付与します。

1. 「**設定**」をクリックします。

1. クイック検索で「プロファイル」を検索します。

1. クリック **編集** Salesforce ユーザーが使用しているプロファイルの横に表示されます。

1. [ 標準オブジェクト権限 ] セクションで、リード、連絡先、アカウント、商談の各オブジェクトに対して読み取りアクセスを有効にします。

1. 「**保存**」をクリックします。

## ページレイアウトのカスタマイズ {#customize-page-layouts}

1. 「**設定**」をクリックします。

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. 「ページレイアウト」を検索し、「**リード**」の下の「**ページレイアウト**」を選択します。

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

1. 左側の「**Visualforce Pages**」をクリックします。「**セクション**」をカスタムリンクセクションの下のレイアウトにドラッグします。

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. 「**セクション名**」に「Marketo Sales Insight」と入力します。「**1 列**」を選択し、「**OK**」をクリックします。

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. 「**リード**」を新しいセクションにドラッグ＆ドロップします。

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >このボックスの名前は、オブジェクトの種類に基づいて変更されます。例えば、取引先責任者のページレイアウトを変更する場合、「取引先責任者」と表示されます。

1. 先ほど追加した「**リード**」ブロックをダブルクリックします。

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. 高さを **450** ピクセルに編集し、「**OK**」をクリックします。

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >スクロールを使用してアクティビティにアクセスする必要がある場合は、「**スクロールバーを表示**」をチェックします。

   >[!TIP]
   >
   >オブジェクトがアカウントと商談の場合、推奨値は 410 ピクセルです。

1. 左側の「**フィールド**」をクリックします。次に、「**エンゲージメント**」ラベルを検索して、**Marketo Sales Insight** レイアウトにドラッグします。

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

1. 以下のフィールドについても、上記の手順を繰り返します。

<table> 
 <tbody> 
  <tr> 
   <td colspan="1">エンゲージメント</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>相対スコア値</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>緊急度の値</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最新の注目のアクション発生日</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最新の注目のアクションの詳細</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最新の注目のアクションのソース</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最新の注目のアクションのタイプ</p></td> 
  </tr> 
 </tbody> 
</table>

1. 終了したら「**保存**」をクリックします。

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. この手順を繰り返して、**取引先責任者**、**アカウント**&#x200B;および&#x200B;**商談**&#x200B;の Visualforce ページセクションと Sales Insight フィールドを追加します。
1. 手順 5〜7 を繰り返して、取引先責任者、アカウント、商談のそれぞれについて Visualforce ページセクションを追加します。次に、手順 8〜10 を繰り返して、**取引先責任者**&#x200B;に Sales Insight のフィールドを追加します。変更したら必ず保存します。

## カスタムユーザフィールドのマッピング {#map-custom-person-fields}

コンバージョンの際にデータが失われないように、Marketo の人物フィールドを Salesforce の取引先責任者フィールドにマッピングする必要があります。手順は以下のとおりです。

1. 「**設定**」をクリックします。

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. 検索バーで「フィールド」を検索し、「**リード**」の下の「**フィールド**」をクリックします。

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. 「**リードフィールドをマッピング**」をクリックします。

   ![](assets/image2015-6-1-9-3a58-3a48-1.png)

1. 右側のドロップダウンをクリックし、「**エンゲージメント**」を選択します。

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. リストから「**取引先責任者、エンゲージメント**」を選択します。

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

1. 上の手順を繰り返して、以下のフィールドもマッピングします。

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1">Marketo の人物のカスタムフィールド</th> 
   <th colspan="1" rowspan="1">Salesforce の取引先責任者のカスタムフィールド</th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>エンゲージメント</p></td> 
   <td colspan="1" rowspan="1"><p>取引先責任者、エンゲージメント</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>相対スコア値</p></td> 
   <td colspan="1" rowspan="1"><p>取引先責任者、相対スコア値</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>緊急度の値</p></td> 
   <td colspan="1" rowspan="1"><p>取引先責任者、緊急度の値</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最新の注目のアクション発生日</p></td> 
   <td colspan="1" rowspan="1"><p>取引先責任者、最新の注目のアクション発生日</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最新の注目のアクションの詳細</p></td> 
   <td colspan="1" rowspan="1"><p>取引先責任者、最新の注目のアクションの詳細</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最新の注目のアクションのソース</p></td> 
   <td colspan="1" rowspan="1"><p>取引先責任者、最新の注目のアクションのソース</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最新の注目のアクションのタイプ</p></td> 
   <td colspan="1" rowspan="1"><p>取引先責任者、最新の注目のアクションのタイプ</p></td> 
  </tr> 
 </tbody> 
</table>

1. 完了したら、「**保存**」をクリックします。

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Marketo Sales Insight の「設定」タブ {#marketo-sales-insight-configuration-tab}

1. Salesforce で、タブバーの最後にある「**+**」をクリックし、「**Marketo Sales Insight の設定**」をクリックします。

1. の Soap API パネルから資格情報をコピーします。 [Marketo Sales Insight 管理ページ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} をクリックし、Salesforce Sales Insight 設定ページの「SOAP API」セクションに貼り付けます。

1. の Rest API パネルから資格情報をコピーします。 [Marketo Sales Insight 管理ページ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} をクリックし、Salesforce Sales Insight 設定ページの Rest API セクションに貼り付けます。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

これで完了です。Marketo Sales Insight フィールドで、リード、取引先責任者、アカウント、商談の詳細を確認できます。

>[!NOTE]
>
>診断テストに失敗した場合は、次の操作を行う必要があります。 [ページレイアウトにフィールドを追加する](https://nation.marketo.com/docs/DOC-1115){target="_blank"}.

>[!NOTE]
>
>アカウントの場合、Sales Insight にはすべての電子メールが含まれますが、最新の注目のアクション、web アクティビティ、スコアの変更のみが含まれます。

>[!MORELIKETHIS]
>
>* [優先度、緊急度、相対スコア、最有望見込客](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md){target="_blank"}
>* [Salesforce への「Marketo」タブの追加](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md){target="_blank"}
>* [Sales Insight へのアクセスをプロファイルに追加](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
