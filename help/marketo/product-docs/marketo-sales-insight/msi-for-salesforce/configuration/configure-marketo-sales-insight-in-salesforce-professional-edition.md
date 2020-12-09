---
unique-page-id: 3571743
description: Salesforce Professional Edition - Marketto Docs — 製品ドキュメントでのMarketo Sales Insightの設定
title: Salesforce Professional EditionでのMarketor Sales Insightの設定
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '920'
ht-degree: 0%

---


# Salesforce Professional EditionでのMarketor Sales Insightの設定 {#configure-marketo-sales-insight-in-salesforce-professional-edition}

Salesforce Professional EditionでMarketon Sales Insightを設定するために必要な手順を次に示します。 始めましょう。

>[!PREREQUISITES]
>
>[Salesforce Professional EditionにMarketoをインストールする](http://docs.marketo.com/display/docs/professional+edition)
>
>[SalesforceAppExchangeへのMarketo Sales Insightパッケージのインストール](../../../../product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**必要な管理者権限**

## MarketorでのSales Insightの設定 {#configure-sales-insight-in-marketo}

1. 新しいブラウザーウィンドウを開き、MarketoアカウントからMarketo Sales Insightの資格情報を取得します。
1. 「管理者」領域に移動し、「 **販売インサイト**」を選択します。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. 「 **API設定を編集**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. 選択したAPI秘密キーを入力し、「 **保存**」をクリックします。 API秘密鍵にはアンパサンド(&amp;)を使用しないでください。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >API秘密キーは、組織のパスワードのようなもので、セキュリティで保護する必要があります。

1. Rest API設定パネルで **表示** をクリックして、秘密鍵証明書を入力します。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. 確認ポップアップが表示されます。 「 **OK**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## SalesforceでのSales Insightの設定 {#configure-sales-insight-in-salesforce}

1. Salesforceで、「 **セットアップ**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. 「remote site」を検索し、「 **Remote Site Settings**」を選択します。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. [ **新規リモートサイト**]をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. リモートサイト名を入力します（「MarketoSoapAPI」など）。 MarketoのSoap API設定パネルから、MarketoホストURLである「リモートサイトURL」を入力します。 「 **保存**」をクリックします。 Soap APIのリモートサイト設定が作成されました。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. [ **新しいリモートサイト** ]を再度クリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. リモートサイト名を入力します（「MarketoRestAPI」など）。 リモートサイトURLを入力します。これは、MarketoのRest API設定パネルから取得したAPI URLです。 「 **保存**」をクリックします。 Rest APIのリモートサイト設定が作成されました。

## Marketor Sales Insightの設定 {#set-up-marketo-sales-insight}

1. Marketorインスタンスにログインし、「 **管理者**」をクリックします。

   ![](assets/login-admin-1.png)

1. 「** Sales Insight**」をクリックします。

   ![](assets/image2015-5-22-15-3a12-3a33-1.png)

1. 「 **API設定を編集**」をクリックします。

   ![](assets/image2015-5-22-15-3a15-3a0-1.png)

1. **API秘密キーを入力し** 、「 **保存**」をクリックします。

   >[!CAUTION]
   >
   >API秘密鍵にアンパサンド(&amp;)を使用しないでください。

   ![](assets/image2015-5-27-16-3a36-3a56-1.png)

   >[!TIP]
   >
   >この窓は開いたままにしておけ。 この情報は、後でSalesforceで必要になります。

1. Salesforceに戻り、「 **セットアップ**」をクリックします。

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. 「remote site」を検索し、「 **Security Controls** 」の「 **Remote Site Setting**」をクリックします。

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. [ **新規リモートサイト**]をクリックします。

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. 「 **リモートサイト名** 」と「 **リモートサイトURL**」を入力し、「 **保存**」をクリックします。

   ![](assets/remote-site-1.png)

   >[!NOTE]
   >
   >「 **リモートサイト名** 」を選択します（MarketoAPIはここで使用します）。 リ **モートサイトURLは** 、手順4のAPI設定を編集ダイアログボックスのMarketo Hostフィールドにあります。

## ページレイアウトのカスタマイズ {#customize-page-layouts}

1. 「 **設定**」をクリックします。

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. 「page layout」を検索し、「 **Leads** 」の下の「 **Page Layout**」を選択します。

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

1. 左側の「**Visualforceページ**」をクリックします。 「 **セクション** 」を「カスタムリンク」セクションの下のレイアウトにドラッグします。

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. 「 **セクション名**」に「Marketto Sales Insight」と入力します。 「 **1-Column** 」を選択し、「 **OK**」をクリックします。

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. リー **ド** を新しいセクションにドラッグ&amp;ドロップします。

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >このボックスの名前は、オブジェクトの種類に応じて変わります。 例えば、連絡先のページレイアウトを変更する場合は、「連絡先」と表示されます。

1. 先ほど追加した **リード** ブロックを重複クリックします。

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. 高さを450 **ピクセルに編集し、** 「OK ****」をクリックします。

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!TIP]
   >
   >AccountsおよびOpportunitiesオブジェクトの高さは、410ピクセルにすることをお勧めします。

1. 左側の「**フィールド**」をクリックします。 次に、「 **Engagement** 」ラベルを検索し、 **Marketor Sales Insight** レイアウトにドラッグします。

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

1. これらのフィールドに対しても、上記の手順を繰り返します。

<table> 
 <tbody> 
  <tr> 
   <td colspan="1">関与</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>相対スコア値</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>緊急度の値</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最後の興味深い瞬間の日付</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最後の注目モーメントの説明</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最後の興味深い瞬間の源</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最後の興味深いモーメントのタイプ</p></td> 
  </tr> 
 </tbody> 
</table>

1. 終了したら、 **「保存** 」をクリックします。

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. この手順を繰り返して、 **Contact**、 **Account** 、 **OpportunityのVisualforceページセクションとSales Insightフィールドを追加します**。
1. 手順5 ～ 7を繰り返して、連絡先、アカウント、オポチュニティのVisualforceページセクションを追加します。 次に、手順8 ～ 10を繰り返して、 **ContactにSales Insightフィールドを追加します**。 変更があったら必ず保存してください。

## ユーザー設定のユーザーフィールドのマッピング {#map-custom-person-fields}

変換が正しく機能するように、Marketing担当者のフィールドをSalesforceの連絡先フィールドにマッピングする必要があります。 これが方法です。

1. 「 **設定**」をクリックします。

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. 検索バーで「フィールド」を検索し、「リード **」の下にある「** フィールド **」をクリックし**&#x200B;ます。

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. 「リードフィールドの **マップ**」をクリックします。

   ** ![](assets/image2015-6-1-9-3a58-3a48-1.png)

   **

1. 右側のドロップダウンをクリックして、「 **エンゲージメント**」を選択します。

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. リストで「**Contact.Engagement **」を選択します。

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

1. これらのフィールドも同様に繰り返してマッピングします。

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1">マーケティング担当者のカスタムフィールド</th> 
   <th colspan="1" rowspan="1">Salesforce連絡先カスタムフィールド</th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>関与</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Engagement</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>相対スコア値</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Relative Score Value</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>緊急度の値</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Ergency値</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最後の興味深い瞬間の日付</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Intersion Moment Date</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最後の注目モーメントの説明</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Intersion Moment Desc</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最後の興味深い瞬間の源</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Oftirution Moment Source</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最後の興味深いモーメントのタイプ</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Ofterist Moment Type</p></td> 
  </tr> 
 </tbody> 
</table>

1. 終了したら「**保存**」をクリックします。

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Marketto Sales Insightの設定 {#marketo-sales-insight-config}

1. 「**+ **」をクリックし、「 **Marketto Sales Insight Config**」を選択します。

   ![](assets/image2014-9-24-17-3a37-3a45.png)

1. 「Marketto APIを **有効にする**」を選択します。 次に、Markettor管理者の [API設定情報を入力します](http://docs.marketo.com/display/DOCS/Configure+Marketo+Sales+Insight+in+Salesforce+Professional+Edition#ConfigureMarketoSalesInsightinSalesforceProfessionalEdition-SetupMarketoSalesInsight)。 終了したら「**変更を保存**」をクリックします。

   ![](assets/image2014-9-24-17-3a38-3a0.png)

   >[!NOTE]
   >
   >診断テストが失敗した場合は、ページレイアウトにフィールドを [追加する必要がある場合があります](http://nation.marketo.com/docs/DOC-1115)。

それだ！ リード、連絡先、アカウント、オポチュニティの「Marketo Sales Insight」フィールドを表示できるはずです。

![](assets/twenty-six-1.png)

>[!NOTE]
>
>アカウントの場合、Sales Insightにはすべての電子メールが含まれますが、最新の興味深い瞬間、Webアクティビティ、スコアの変更のみが含まれます。

## マーケティングに対する販売インサイトへのアクセス {#access-marketo-sales-insight}

1. Salesforceで、タブバーの最後にある **+をクリック** し、「 **Marketor Sales Insight Config**」をクリックします。
1. 「Marketto APIを **有効にする** 」チェックボックスを選択します。
1. MarketorのSales Insight管理者ページのSoap APIパネルから秘密鍵証明書をコピーし、Salesforce Sales Insight ConfigurationページのSoap APIセクションに貼り付けます。
1. MarketorのSales Insight管理者ページのRest APIパネルから秘密鍵証明書をコピーし、Salesforce Sales Insight ConfigurationページのRest APIセクションに貼り付けます。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

>[!NOTE]
>
>**関連記事**
>
>* [優先度、緊急度、相対スコア、ベストベット](../../../../product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Marketor追加の「Sales Insight」タブとSalesforce用のボタン](../../../../product-docs/marketo-sales-insight/msi-for-salesforce/features/bulk-actions/add-marketo-sales-insight-tab-and-buttons-to-salesforce.md)

>



hh