---
unique-page-id: 2360364
description: 手順 2／3 - Marketo 用の Salesforce ユーザーの作成（Enterprise／Unlimited）- Marketo ドキュメント - 製品ドキュメント
title: 手順 2／3 - Marketo 用の Salesforce ユーザーの作成（Enterprise／Unlimited）
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
feature: Salesforce Integration
source-git-commit: c10ecc0ccad28f2e480343acefe10f5eca2ae578
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 93%

---

# 手順 2／3：Marketo 用の Salesforce ユーザーの作成（Enterprise／Unlimited） {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>これらの手順は、Salesforce 管理者が実行する必要があります

>[!PREREQUISITES]
>
>[手順 1／3：Marketo フィールドの Salesforce への追加（Enterprise／Unlimited）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}

この記事では、Salesforce プロファイルでユーザー権限を設定し、Marketo-Salesforce 統合アカウントを作成します。

## プロファイルの作成 {#create-a-profile}

1. 「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. ナビゲーション検索バーに「プロファイル」と入力し、**[!UICONTROL プロファイル]**&#x200B;リンクをクリックします。

   ![](assets/sfdc-profiles-hands.png)

1. 「**[!UICONTROL 新規]**」をクリックします。

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. **[!UICONTROL 標準ユーザー]** を選択し、プロファイルに「Marketo - Salesforce同期」という名前を付けて **[!UICONTROL 保存]** をクリックします。

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## プロファイル権限の設定 {#set-profile-permissions}

1. 「**[!UICONTROL 編集]**」をクリックしてセキュリティ権限を設定します。

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. **[!UICONTROL 管理権限]**&#x200B;セクションで、次のボックスがオンになっていることを確認します。

   * API 有効
   * HTML テンプレートを編集
   * 公開ドキュメントを管理
   * 公開テンプレートを管理

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >**[!UICONTROL パスワードの有効期限なし]**&#x200B;ボックスのチェックは必ずオンにしてください。

1. 一般ユーザー権限セクションで、次のボックスがオンになっていることを確認します。

   * リードをコンバート
   * イベントを編集
   * タスクを編集

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. 標準オブジェクト権限セクションで、読み取り、作成、編集、削除の権限が次の項目に対して有効になっていることを確認します。

   * アカウント
   * キャンペーン
   * 取引先責任者
   * リード
   * 商談

   >[!NOTE]
   >
   >キャンペーン同期を使用する予定がある場合は、キャンペーンに権限を付与します。

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. 終了したら、ページの下部にある「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## フィールド権限の設定 {#set-field-permissions}

1. 同期に必要なカスタムフィールドをマーケターと話し合います。

   >[!NOTE]
   >
   >この手順を実行すると、Marketo に表示する必要のないフィールドが防止され、混乱が軽減され、同期が高速化されます。

1. プロファイルの詳細ページで、**[!UICONTROL フィールドレベルのセキュリティ]**&#x200B;セクションに移動します。オブジェクトのアクセシビリティを編集するには、「**[!UICONTROL 表示]**」をクリックします。

   * リード
   * 取引先責任者
   * アカウント
   * 商談

   >[!TIP]
   >
   >組織のニーズに応じて、他のオブジェクトを設定できます。

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. 各オブジェクトに対して、「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/sfdc-sync-field-edit1.png)

1. 不要なフィールドを見つけ、**[!UICONTROL 読み取りアクセス]**&#x200B;と&#x200B;**[!UICONTROL 編集アクセスを]**&#x200B;がオフになっていることを確認してください。終了したら「**[!UICONTROL 保存]**」をクリックします。

   >[!NOTE]
   >
   >カスタムフィールドのアクセシビリティのみを編集します。

   ![](assets/sfdc-sync-field-edit2.png)

1. 不要なフィールドをすべて無効にした後で、次のオブジェクトフィールドの&#x200B;**[!UICONTROL 読み取りアクセスと編集アクセス]**&#x200B;のチェックをオンにします。終了したら「**[!UICONTROL 保存]**」をクリックします。

<table> 
 <tbody> 
  <tr> 
   <th>オブジェクト</th> 
   <th>フィールド</th> 
  </tr> 
  <tr> 
   <td>アカウント</td> 
   <td>タイプフィールド</td> 
  </tr> 
  <tr> 
   <td>イベント</td> 
   <td>すべてのフィールド</td> 
  </tr> 
  <tr> 
   <td>タスク</td> 
   <td>すべてのフィールド</td> 
  </tr> 
 </tbody> 
</table>

![](assets/sfdc-check-the-boxes.png)

## Marketo-Salesforce 同期アカウントを作成 {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>専用のSalesforce アカウント（`marketo@yourcompany.com` など）を作成して、Marketoによる変更を他のSalesforce ユーザーと区別します。

1. ナビゲーション検索バーに「ユーザーを管理」と入力し、「**[!UICONTROL ユーザー]**」をクリックします。「**[!UICONTROL 新規ユーザ]**」をクリックします。

   ![](assets/sfdc-new-users.png)

1. 必須フィールドに入力します。次に、「**[!UICONTROL ユーザライセンス：Salesforce]**」と、以前に作成したプロファイルを選択します。完了したら、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-12-9-9-3a20-3a56.png)

手順 2／2 が完了しました。

>[!NOTE]
>
>[手順 3 / 3：Marketo と Salesforce の接続（Enterprise／Unlimited）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md){target="_blank"}
