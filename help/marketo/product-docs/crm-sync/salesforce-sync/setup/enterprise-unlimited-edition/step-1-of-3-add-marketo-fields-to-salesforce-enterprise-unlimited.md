---
unique-page-id: 2360362
description: 手順 1／3 - Marketo フィールドの Salesforce への追加（Enterprise／Unlimited）- Marketo ドキュメント - 製品ドキュメント
title: 手順 1／3 - Marketo フィールドの Salesforce への追加（Enterprise／Unlimited）
exl-id: bcfba281-0d4b-42c3-b52a-ce1c3da884ba
feature: Salesforce Integration
source-git-commit: 989804463f44afbf35ab11c0f23c37b0d328e652
workflow-type: tm+mt
source-wordcount: '766'
ht-degree: 92%

---

# 手順 1／3：Marketo フィールドの Salesforce への追加（Enterprise／Unlimited） {#step-of-add-marketo-fields-to-salesforce-enterprise-unlimited}

>[!PREREQUISITES]
>
>Marketo EngageとSalesforceを同期するには、Salesforce API にアクセスできる必要があります。

Marketo は、一連のフィールドを使用して、特定の種類のマーケティング関連情報を取り込みます。Salesforce でこのデータを使用する場合は、以下の手順に従ってください。

1. Salesforce でリードと連絡先オブジェクトの 3 つのカスタムフィールド（スコア、獲得プログラム、獲得日）を作成します。
1. これらのカスタムフィールドをリードと連絡先の間にマッピングし、Salesforce でのコンバージョン時に値が持ち越されるようにします。
1. 必要に応じて、その他のフィールドを作成できます（以下の表を参照）。

これらのカスタムフィールドはすべてオプションで、Marketo と Salesforce を同期するのに必須ではありません。ベストプラクティスとして、「スコア」、「獲得プログラム」、「獲得日」のフィールドを作成することをお勧めします。

## Marketo フィールドを Salesforce に追加 {#add-marketo-fields-to-salesforce}

上記の Salesforce 内のリードおよび連絡先オブジェクトに 3 つのカスタムフィールドを追加します。さらに追加する場合は、この節の最後にある使用可能フィールドのテーブルを参照してください。

3 つのカスタムフィールドのそれぞれに対して、次の手順を実行して追加します。「スコア」から始めます。

1. Salesforce にログインし、「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/image2016-5-23-13-3a15-3a21.png)

1. 左側の [!UICONTROL  ビルド ] メニューで **[!UICONTROL カスタマイズ]** をクリックし、**[!UICONTROL リード]** を選択します。 「**[!UICONTROL フィールド]**」をクリックします。

   ![](assets/image2016-5-23-13-3a20-3a5.png)

1. ページ下部のカスタムフィールドと関係セクションで「**[!UICONTROL 新規]**」をクリックします。

   ![](assets/image2016-5-26-14-3a41-3a40.png)

1. 適切なフィールドタイプを選択します（スコア – 数値、獲得プログラム – テキスト、獲得日 – 日時の場合）。

   ![](assets/choose-field-type-2-hand.png)

1. 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2016-5-26-14-3a51-3a14.png)

1. 次の表に示すように、フィールドに [!UICONTROL  フィールドラベル ]、[!UICONTROL  長さ ]、[!UICONTROL  フィールド名 ] を入力します。

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
   <td>長さ 10 <br>小数点以下桁数 0 </td> 
  </tr> 
  <tr> 
   <td>取得日</td> 
   <td>mkto71_Acquisition_Date</td> 
   <td>日時</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>新規顧客獲得プログラム</td> 
   <td>mkto71_Acquisition_Program</td> 
   <td>テキスト</td> 
   <td>長さ 255</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Salesforce では、フィールド名を使用して API 名を作成するときに、フィールド名に __c を追加します。

![](assets/image2016-5-26-14-3a55-3a33.png)

>[!NOTE]
>
>テキストフィールドと数値フィールドには長さが必要ですが、日付/時間フィールドには必要ありません。説明はオプションです。

1. 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2016-5-23-14-3a50-3a5.png)

1. アクセス設定を指定し、「**[!UICONTROL 次へ]**」をクリックします。

   * すべての役割を&#x200B;**[!UICONTROL 表示]**&#x200B;および&#x200B;**[!UICONTROL 読み取り専用]**&#x200B;に設定します。

   * 同期ユーザーのプロファイルの&#x200B;**[!UICONTROL 読み取り専用]**&#x200B;のチェックをオフにします。

      * 同期ユーザーとして&#x200B;_システム管理者_&#x200B;のプロファイルを持つユーザーがいる場合は、システム管理者プロファイルの&#x200B;**[!UICONTROL 読み取り専用]**&#x200B;のチェックをオフにします（以下を参照）。
      * 同期ユーザーに&#x200B;_カスタムプロファイル_&#x200B;を作成した場合は、のカスタムプロファイルの&#x200B;**[!UICONTROL 読み取り専用]**&#x200B;のチェックをオフにします。

   ![](assets/image2016-6-30-9-3a25-3a4.png)

1. フィールドを表示するページレイアウトを選択します。

   ![](assets/image2016-5-26-15-3a14-3a45.png)

1. 「**[!UICONTROL 保存して新規作成]**」をクリックして戻り、他の 2 つのカスタムフィールドのそれぞれを作成します。3 つとも完成したら、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2016-5-23-15-3a8-3a43.png)

1. 左側のビルドメニューで、「**[!UICONTROL カスタマイズ]**」をクリックして「連絡先」を選択します。「フィールド」をクリックします。
1. リードオブジェクトと同様に、連絡先オブジェクトの「スコア」、「獲得日」、「獲得プログラム」フィールドについて手順 3 ～ 10 を実行します。
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
   <td>新規顧客獲得プログラム ID</td> 
   <td>mkto71_Acquisition_Program_Id</td> 
   <td>数字</td> 
   <td>長さ 18 <br>小数点以下桁数 0 </td> 
  </tr> 
  <tr> 
   <td>訪問者の参照元</td> 
   <td>mkto71_Original_Referrer</td> 
   <td>テキスト</td> 
   <td>長さ 255</td> 
  </tr> 
  <tr> 
   <td>参照元検索エンジン</td> 
   <td>mkto71_Original_Search_Engine</td> 
   <td>テキスト</td> 
   <td>長さ 255</td> 
  </tr> 
  <tr> 
   <td>参照元検索フレーズ</td> 
   <td>mkto71_Original_Search_Phrase</td> 
   <td>テキスト</td> 
   <td>長さ 255</td> 
  </tr> 
  <tr> 
   <td>参照元のソース情報</td> 
   <td>mkto71_Original_Source_Info</td> 
   <td>テキスト</td> 
   <td>長さ 255</td> 
  </tr> 
  <tr> 
   <td>参照元のソースのタイプ</td> 
   <td>mkto71_Original_Source_Type</td> 
   <td>テキスト</td> 
   <td>長さ 255</td> 
  </tr> 
  <tr> 
   <td>推測される市区町村</td> 
   <td>mkto71_Inferred_City</td> 
   <td>テキスト</td> 
   <td>長さ 255</td> 
  </tr> 
  <tr> 
   <td>推測される企業</td> 
   <td>mkto71_Inferred_Company</td> 
   <td>テキスト</td> 
   <td>長さ 255</td> 
  </tr> 
  <tr> 
   <td>推測される国</td> 
   <td>mkto71_Inferred_Country</td> 
   <td>テキスト</td> 
   <td>長さ 255</td> 
  </tr> 
  <tr> 
   <td>推測される都市圏</td> 
   <td>mkto71_Inferred_Metropolitan_Area</td> 
   <td>テキスト</td> 
   <td>長さ 255</td> 
  </tr> 
  <tr> 
   <td>推測される市外局番</td> 
   <td>mkto71_Inferred_Phone_Area_Code</td> 
   <td>テキスト</td> 
   <td>長さ 255</td> 
  </tr> 
  <tr> 
   <td>推測される郵便番号</td> 
   <td>mkto71_Inferred_Postal_Code</td> 
   <td>テキスト</td> 
   <td>長さ 255</td> 
  </tr> 
  <tr> 
   <td>推測される都道府県／地域</td> 
   <td>mkto71_Inferred_State_Region</td> 
   <td>テキスト</td> 
   <td>長さ 255</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Marketo によって自動的に割り当てられたフィールドの値は、新しいフィールドが作成されたときに Salesforce ですぐに使用できるわけではありません。Marketo は、次のアップデート時にいずれかのシステム上のレコードに対して Salesforce とデータを同期します（つまり、Marketo と Salesforce の間で同期されているフィールドのアップデート）。

## コンバージョン用のカスタムフィールドのマッピング {#map-custom-fields-for-conversions}

コンバージョンが発生した際にデータが引き継がれるように、Salesforce 内のリードオブジェクトのカスタムフィールドを連絡先オブジェクトの連絡先フィールドにマッピングする必要があります。

1. 右上隅にある「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/image2016-5-26-16-3a34-3a0.png)

1. ナビゲーション検索で「フィールド」と入力します。Enter は押しません。フィールドは色々なオブジェクトの下に表示されます。リードの下の「**[!UICONTROL フィールド]**」をクリックします。

   ![](assets/image2016-5-26-16-3a36-3a32.png)

1. リードのカスタムフィールドと関係セクションに移動し、「**[!UICONTROL リードフィールドをマッピングする]**」をクリックします。

   ![](assets/image2016-5-26-16-3a39-3a29.png)

1. マッピングするフィールドの横にあるドロップダウンをクリックします。

   ![](assets/image2016-5-26-16-3a49-3a53.png)

1. 対応する連絡先カスタムフィールドを選択します。

   ![](assets/image2016-5-26-16-3a56-3a23.png)

1. 作成した他のフィールドに対して、上記の手順を繰り返します。

1. 終了したら「**[!UICONTROL 保存]**」をクリックします。

>[!MORELIKETHIS]
>
>[手順 2 / 3：Marketo 用の Salesforce ユーザの作成（Enterprise／Unlimited）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}
