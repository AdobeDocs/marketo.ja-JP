---
unique-page-id: 2360368
description: Salesforce Enterprise/Unlimited - Marketto Docs — 製品ドキュメントでのMarketo Sales Insightの設定
title: Salesforce Enterprise/UnlimitedでのMarketor Sales Insightの設定
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 0%

---


# Salesforce EnterpriseでのMarketor Sales Insightの設定/無制限{#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Salesforce Enterprise/Unlimited EditionでMarketon Sales Insightを設定するために必要な手順を以下に示します。 始めましょう。

>[!PREREQUISITES]
>
>* [Salesforce Enterprise/Unlimited EditionでMarketoフィールドの同期を設定](https://docs.marketo.com/pages/viewpage.action?pageid=2360372)
>* [SalesforceAppExchangeへのMarketo Sales Insightパッケージのインストール](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)


>[!NOTE]
>
>**必要な管理者権限**

## MarketorでのSales Insightの設定{#configure-sales-insight-in-marketo}

1. 新しいブラウザーウィンドウを開き、MarketoアカウントからMarketo Sales Insightの資格情報を取得します。

1. 「管理者」領域に移動し、「**販売インサイト**」を選択します。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. 「**API設定を編集**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. 選択したAPI秘密キーを入力し、「**保存**」をクリックします。 API秘密鍵にはアンパサンド(&amp;)を使用しないでください。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >API秘密キーは、組織のパスワードのようなもので、セキュリティで保護する必要があります。

1. Rest API設定パネルで&#x200B;**表示**&#x200B;をクリックして、秘密鍵証明書を入力します。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. 確認ポップアップが表示されます。 「**OK**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

## SalesforceでのSales Insightの設定{#configure-sales-insight-in-salesforce}

1. Salesforceで、**セットアップ**&#x200B;をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. 「remote site」を検索し、「**Remote Site Settings**」を選択します。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. [**新しいリモートサイト**]をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. リモートサイト名を入力します（「MarketoSoapAPI」など）。 MarketoのSoap API設定パネルから、MarketoホストURLである「リモートサイトURL」を入力します。 「**保存**」をクリックします。 Soap APIのリモートサイト設定が作成されました。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. 「**新しいリモートサイト**」を再度クリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. リモートサイト名を入力します（「MarketoRestAPI」など）。 リモートサイトURLを入力します。これは、MarketoのRest API設定パネルから取得したAPI URLです。 「**保存**」をクリックします。 Rest APIのリモートサイト設定が作成されました。

## Marketor Sales Insightの設定{#set-up-marketo-sales-insight}

1. Marketoインスタンスにログインし、**管理者**&#x200B;をクリックします。

   ![](assets/login-admin.png)

1. 「**Sales Insight**」をクリックします。

   ![](assets/image2015-5-22-15-3a12-3a33.png)

1. 「**API設定を編集**」をクリックします。

   ![](assets/image2015-5-22-15-3a15-3a0.png)

1. **API秘密キー**&#x200B;を入力し、**保存**&#x200B;をクリックします。

   >[!CAUTION]
   >
   >API秘密鍵にアンパサンド(&amp;)を使用しないでください。

   ![](assets/image2015-5-27-16-3a36-3a56.png)

   >[!TIP]
   >
   >この窓は開いたままにしておけ。 この情報は、後でSalesforceで必要になります。

1. Salesforceに戻り、**セットアップ**&#x200B;をクリックします。

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 「リモートサイト」を検索し、**セキュリティコントロール**&#x200B;の下の&#x200B;**リモートサイト設定**&#x200B;をクリックします。

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. [**新しいリモートサイト**]をクリックします。

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. **リモートサイト名**&#x200B;と&#x200B;**リモートサイトURL**&#x200B;を入力し、**保存**&#x200B;をクリックします。

   ![](assets/remote-site.png)

   >[!NOTE]
   >
   >**リモートサイト名**&#x200B;を選択します（MarketoAPIはここで使用します）。 **リモートサイトURL**&#x200B;は、手順4のAPI設定を編集ダイアログボックスの「Marketo Host」フィールドにあります。

## ページレイアウトのカスタマイズ{#customize-page-layouts}

1. 「**セットアップ**」をクリックします。

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 「ページレイアウト」を検索し、「**リード**」の下の「**ページレイアウト**」を選択します。

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. 左側の「**Visualforceページ**」をクリックします。 **セクション**&#x200B;を「カスタムリンク」セクションの下のレイアウトにドラッグします。

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. **セクション名**&#x200B;として「Marketo Sales Insight」と入力します。 「**1 — 列**」を選択し、「**OK**」をクリックします。

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. **リード**&#x200B;を新しいセクションにドラッグ&amp;ドロップします。

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >このボックスの名前は、オブジェクトの種類に応じて変わります。 例えば、連絡先のページレイアウトを変更する場合は、「連絡先」と表示されます。

1. 追加した&#x200B;**リード**&#x200B;ブロックを重複クリックします。

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. 高さを&#x200B;**450**&#x200B;ピクセルに編集し、**「OK**」をクリックします。

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!TIP]
   >
   >AccountsおよびOpportunitiesオブジェクトの高さは、410ピクセルにすることをお勧めします。

1. 左側の&#x200B;**フィールド**&#x200B;をクリックします。 次に、**エンゲージメント**&#x200B;ラベルを検索し、**マーケティング担当者向けSales Insight**&#x200B;レイアウトにドラッグします。

   ![](assets/image2015-5-22-16-3a32-3a46.png)

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

1. 終了したら「**保存**」をクリックします。

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. この手順を繰り返して、**連絡先**、**アカウント**、**商談**&#x200B;に対してVisualforceページセクションとSales Insightフィールドを追加します。

1. 手順5 ～ 7を繰り返して、連絡先、アカウント、オポチュニティのVisualforceページセクションを追加します。 次に、手順8 ～ 10を繰り返して、**連絡先**&#x200B;の「Sales Insight」フィールドを追加します。 変更があったら必ず保存してください。

## ユーザー設定フィールドのマッピング{#map-custom-person-fields}

変換が正しく機能するように、Marketing担当者のフィールドをSalesforceの連絡先フィールドにマッピングする必要があります。 これが方法です。

1. 「**セットアップ**」をクリックします。

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 検索バーで「フィールド」を検索し、「**リード**」の下の「**フィールド**」をクリックします。

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. 「**Map Lead Fields**」をクリックします。

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. 右側のドロップダウンをクリックして、**アクション**&#x200B;を開きます。

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. リストーで「**Contact.Engagement**」を選択します。

   ![](assets/image2015-6-1-10-3a12-3a11.png)

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

## Marketo Sales Insight Config {#marketo-sales-insight-config}

1. **+**&#x200B;をクリックし、**Marketto Sales Insight Config**&#x200B;を選択します。

   ![](assets/image2014-9-24-17-3a37-3a45.png)

1. **Marketo API**&#x200B;を有効にするをチェックします。 次に、Marketo Admin](#set-up-marketo-sales-insight)の[API設定情報を入力します。 完了したら、「**変更の保存**」をクリックします。

   ![](assets/image2014-9-24-17-3a38-3a0.png)

   >[!NOTE]
   >
   >診断テストが失敗した場合は、[ページレイアウト](https://nation.marketo.com/docs/DOC-1115)にフィールドを追加する必要がある場合があります。

それだ！ リード、連絡先、アカウント、オポチュニティの「Marketo Sales Insight」フィールドを表示できるはずです。

![](assets/twenty-six.png)

>[!NOTE]
>
>アカウントの場合、Sales Insightにはすべての電子メールが含まれますが、最新の興味深い瞬間、Webアクティビティ、スコアの変更のみが含まれます。

## Marketing to Sales Insight {#access-marketo-sales-insight}へのアクセス

1. Salesforceで、タブバーの末尾の&#x200B;**+**&#x200B;をクリックし、**Marketto Sales Insight Config**&#x200B;をクリックします。

1. 「Marketto API **を有効にする」チェックボックスを選択します。**

1. MarketorのSales Insight管理者ページのSoap APIパネルから秘密鍵証明書をコピーし、Salesforce Sales Insight ConfigurationページのSoap APIセクションに貼り付けます。

1. MarketorのSales Insight管理者ページのRest APIパネルから秘密鍵証明書をコピーし、Salesforce Sales Insight ConfigurationページのRest APIセクションに貼り付けます。

   ![](assets/access-msi.png)

>[!MORELIKETHIS]
>
>* [優先度、緊急度、相対スコア、ベストベット](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Marketor追加の「Sales Insight」タブとSalesforce用のボタン](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/bulk-actions/add-marketo-sales-insight-tab-and-buttons-to-salesforce.md)
>* [チーム向けのSales Insightの設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/setting-up-sales-insight-for-your-team.md)

