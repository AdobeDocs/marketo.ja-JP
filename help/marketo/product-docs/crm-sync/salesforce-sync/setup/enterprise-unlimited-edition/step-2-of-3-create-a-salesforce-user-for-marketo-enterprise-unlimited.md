---
unique-page-id: 2360364
description: 手順2/3 - Marketor向けSalesforceユーザーの作成(Enterprise/Unlimited) - Marketto Docs — 製品ドキュメント
title: ステップ2/3 - Marketto向けSalesforceユーザーの作成(Enterprise/Unlimited)
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---


# 手順2/3:Marketor向けSalesforceユーザーの作成(Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>これらの手順は、Salesforce管理者が実行する必要があります

>[!PREREQUISITES]
>
>[手順1/3:Salesforce追加に対するマーケティング担当者のフィールド(Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

この記事では、Salesforceプロファイルでユーザー権限を設定し、Marketor-Salesforce統合アカウントを作成します。

## プロファイルの作成{#create-a-profile}

1. 「**セットアップ**」をクリックします。

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. ナビゲーション検索バーに「プロファイル」と入力し、**プロファイル**&#x200B;リンクをクリックします。

   ![](assets/sfdc-profiles-hands.png)

1. 「**新規**」をクリックします。

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. 「**標準ユーザー**」を選択し、プロファイルに「Marketo-Salesforce Sync」という名前を付けて、「**保存**」をクリックします。

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## プロファイル権限の設定{#set-profile-permissions}

1. 「**編集**」をクリックして、セキュリティ権限を設定します。

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. 「**管理権限**」セクションで、次のチェックボックスがオンになっていることを確認します。

   * API有効
   * HTMLテンプレートの編集
   * パブリックドキュメントの管理
   * 公開テンプレートの管理

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >「**パスワードの有効期限が切れない**」ボックスを必ずチェックしてください。

1. 「一般的なユーザー権限」セクションで、次のチェックボックスがオンになっていることを確認します。

   * リードのコンバージョン
   * イベントの編集
   * タスクの編集

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. 「標準オブジェクト権限」セクションで、「読み取り」、「作成」、「編集」、「削除」の権限が次の対象になっていることを確認します。

   * アカウント
   * キャンペーン
   * 連絡先
   * リード
   * オポチュニティ

   >[!NOTE]
   >
   >キャンペーン同期を使用する予定がある場合は、キャンペーンに権限を付与します。

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. 終了したら、ページの下部にある「**保存**」をクリックします。

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## フィールド権限の設定{#set-field-permissions}

1. 同期に必要なカスタムフィールドを調べるには、マーケターと相談してください。

   >[!NOTE]
   >
   >この手順により、不要なフィールドがMarketoに表示されるのを防ぎ、混乱を軽減し、同期を高速化します。

1. プロファイルの詳細ページで、「**フィールドレベルセキュリティ**」セクションに移動します。 **表示**&#x200B;をクリックして、オブジェクトのアクセシビリティを編集します。

   * リード
   * 連絡先
   * アカウント
   * オポチュニティ

   >[!TIP]
   >
   >組織のニーズに応じて、他のオブジェクトを設定できます。

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. 各オブジェクトに対して、「**編集**」をクリックします。

   ![](assets/sfdc-sync-field-edit1.png)

1. 不要なフィールドを探し、「**読み取りアクセス**」と「**アクセスを編集**」がオフになっていることを確認します。 終了したら「**保存**」をクリックします。

   >[!NOTE]
   >
   >カスタムフィールドのアクセシビリティの編集のみを行います。

   ![](assets/sfdc-sync-field-edit2.png)

1. 不要なフィールドをすべて無効にした後、次のオブジェクトフィールドについて、**読み取りアクセスと編集アクセス**&#x200B;をチェックする必要があります。 終了したら「**保存**」をクリックします。

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1"><p>オブジェクト</p></th> 
   <th colspan="1" rowspan="1"><p>フィールド</p></th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>アカウント</p></td> 
   <td colspan="1" rowspan="1"><p>タイプフィールド</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>イベント</p></td> 
   <td colspan="1" rowspan="1"><p>すべてのフィールド</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>タスク</p></td> 
   <td colspan="1" rowspan="1"><p>すべてのフィールド</p></td> 
  </tr> 
 </tbody> 
</table>

![](assets/sfdc-check-the-boxes.png)

## Marketo-Salesforce同期アカウントを作成{#create-marketo-salesforce-sync-account}

>[!TIP]
>
>専用のSalesforceアカウント(marketo@yourcompany.comなど)を作成して、Marketoが行った変更と他のSalesforceユーザーが行った変更を区別します。

1. ナビゲーション検索バーに「ユーザーを管理」と入力し、「**ユーザー**」をクリックします。 「**新しいユーザー**」をクリックします。

   ![](assets/sfdc-new-users.png)

1. 必須フィールドに入力します。 次に、**ユーザーライセンスを選択します。Salesforce**&#x200B;と、以前に作成したプロファイル。 終了したら「**保存**」をクリックします。

   ![](assets/image2014-12-9-9-3a20-3a56.png)

ステップ2/2が完了。

>[!NOTE]
>
>[手順3/3:MarketoとSalesforceの連携(Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
