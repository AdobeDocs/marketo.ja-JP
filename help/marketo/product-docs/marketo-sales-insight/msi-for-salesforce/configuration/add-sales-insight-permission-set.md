---
description: Sales Insight 権限セットの追加 - Marketo ドキュメント - 製品ドキュメント
title: Sales Insight 権限セットの追加
exl-id: b93ddf2e-0f7b-41e0-ba88-7363f5e34970
source-git-commit: cccea2e9b7e1d0017e9be071ec85051f71e737bd
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 100%

---

# Sales Insight 権限セットの追加 {#add-sales-insight-permission-set}

次の手順を使用して、Salesforce の Sales Insight 機能へのアクセスを追加します。Salesforce Classic および Lightning に適用可能

>[!PREREQUISITES]
>
>この機能を使用するには、お使いの [Sales Insight Salesforce パッケージを更新](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target=&quot;_blank&quot;}して、バージョン 1.8000 以降にする必要があります。

>[!IMPORTANT]
>
>以前にすべてのプロファイルに Sales Insight のアクセス権を付与している場合や、すべてのユーザに Sales Insight を実装している場合は、[プロファイルレベルのアクセスを削除](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target=&quot;_blank&quot;}して、この権限セットを使用する必要があります。

## 概要 {#overview}

「Marketo アプリ」権限は、Sales Insight Salesforce パッケージの一部です。これには、以下に示すオブジェクト、apex クラス、visualforce ページへのアクセスが含まれます。これらは、すべての Sales Insight 機能にアクセスするために必要です。

**オブジェクト設定**

<table> 
 <tbody> 
 <tr> 
   <td>BestBetsCache</td> 
   <td>読み取り、作成、編集、削除、すべて表示、すべて変更</td> 
  </tr> 
  <tr> 
   <td>最有望見込客ビューの詳細</td> 
   <td>読み取り、作成、編集、削除、すべて表示、すべて変更</td> 
  </tr> 
  <tr> 
   <td>最有望見込客ビュー</td> 
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
   <td>Marketo Sales Insight の設定</td> 
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

## Marketo アプリ権限セットをユーザに追加 {#adding-marketo-app-permission-set-to-users}

1. Salesforce アカウントにログインします。

1. 「**設定**」をクリックします。

   ![](assets/add-sales-insight-permission-set-1.png)

1. 「管理者」で、「**ユーザを管理**」をクリックし、「**ユーザ**」をクリックします。

   ![](assets/add-sales-insight-permission-set-2.png)

1. 「すべてのユーザ」で、アクセス権を付与するユーザを選択し、「**権限セットの割り当て**」をクリックします。

   ![](assets/add-sales-insight-permission-set-3.png)

1. 「**割り当てを編集**」をクリックします。

   ![](assets/add-sales-insight-permission-set-4.png)

1. 使用可能な権限セットから「**Marketo アプリアクセス**」を選択し、「**追加**」を選択します。「**保存**」をクリックします。

   ![](assets/add-sales-insight-permission-set-5.png)

1. ユーザの詳細ページを下にスクロールすると、「権限セットの割り当て」の下に「Marketo アプリアクセス」が表示されます。

   ![](assets/add-sales-insight-permission-set-6.png)

>[!NOTE]
>
>Sales Insight へのアクセス権を持たないユーザには、「このタブにアクセスするのに十分な権限がありません」というメッセージが表示されます。

これで完了です。Sales Insight へのアクセス権が正常に追加されました。アクセスを追加する他のプロファイルに対しても同じ手順を繰り返します。
