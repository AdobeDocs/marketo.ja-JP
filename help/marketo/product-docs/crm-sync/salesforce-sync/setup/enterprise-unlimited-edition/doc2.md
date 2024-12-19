---
description: 手順 2/3 - MarketoのSalesforce ユーザーを作成（Enterprise/Unlimited） – Marketo ドキュメント – 製品ドキュメント
title: 手順 2/3 - MarketoのSalesforce ユーザーを作成する（Enterprise/Unlimited）
hide: true
hidefromtoc: true
feature: Salesforce Integration
source-git-commit: 989804463f44afbf35ab11c0f23c37b0d328e652
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 57%

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

   スクリーンショット

1. ナビゲーション検索バーに「プロファイル」と入力し、「プロファイル」リンクをクリックします。

   スクリーンショット

1. 「新規プロファイル」をクリックします。

   スクリーンショット

1. 「標準ユーザー」を選択し、プロファイルに「Marketo - Salesforce同期」という名前を付けて、「保存」をクリックします。

   スクリーンショット

## プロファイル権限の設定 {#set-profile-permissions}

1. 「編集」をクリックして、セキュリティ権限を設定します。

   スクリーンショット

1. 「管理者権限」セクションで、次のチェックボックスがオンになっていることを確認します。

   * API 有効
   * HTML テンプレートを編集
   * 公開ドキュメントを管理
   * 公開テンプレートを管理

   >[!TIP]
   >
   >パスワードの有効期限なしボックスのチェックは必ずオンにしてください。

1. 一般ユーザー権限セクションで、次のボックスがオンになっていることを確認します。

   * リードをコンバート
   * イベントを編集
   * タスクを編集

1. 標準オブジェクト権限セクションで、読み取り、作成、編集、削除の権限が次の項目に対して有効になっていることを確認します。

   * アカウント
   * キャンペーン
   * 取引先責任者
   * リード
   * 商談

   >[!NOTE]
   >
   >キャンペーン同期を使用する予定がある場合は、キャンペーンに権限を付与します。

   スクリーンショット

1. 終了したら、ページ下部の「保存」をクリックします。

   スクリーンショット

## フィールド権限の設定 {#set-field-permissions}

1. 同期に必要なカスタムフィールドをマーケターと話し合います。

   >[!NOTE]
   >
   >この手順を実行すると、Marketo に表示する必要のないフィールドが防止され、混乱が軽減され、同期が高速化されます。

1. プロファイルの詳細ページで、フィールドレベルのセキュリティセクションに移動します。「表示」をクリックして、オブジェクトのアクセシビリティを編集します。

   * リード
   * 取引先責任者
   * アカウント
   * 商談

   >[!TIP]
   >
   >組織のニーズに応じて、他のオブジェクトを設定できます。

1. オブジェクトごとに「編集」をクリックします。

   スクリーンショット

1. 不要なフィールドを探し、「読み取りアクセス」と「編集アクセス」がオフになっていることを確認します。 終了したら「保存」をクリックします。

   >[!NOTE]
   >
   >カスタムフィールドのアクセシビリティのみを編集します。

   スクリーンショット

1. 不要なフィールドをすべて無効にした後は、次のオブジェクトフィールドの「読み取りアクセス」と「編集アクセス」をオンにする必要があります。 終了したら「保存」をクリックします。

   テーブル

   スクリーンショット

## Marketo-Salesforce 同期アカウントを作成 {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>専用のSalesforce アカウント（`marketo@yourcompany.com` など）を作成して、Marketoによる変更を他のSalesforce ユーザーと区別します。

1. ナビゲーションの検索バーに「ユーザーの管理」と入力し、「ユーザー」をクリックします。 「新規ユーザー」をクリックします。

   スクリーンショット

   スクリーンショット

1. 必須フィールドに入力します。次に、「ユーザーライセンス : Salesforce」と、以前に作成したプロファイルを選択します。 完了したら、「保存」をクリックします。

   スクリーンショット

手順 2／3 が完了しました。
