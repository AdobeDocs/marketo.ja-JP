---
unique-page-id: 2360362
description: 手順1/3 - Salesforce追加に対するMarketoフィールド(Enterprise/Unlimited) - Markettoドキュメント — 製品ドキュメント
title: 手順1/3 - Salesforceに対する追加Marketoフィールド(Enterprise/Unlimited)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---


# 手順1/3:Salesforce追加に対するMarketoフィールド(Enterprise/Unlimited) {#step-of-add-marketo-fields-to-salesforce-enterprise-unlimited}

>[!PREREQUISITES]
>
>MarketoとSalesforceを同期するには、Salesforce APIにアクセスできる必要があります。

Marketorは一連のフィールドを使用して、特定の種類のマーケティング関連情報を取り込みます。 Salesforceでこのデータを使用したい場合は、次の手順に従ってください。

1. リードおよび連絡先オブジェクトに対して、Salesforceで次の3つのカスタムフィールドを作成します。スコア、獲得プログラムおよび獲得日を参照してください。
1. Salesforceでのコンバージョン時に値が持ち越されるように、リードと連絡先の間にこれらのカスタムフィールドをマッピングします。
1. 必要に応じて、その他のフィールドも作成できます（下の表を参照）。

これらのカスタムフィールドはすべてオプションで、MarketoとSalesforceを同期する必要はありません。 ベストプラクティスとして、「スコア」、「獲得プログラム」および「獲得日」のフィールドを作成することをお勧めします。

## Salesforce追加に対するマーケティング先フィールド{#add-marketo-fields-to-salesforce}

上記のSalesforceのリードおよび連絡先オブジェクトに追加3つのカスタムフィールドがあります。 さらに追加する場合は、この節の最後にある使用可能なフィールドの表を参照してください。

3つのカスタムフィールドのそれぞれに対して次の手順を実行し、追加します。 スコア付き開始。

1. Salesforceにログインし、「Setup」をクリックします。

   ![](assets/image2016-5-23-13-3a15-3a21.png)

1. 左側のビルドメニューで、「Customize」をクリックし、「Leads」を選択します。 「フィールド」をクリックします。

   ![](assets/image2016-5-23-13-3a20-3a5.png)

1. ページの下部にある「カスタムフィールドとリレーションシップ」セクションで「新規」をクリックします。

   ![](assets/image2016-5-26-14-3a41-3a40.png)

1. 適切なフィールドタイプを選択します(スコアの場合は数値、獲得プログラム — テキスト；獲得日 — 日付/時刻)。

   ![](assets/choose-field-type-2-hand.png)

1. 「次へ」をクリックします。

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
   <td>数値</td> 
   <td>長さ10<br>小数点以下0桁 </td> 
  </tr> 
  <tr> 
   <td>獲得日</td> 
   <td>mkto71_Acquisition_Date</td> 
   <td>日付/時刻</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>獲得プログラム</td> 
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

1. 「次へ」をクリックします。

   ![](assets/image2016-5-23-14-3a50-3a5.png)

1. アクセス設定を指定し、「次へ」をクリックします。

   * すべてのロールを**表示**および&#x200B;**読み取り専用**&#x200B;に設定

   * 同期ユーザーのプロファイルの&#x200B;**読み取り専用**&#x200B;チェックボックスをオフにします。

      * *システム管理者*&#x200B;のプロファイルを同期ユーザーとして持つユーザーがいる場合は、「システム管理者」プロファイルの「**読み取り専用**」チェックボックスをオフにします（以下を参照）
      * 同期ユーザーに対して&#x200B;*カスタムプロファイル*&#x200B;を作成した場合は、そのカスタムプロファイルの&#x200B;**読み取り専用**&#x200B;チェックボックスをオフにします

   ![](assets/image2016-6-30-9-3a25-3a4.png)

1. フィールドを表示するページレイアウトを選択します。

   ![](assets/image2016-5-26-15-3a14-3a45.png)

1. 「保存して新規作成」をクリックすると、前のページに戻り、他の2つのカスタムフィールドをそれぞれ作成できます。 「保存」をクリックします。3つの操作はすべて完了です。

   ![](assets/image2016-5-23-15-3a8-3a43.png)

1. 左側の[ビルド]メニューで[カスタマイズ]をクリックし、[連絡先]を選択します。 「フィールド」をクリックします。
1. リードオブジェクトと同様に、連絡先オブジェクトの「スコア」、「獲得日」、「獲得プログラム」の各フィールドに対して手順3 ～ 10を実行します。
1. 必要に応じて、このテーブルの追加のカスタムフィールドに対して上記の手順を実行します。

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
   <td>獲得プログラムID</td> 
   <td>mkto71_Acquisition_プログラム_Id</td> 
   <td>数値</td> 
   <td>長さ18<br>小数点以下0桁 </td> 
  </tr> 
  <tr> 
   <td>元の転送者</td> 
   <td>mkto71_Original_転送者</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>オリジナル検索エンジン</td> 
   <td>mkto71_Original_Search_Engine</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>オリジナルの検索フレーズ</td> 
   <td>mkto71_Original_Search_Phrase</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>元のソース情報</td> 
   <td>mkto71_Original_Source_Info</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>元のソースの種類</td> 
   <td>mkto71_Original_Source_Type</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>推定都市</td> 
   <td>mkto71_Inferred_City</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>推定会社</td> 
   <td>mkto71_Inferred_会社</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>推定国</td> 
   <td>mkto71_Inferred_Country</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>推定都市圏</td> 
   <td>mkto71_Inferred_Metropolitan_Area</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>推定電話番号市外局番</td> 
   <td>mkto71_Inferred_Phone_Area_Code</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>推定郵便番号</td> 
   <td>mkto71_Inferred_Postal_Code</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
  <tr> 
   <td>推定状態領域</td> 
   <td>mkto71_Inferred_State_Region</td> 
   <td>テキスト</td> 
   <td>長さ255</td> 
  </tr> 
 </tbody> 
</table>

## 変換用のカスタムフィールドのマッピング{#map-custom-fields-for-conversions}

Salesforceのリードオブジェクトのカスタムフィールドは、コンバージョンの発生時にデータが持ち越されるように、コンタクトオブジェクトのコンタクトフィールドにマップする必要があります。

1. 右上隅の「**セットアップ**」をクリックします。

   ![](assets/image2016-5-26-16-3a34-3a0.png)

1. ナビゲーション検索でEnterキーを押さずに「Fields」と入力します。 フィールドは別のオブジェクトの下に表示されます。「Leads」の下の「**Fields**」をクリックします。

   ![](assets/image2016-5-26-16-3a36-3a32.png)

1. 「Lead Custom Fields &amp; Relationships」セクションに移動し、「**Map Lead Fields**」をクリックします。

   ![](assets/image2016-5-26-16-3a39-3a29.png)

1. マッピングするフィールドの横にあるドロップダウンをクリックします。

   ![](assets/image2016-5-26-16-3a49-3a53.png)

1. 対応する連絡先カスタムフィールドを選択します。

   ![](assets/image2016-5-26-16-3a56-3a23.png)

1. 作成した他のフィールドに対して、上記の手順を繰り返します。
1. 終了したら「**保存**」をクリックします。

   簡単だろ？

>[!NOTE]
>
>**ディープダイブ**
>
>これは[全ての手順のビデオ](https://nation.marketo.com/videos/1475)へのリンクです。

>[!NOTE]
>
>**関連記事**
>
>* [手順2/3:Marketor向けSalesforceユーザーの作成(Enterprise/Unlimited)](step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)

>



