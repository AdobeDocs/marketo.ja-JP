---
description: 手順 1/3 - Marketo フィールドを CRM に追加  [!DNL Veeva]  Marketo ドキュメント – 製品ドキュメント
title: 手順 1/3 - Marketo フィールドを  [!DNL Veeva] CRM に追加
exl-id: a9a59e76-a7a4-4391-8169-922bd6acfb6d
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 46%

---

# 手順 1/3:CRM へのMarketo フィールド [!DNL Veeva] 追加 {#step-1-of-3-add-marketo-fields-to-veeva-crm}

>[!PREREQUISITES]
>
>[!DNL Veeva] CRM インスタンスがMarketo Engageと [!DNL Veeva] CRM の間でデータを同期するには、Salesforce API にアクセスできる必要があります。

Marketo Engage は、一連のフィールドを使用して、特定の種類のマーケティング関連情報を取り込みます。このデータを [!DNL Veeva] CRM に取り込む場合は、次の手順に従ってください。

連絡先オブジェクトの CRM`1.` カスタムフィールド [!DNL Veeva] 作成するには：スコア

`2.`必要に応じて、追加のフィールドを作成できます（以下の表を参照）。

これらのカスタムフィールドはすべてオプションであり、Marketo Engageと [!DNL Veeva] CRM を同期するために必要なものではありません。

## CRM へのMarketo フィールド [!DNL Veeva] 追加 {#add-marketo-fields-to-veeva-crm}

上記の CRM のリードおよび連絡先オブジェクトにカスタムフィールド [!DNL Veeva] 追加します。 さらに追加する場合は、この節の最後にある使用可能フィールドのテーブルを参照してください。

「スコア」フィールドに対して、次の手順を実行してフィールドを追加します。

1. [!DNL Veeva] CRM にログインし、「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/step-1-of-3-add-marketo-fields-1.png)

1. **[!UICONTROL オブジェクトとフィールド]** をクリックし、「**[!UICONTROL オブジェクトマネージャ]**」を選択します。

   ![](assets/step-1-of-3-add-marketo-fields-2.png)

1. 検索バーで「連絡先」を検索します。

   ![](assets/step-1-of-3-add-marketo-fields-3.png)

1. **[!UICONTROL 連絡先]** オブジェクトをクリックします。

1. **[!UICONTROL フィールドと関係]** を選択します。

1. 「**[!UICONTROL 新規]**」をクリックします。

   ![](assets/step-1-of-3-add-marketo-fields-4.png)

1. 適切なフィールドタイプ（スコア – 数値の場合）を選択します。

   ![](assets/step-1-of-3-add-marketo-fields-5.png)

1. 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/step-1-of-3-add-marketo-fields-6.png)

1. 次の表に示すように、フィールドの「**[!UICONTROL フィールドラベル]**」、「**[!UICONTROL 長さ]**」、「**[!UICONTROL フィールド名]**」を入力します。

<table>
 <tbody>
  <tr>
   <th>フィールドラベル
   <th>フィールド名
   <th>データタイプ
   <th>フィールド属性
  </tr>
  <tr>
   <td>スコア</td>
   <td>mkto71_Lead_Score</td>
   <td>数字</td>
   <td>長さ 10 <br/>小数点以下桁数 0</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>CRM[!DNL Veeva]API 名の作成にフィールド名を使用する場合は、フィールド名に__c を付加します。

![](assets/step-1-of-3-add-marketo-fields-7.png)

>[!NOTE]
>
>テキストフィールドと数値フィールドには長さが必要ですが、日付/時間フィールドには必要ありません。説明はオプションです。

1. 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/step-1-of-3-add-marketo-fields-8.png)

1. アクセス設定を指定し、「**[!UICONTROL 次へ]**」をクリックします。

1. すべての役割を **[!UICONTROL 表示]** および **[!UICONTROL 読み取り専用]** に設定します。

1. 同期ユーザーのプロファイルの&#x200B;**[!UICONTROL 読み取り専用]**&#x200B;のチェックをオフにします。

* システム管理者のプロファイルを同期ユーザーとして使用しているユーザーがいる場合は、そのシステム管理者プロファイルの [!UICONTROL  読み取り専用 ] チェックボックスをオフにします（下図を参照）。
* 同期ユーザーのカスタムプロファイルを作成した場合は、そのカスタムプロファイルの「[!UICONTROL  読み取り専用 ]」チェックボックスをオフにします。

  ![](assets/step-1-of-3-add-marketo-fields-9.png)

1. フィールドを表示するページレイアウトを選択します。

1. 「**[!UICONTROL 保存して新規作成]**」をクリックして戻り、他の 2 つのカスタムフィールドのそれぞれを作成します。

1. 3 つすべてが完了したら、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/step-1-of-3-add-marketo-fields-10.png)

>[!NOTE]
>
>フィールドを取引先責任者オブジェクトに追加することで、個人取引先オブジェクトにも追加されます。

オプション：このテーブルの追加のカスタムフィールドに対して上記の手順を実行します。

<table>
 <tbody>
  <tr>
   <th>フィールドラベル
   <th>フィールド名
   <th>データタイプ
   <th>フィールド属性
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
>新しいフィールドが作成されると、Marketoによって自動的に割り当てられたフィールドの値は [!DNL Veeva] CRM ですぐに使用できなくなります。 Marketoは、次の更新時に、いずれかのシステム上のレコードに対してデータを [!DNL Veeva] CRM と同期します（つまり、Marketoと [!DNL Veeva] CRM の間で同期されているフィールドのいずれかを更新します）。
