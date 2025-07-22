---
description: Sales Insight アクセスの削除 - Marketo ドキュメント - 製品ドキュメント
title: Sales Insight アクセスの削除
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 61%

---

# [!DNL Sales Insight] アクセスを削除 {#remove-sales-insight-access}

[!DNL Sales Insight] の [!DNL Salesforce] 機能へのアクセスを削除するには、次の手順を使用します。 [!DNL Salesforce] Classic および Lightning に適用できます。

## 概要 {#overview}

[!DNL Sales Insight] のすべての機能にアクセスするには、以下に説明するオブジェクト、apex クラスおよび visualforce ページへの権限が必要です。 これらを削除すると、[!DNL Sales Insight] へのアクセス権が削除されます。

**オブジェクト設定**

<table> 
 <tbody> 
 <tr> 
   <td>BestBetsCache</td> 
   <td>読み取り、作成、編集、削除、すべて表示、すべて変更</td> 
  </tr> 
  <tr> 
   <td>[!DNL Best Bets] 詳細を表示</td> 
   <td>読み取り、作成、編集、削除、すべて表示、すべて変更</td> 
  </tr> 
  <tr> 
   <td>[!DNL Best Bets] ビュー</td> 
   <td>読み取り、作成、編集、削除、すべて表示、すべて変更</td> 
  </tr> 
  <tr> 
   <td>EmailActivityCache</td> 
   <td>読み取り、作成、編集、削除、すべて表示、すべて変更</td> 
  </tr> 
  <tr> 
   <td>GetMethodArgus</td> 
   <td>読み取り、作成、編集、削除、すべて表示、すべて変更</td> 
  </tr> 
  <tr> 
   <td>GroupedWebActivityCache</td> 
   <td>読み取り、作成、編集、削除、すべて表示、すべて変更</td> 
  </tr> 
  <tr> 
   <td>InterestingMomentsCache</td> 
   <td>読み取り、作成、編集、削除、すべて表示、すべて変更</td> 
  </tr> 
  <tr> 
   <td>[!DNL Marketo Sales Insight] 設定</td> 
   <td>読み取り、作成、編集、削除、すべて表示、すべて変更</td> 
  </tr> 
  <tr> 
   <td>ScoringCache</td> 
   <td>読み取り、作成、編集、削除、すべて表示、すべて変更</td> 
  </tr> 
  <tr> 
   <td>値</td> 
   <td>読み取り、作成、編集、削除、すべて表示、すべて変更</td> 
  </tr> 
  <tr> 
   <td>WebActivityCache</td> 
   <td>読み取り、作成、編集、削除、すべて表示、すべて変更</td> 
  </tr> 
 </tbody> 
</table>

* Apex クラスアクセス：「mkto_si」で始まる 159 個の Apex クラス
* Visualforce ページアクセス：「mkto_si」で始まる 64 個の Visualforce ページ
* カスタム設定の定義：mkto_si.Marketo 設定と mkto_si.User 環境設定

## [!DNL Sales Insight] へのアクセス権の削除 {#removing-access-to-sales-insight}

1. [!DNL Salesforce] アカウントにログインします。

1. 「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/remove-sales-insight-access-1.png)

1. [!UICONTROL &#x200B; 管理者 &#x200B;] で **[!UICONTROL ユーザーを管理]**/**[!UICONTROL プロファイル]** をクリックします。

1. 更新するプロファイルをクリックし、「**[!UICONTROL 編集]**」をクリックします。

1. [!UICONTROL &#x200B; タブ設定 &#x200B;] の「[!UICONTROL &#x200B; カスタムタブ設定 &#x200B;]」までスクロールダウンします。

1. [!UICONTROL &#x200B; Config および MSI &#x200B;] Outbox のドロップダウンから「[!DNL Marketo Sales Insight]Tab Hidden[!DNL Marketo Sales]」オプションを選択します。

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. 「[!UICONTROL &#x200B; カスタムオブジェクト権限 &#x200B;]」までスクロールします。

1. 次のオブジェクトから「読み取り、作成、編集、削除」アクセスを削除します。

   * BestBetsCache
   * [!DNL Best Bets] 詳細を表示
   * [!DNL Best Bets] Views
   * EmailActivityCache
   * GetMethodArgus
   * GroupedWebActivityCache
   * InterestingMomentsCache
   * [!DNL Marketo Sales Insight] 設定
   * ScoringCache
   * 値
   * WebActivityCache

1. 「[!UICONTROL Apex クラスアクセスを有効にする &#x200B;]」セクションまでスクロールします。 「**[!UICONTROL 編集]**」をクリックします。

1. 「[!UICONTROL Enabled Apex Classes]」セクションで、「mkto_si」で始まるすべてのクラスを選択します。 クラスの合計は 159 個になります。

1. 「**[!UICONTROL 削除]**」をクリックして、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/remove-sales-insight-access-4.png)

1. 「[!UICONTROL &#x200B; 有効な Visualforce ページアクセス &#x200B;]」セクションまでスクロールします。 「**[!UICONTROL 編集]**」をクリックします。

1. 「[!UICONTROL &#x200B; 有効な Visualforce ページ &#x200B;]」セクションから、「mkto_si」で始まるすべてのページを選択します。 ページの合計は 64 個になります。

1. 「**[!UICONTROL 削除]**」をクリックして、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/remove-sales-insight-access-5.png)

1. 「[!UICONTROL &#x200B; 有効なカスタム設定定義へのアクセス &#x200B;]」セクションまでスクロールします。 「**[!UICONTROL 編集]**」をクリックします。

1. 「Marketo Sales Insight.mkto_si.Marketo 設定」および「Marketo Sales Insight.mkto_si.User 環境設定」を選択します。

1. 「**[!UICONTROL 削除]**」をクリックして、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/remove-sales-insight-access-6.png)

これで完了です。[!DNL Sales Insight] アクセスが正常に削除されました。 アクセスを削除する他のプロファイルに対しても同じ手順を繰り返します。
