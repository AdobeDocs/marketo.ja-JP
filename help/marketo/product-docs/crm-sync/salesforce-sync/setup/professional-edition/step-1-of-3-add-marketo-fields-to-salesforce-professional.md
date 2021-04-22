---
unique-page-id: 11372975
description: 手順1/3 - Salesforce(Professional)追加へのMarketoフィールド —Marketoドキュメント — 製品ドキュメント
title: 手順1/3 - Salesforceに対する追加Marketoフィールド(Professional)
exl-id: 1b52825e-201d-4b55-8edf-444b1653d591
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 8%

---

# 手順1/3:Salesforce (Professional)追加へのMarketoフィールド{#step-of-add-marketo-fields-to-salesforce-professional}

>[!PREREQUISITES]
>
>MarketoとSalesforceの間でデータを同期するには、Salesforce APIにSalesforceインスタンスがアクセスできる必要があります。

Marketoは一連のフィールドを使用して、特定の種類のマーケティング関連情報を取り込みます。 Salesforceでこのデータを使用したい場合は、次の手順に従ってください。

1. リードおよび連絡先オブジェクトに対して、Salesforceで次の3つのカスタムフィールドを作成します。スコア、獲得プログラムおよび獲得日を参照してください。
1. Salesforceでのコンバージョン時に値が持ち越されるように、リードと連絡先の間にこれらのカスタムフィールドをマッピングします。
1. 必要に応じて、その他のフィールドも作成できます（下の表を参照）。

これらのカスタムフィールドはすべてオプションで、MarketoとSalesforceを同期する必要はありません。 ベストプラクティスとして、「スコア」、「獲得プログラム」および「獲得日」のフィールドを作成することをお勧めします。

## Salesforce追加へのMarketoフィールド{#add-marketo-fields-to-salesforce}

上記のSalesforceのリードおよび連絡先オブジェクトに追加3つのカスタムフィールドがあります。 さらに追加する場合は、この節の最後にある使用可能なフィールドの表を参照してください。

3つのカスタムフィールドのそれぞれに対して次の手順を実行し、追加します。 **スコア**&#x200B;との開始。

1. Salesforceにログインし、**セットアップをクリックします。**

   ![](assets/image2016-5-23-13-3a15-3a21.png)

1. 左側のBuildメニューで、「**Customize**」をクリックし、「**Leads**」を選択します。 「**フィールド**」をクリックします。

   ![](assets/image2016-5-23-13-3a20-3a5.png)

1. ページの下部にある「カスタムフィールドとリレーションシップ」セクションで、「**新規**」をクリックします。

   ![](assets/image2016-5-26-14-3a41-3a40.png)

1. 適切なフィールドタイプを選択します(スコアの場合 — **数値**;獲得プログラム— **text**;獲得日 — **日付/時刻**)。

   ![](assets/choose-field-type-2-hand.png)

1. 「**次へ**」をクリックします。

   ![](assets/image2016-5-26-14-3a51-3a14.png)

1. 次の表に示すように、フィールドのフィールドラベル、長さ、フィールド名を入力します。

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      フィールドラベル 
    </div></th> 
   <th> 
    <div>
      フィールド名 
    </div></th> 
   <th> 
    <div>
      データタイプ 
    </div></th> 
   <th> 
    <div>
      フィールド属性 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>スコア</td> 
   <td>mkto71_Lead_Score</td> 
   <td>数字</td> 
   <td>長さ10<br>小数点以下0桁 </td> 
  </tr> 
  <tr> 
   <td>取得日</td> 
   <td>mkto71_Acquisition_Date</td> 
   <td>日時</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>新規顧客獲得プログラム</td> 
   <td>mkto71_Acquisition_プログラム</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Salesforceは、フィールド名を使用してAPI名を作成する際に、フィールド名に__cを追加します。

![](assets/image2016-5-26-14-3a55-3a33.png)

>[!NOTE]
>
>テキストフィールドと数値フィールドには長さが必要ですが、日付/時間フィールドには必要ありません。説明はオプションです。

1. 「**次へ**」をクリックします。

   ![](assets/image2016-5-23-14-3a50-3a5.png)

1. アクセス設定を指定し、「**次へ**」をクリックします。

   * すべてのロールを&#x200B;**表示**&#x200B;と&#x200B;**読み取り専用**&#x200B;に設定

   * 同期ユーザーのプロファイルの&#x200B;**読み取り専用**&#x200B;チェックボックスをオフにします。

      * _システム管理者_&#x200B;のプロファイルを同期ユーザーとして持つユーザーがいる場合は、「システム管理者」プロファイルの「**読み取り専用**」チェックボックスをオフにします（以下を参照）

      * 同期ユーザーに対して&#x200B;_カスタムプロファイル_&#x200B;を作成した場合は、そのカスタムプロファイルの&#x200B;**読み取り専用**&#x200B;チェックボックスをオフにします

   ![](assets/image2016-6-30-9-3a25-3a4.png)

1. フィールドを表示するページレイアウトを選択します。

   ![](assets/image2016-5-26-15-3a14-3a45.png)

1. [**保存して新規作成**]をクリックすると、前のページに戻り、他の2つのカスタムフィールドがそれぞれ作成されます。 「**保存**」をクリックします。3つすべての作業は終了です。

   ![](assets/image2016-5-23-15-3a8-3a43.png)

1. 左側のビルドメニューで、「**カスタマイズ**」をクリックし、「**連絡先**」を選択します。 「**フィールド**」をクリックします。
1. リードオブジェクトと同様に、連絡先オブジェクトの「スコア」、「獲得日」、「獲得プログラム」の各フィールドに対して手順3 ～ 10を実行します。
1. 必要に応じて、このテーブルの追加のカスタムフィールドに対して上記の手順を実行します。

<table> 
 <tbody> 
  <tr> 
   <th>フィールドラベル</th> 
   <th>フィールド名</th> 
   <th>データタイプ</th> 
   <th>フィールド属性</th> 
  </tr> 
  <tr> 
   <td>獲得プログラムID</td> 
   <td>mkto71_Acquisition_プログラム_Id</td> 
   <td>数字</td> 
   <td>長さ18<br>小数点以下0桁 </td> 
  </tr> 
  <tr> 
   <td>訪問者の参照元</td> 
   <td>mkto71_Original_転送者</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>参照元検索エンジン</td> 
   <td>mkto71_Original_Search_Engine</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>参照元検索フレーズ</td> 
   <td>mkto71_Original_Search_Phrase</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>参照元のソース情報</td> 
   <td>mkto71_Original_Source_Info</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>参照元のソースのタイプ</td> 
   <td>mkto71_Original_Source_Type</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>推測される都市</td> 
   <td>mkto71_Inferred_City</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>推測される企業</td> 
   <td>mkto71_Inferred_会社</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>推測される国</td> 
   <td>mkto71_Inferred_Country</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>推測される都市圏</td> 
   <td>mkto71_Inferred_Metropolitan_Area</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>推測される市外局番</td> 
   <td>mkto71_Inferred_Phone_Area_Code</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>推測される郵便番号</td> 
   <td>mkto71_Inferred_Postal_Code</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>推測される都道府県/地域</td> 
   <td>mkto71_Inferred_State_Region</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
 </tbody> 
</table>

## 変換用のカスタムフィールドのマッピング{#map-custom-fields-for-conversions}

Salesforceのリードオブジェクトのカスタムフィールドは、コンバージョンの発生時にデータが持ち越されるように、コンタクトオブジェクトのコンタクトフィールドにマップする必要があります。

1. 右上隅の「設定」をクリックします。

   ![](assets/image2016-5-26-16-3a34-3a0.png)

1. ナビゲーション検索では、Enterキーを押さずに「fields」と入力します。 フィールドは別のオブジェクトの下に表示されます。「Leads」の下の「Fields」をクリックします。

   ![](assets/image2016-5-26-16-3a36-3a32.png)

1. 「リードのカスタムフィールドと関係」セクションに移動し、「リードフィールドのマッピング」をクリックします。

   ![](assets/image2016-5-26-16-3a39-3a29.png)

1. マッピングするフィールドの横にあるドロップダウンをクリックします。

   ![](assets/image2016-5-26-16-3a49-3a53.png)

1. 対応する連絡先カスタムフィールドを選択します。

   ![](assets/image2016-5-26-16-3a56-3a23.png)

1. 作成した他のフィールドに対して、上記の手順を繰り返します。
1. 終了したら「保存」をクリックします。

簡単だろ？

>[!NOTE]
>
>これは[プロセス全体のビデオ](https://nation.marketo.com/videos/1475)です。

>[!MORELIKETHIS]
>
>[手順2/3:Marketo(Professional)用Salesforceユーザーの作成](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)
