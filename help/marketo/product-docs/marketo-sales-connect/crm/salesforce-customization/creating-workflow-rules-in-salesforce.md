---
unique-page-id: 14745823
description: Salesforce でのワークフロールールの作成 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce でのワークフロールールの作成
exl-id: 0cfce178-453b-4949-96aa-c327278a267d
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 59%

---

# Salesforce でのワークフロールールの作成 {#creating-workflow-rules-in-salesforce}

Marketo Sales Insight（MSI）とMarketo Sales Connect （MSC）を並行して使用する場合、[!DNL Salesforce] の MSI のおすすめコンテンツ機能が更新されません。 その他の MSI 機能はすべて通常どおりに動作します（iFrame での注目のアクションの表示、メール送信、キャンペーンへの追加など）。この記事では、最有望見込客を再度機能させるための回避策を示します。

>[!NOTE]
>
>これは、**MSI と MSE の両方**&#x200B;を使用し、MSI の最有望見込客機能を使用する顧客にのみ影響します。最有望見込客が不要な場合は、無視してかまいません。

## 開始方法 {#getting-started}

回避策には、新しい MSE フィールドの値を古い MSI フィールドにコピーする新しいワークフロールールの作成が含まれます。独自の [!DNL Salesforce] インスタンスで、連絡先オブジェクト用に 4 つのワークフロールールとリードオブジェクト用に同じ 4 つのワークフロールールを作成する必要があります。 これには、（CRM の役割と設定に応じて）CRM 管理者権限が必要になる場合があります。

以下に、ワークフロールールの推奨名とそれぞれの説明を示します。これらは、[!UICONTROL &#x200B; 連絡先 &#x200B;] および [!UICONTROL &#x200B; リード &#x200B;] オブジェクトに適用されます。

<table>
 <colgroup>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <td>「注目のアクションの詳細」フィールドの更新</td>
   <td><p>コピー元：最新の Marketo エンゲージメントの詳細<br>コピー先：最新の注目のアクションの詳細</p></td>
  </tr>
  <tr>
   <td>「注目のアクションのタイプ」フィールドの更新</td>
   <td><p>コピー元：最新の Marketo エンゲージメントのタイプ<br>コピー先：最新の注目のアクションのタイプ</p></td>
  </tr>
  <tr>
   <td>「最新の注目のアクションのソース」フィールドの更新</td>
   <td><p>コピー元：最新の Marketo エンゲージメントのソース<br>コピー先：最新の注目のアクションのソース</p></td>
  </tr>
  <tr>
   <td>「最新の注目のアクションの日付」フィールドの更新</td>
   <td><p>コピー元：最新の Marketo エンゲージメントの日付<br>コピー先：最新の注目のアクションの日付</p></td>
  </tr>
 </tbody>
</table>

## 入力ガイド {#instructions}

1. **[!UICONTROL 設定]** をクリックした後、**ワークフロー** を検索し、**[!UICONTROL ワークフロールール]** を選択します。

   ![](assets/one-1.png)

1. 「**[!UICONTROL 新規ルール]**」を選択します。

   ![](assets/two-1.png)

1. [!UICONTROL &#x200B; オブジェクト &#x200B;] ドロップダウンをクリックし、**[!UICONTROL リード]** を選択して **[!UICONTROL 次へ]** をクリックします。

   ![](assets/three-1.png)

1. [!UICONTROL &#x200B; ルール名 &#x200B;] として「注目のモーメントの説明フィールドを更新」と入力します。 **[!UICONTROL 作成したラジオボタンを選択し、編集のたびに選択します]**。[!UICONTROL &#x200B; ルールの条件 &#x200B;] ドロップダウンで、「**[!UICONTROL 数式の評価結果が true]**」を選択します。 ISCHANGED 関数を検索して選択します。次に、デフォルトのフィールド値をハイライト表示し、「**[!UICONTROL フィールドを挿入]**」をクリックします。

   ![](assets/four-1.png)

1. 「[!UICONTROL &#x200B; フィールドを挿入 &#x200B;]」ポップアップで、「前回のMarketo契約説明 **[!UICONTROL を選択し]** 「**[!UICONTROL 挿入]**」をクリックします。

   ![](assets/five-1.png)

1. 「**[!UICONTROL 保存して次へ]**」をクリックします。

   ![](assets/6.png)

1. [!UICONTROL &#x200B; ワークフローアクションを追加 &#x200B;] ドロップダウンで、「**[!UICONTROL 新しいフィールドの更新]**」を選択します。

   ![](assets/seven.png)

1. 「[!UICONTROL &#x200B; 名前 &#x200B;]」フィールドに「注目のモーメントの説明フィールドを更新」と入力します（[!UICONTROL &#x200B; 一意の名前 &#x200B;] が自動生成されます）。 [!UICONTROL &#x200B; 更新するフィールド &#x200B;] ドロップダウンで、「**[!UICONTROL 最終注目のモーメントの説明]**」を選択します。 「**[!UICONTROL 数式を使用して新しい値を設定]**」ラジオボタンを選択し、「**[!UICONTROL 数式エディターを表示]**」をクリックします。

   ![](assets/eight.png)

1. 「**[!UICONTROL フィールドを挿入]**」ボタンをクリックします。

   ![](assets/9a.png)

1. 「**[!UICONTROL 最新の Marketo エンゲージメントの詳細]**」を選択し、「**[!UICONTROL 挿入]**」をクリックします。次のページで、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/nine.png)

1. 「**[!UICONTROL 完了]**」をクリックします。

   ![](assets/twelve.png)

1. 「**[!UICONTROL アクティブ化]**」をクリックして、ワークフロールールをオンにします。

   ![](assets/thirteen.png)

   最後の手順の後、「はじめに [!UICONTROL &#x200B; セクション：説明、タイプ、Source、日付にリストされている他のフィールドのワークフロールールを複製する &#x200B;] とができます。 [!UICONTROL &#x200B; 連絡先 &#x200B;] オブジェクトの 4 つのワークフロールールを完了したら、同じ手順を [!UICONTROL &#x200B; リード &#x200B;] オブジェクトに対して繰り返します。
