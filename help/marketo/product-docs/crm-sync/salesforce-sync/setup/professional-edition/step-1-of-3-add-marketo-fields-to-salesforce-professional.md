---
unique-page-id: 11372975
description: 手順 1／3 - Marketo フィールドの Salesforce への追加（Professional）- Marketo ドキュメント - 製品ドキュメント
title: 手順 1／3 - Marketo フィールドの Salesforce への追加（Professional）
exl-id: 1b52825e-201d-4b55-8edf-444b1653d591
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 70%

---

# 手順 1/3:[!DNL Salesforce] へのMarketo フィールドの追加（Professional） {#step-of-add-marketo-fields-to-salesforce-professional}

>[!PREREQUISITES]
>
>Marketo EngageとSalesforceの間でデータを同期するには、Salesforce インスタンスがSalesforce API にアクセスできる必要があります。

Marketo は、一連のフィールドを使用して、特定の種類のマーケティング関連情報を取り込みます。このデータを [!DNL Salesforce] に取り込む場合は、以下の手順に従ってください。

1. リードおよび連絡先オブジェクトに、スコア、獲得プログラム、獲得日の 3 つのカスタムフィールドを [!DNL Salesforce] に作成します。
1. これらのカスタムフィールドをリードと連絡先の間でマッピングし、コンバージョン時に [!DNL Salesforce] の値が引き継がれるようにします。
1. 必要に応じて、その他のフィールドを作成できます（以下の表を参照）。

これらのカスタムフィールドはすべてオプションであり、Marketoと [!DNL Salesforce] を同期するために必要なものではありません。 ベストプラクティスとして、「スコア」、「獲得プログラム」、「獲得日」のフィールドを作成することをお勧めします。

## [!DNL Salesforce] へのMarketo フィールドの追加 {#add-marketo-fields-to-salesforce}

上記のリストのリードオブジェクトおよび連絡先オブジェクトに 3 つのカスタムフィールド [!DNL Salesforce] 追加します。 さらに追加する場合は、この節の最後にある使用可能フィールドのテーブルを参照してください。

3 つのカスタムフィールドのそれぞれに対して、次の手順を実行して追加します。「**[!UICONTROL スコア]**」から始めます。

1. Salesforceにログインし、「設定 **[!UICONTROL をクリックし]** す。

   ![](assets/image2016-5-23-13-3a15-3a21.png)

1. 左側のビルドメニューで、「**[!UICONTROL カスタマイズ]**」をクリックし、「**[!UICONTROL リード]**」を選択します。「**[!UICONTROL フィールド]**」をクリックします。

   ![](assets/image2016-5-23-13-3a20-3a5.png)

1. ページ下部のカスタムフィールドと関係セクションで「**[!UICONTROL 新規]**」をクリックします。

   ![](assets/image2016-5-26-14-3a41-3a40.png)

1. 適切なフィールドタイプを選択します（スコア - **[!UICONTROL 数値]**、獲得プログラム - **[!UICONTROL テキスト]**、獲得日 – **日付/時刻**）。

   ![](assets/choose-field-type-2-hand.png)

1. 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2016-5-26-14-3a51-3a14.png)

1. 次の表に示すように、フィールドの「[!UICONTROL フィールドラベル]」、「[!UICONTROL 長さ]」、「[!UICONTROL フィールド名]」を入力します。

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
>[!DNL Salesforce] は、API 名の作成にフィールド名を使用する場合、フィールド名に__c を追加します。

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

1. 左側のビルドメニューで、「**[!UICONTROL カスタマイズ]**」をクリックし、「**[!UICONTROL 連絡先]**」を選択します。「**[!UICONTROL フィールド]**」をクリックします。
1. リードオブジェクトと同様に、連絡先オブジェクトの「スコア」、「獲得日」、「獲得プログラム」フィールドについて手順 3 ～ 10 を実行します。
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
>Marketoによって自動的に割り当てられたフィールドの値は、新しいフィールドを作成したときに [!DNL Salesforce] で直ちに使用できなくなります。 Marketoは、次回いずれかのシステムのレコードに対する更新（つまり、Marketoと [!DNL Salesforce] の間で同期されるいずれかのフィールドの更新）時に [!DNL Salesforce] ータと同期します。

## コンバージョン用のカスタムフィールドのマッピング  {#map-custom-fields-for-conversions}

[!DNL Salesforce] のリードオブジェクトのカスタムフィールドは、コンバージョンが発生したときにデータが引き継がれるように、コンタクトオブジェクトのコンタクトフィールドにマッピングする必要があります。

1. 右上隅にある「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/image2016-5-26-16-3a34-3a0.png)

1. Enter キーを押さずにナビゲーション検索に「[!UICONTROL fields]」と入力します。 フィールドは色々なオブジェクトの下に表示されます。リードの下の「**[!UICONTROL フィールド]**」をクリックします。

   ![](assets/image2016-5-26-16-3a36-3a32.png)

1. リードのカスタムフィールドと関係セクションに移動し、「**[!UICONTROL リードフィールドをマッピングする]**」をクリックします。

   ![](assets/image2016-5-26-16-3a39-3a29.png)

1. マッピングするフィールドの横にあるドロップダウンをクリックします。

   ![](assets/image2016-5-26-16-3a49-3a53.png)

1. 対応する連絡先カスタムフィールドを選択します。

   ![](assets/image2016-5-26-16-3a56-3a23.png)

1. 作成した他のフィールドに対して、上記の手順を繰り返します。
1. 完了したら、「**[!UICONTROL 保存]**」をクリックします。

簡単ですね。

>[!MORELIKETHIS]
>
>[手順 2／3：Marketo 用の Salesforce ユーザーの作成（Professional）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md){target="_blank"}
