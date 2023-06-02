---
description: Sales Insight Actions 管理者設定ガイド - Marketo ドキュメント - 製品ドキュメント
title: Sales Insight Actions 管理者設定ガイド
exl-id: 339d518d-445b-4634-ab81-92c9d5541927
source-git-commit: f238214988ae396d7c6e6ad0bd46fff232d442d6
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 94%

---

# Sales Insight Actions 管理者設定ガイド {#sales-insight-actions-admin-setup-guide}

>[!NOTE]
>
>Marketo Sales Insight Actions は、 [Marketo Sales Insight パッケージ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. 「Marketoセールス」、単に「アクション」とも呼ばれます。

>[!PREREQUISITES]
>
>* MSI アクションが Marketo Engage アカウントで有効になっていることをアドビアカウントチーム（担当のアカウントマネージャー）に確認します（アカウントマネージャーがいない場合は、[Marketo サポート](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}にお問い合わせください）。
>* Marketo と Salesforce の同期を設定する必要があります。


<table>
 <tr>
  <th>ペルソナ</th>
  <th>ステップ</th>
 </tr>
 <tr>
  <td>Marketo 管理者</td>
  <td>Marketo Sales アカウントの設定</td>
 </tr>
 <tr>
  <td>Marketo 管理者または <br/>Salesforce 管理者</td>
  <td>Marketo Sales アカウントの Salesforce への接続</td>
 </tr>
 <tr>
  <td>Marketo 管理者</td>
  <td>Marketo Sales アカウントを Marketo に接続</td>
 </tr>
 <tr>
  <td>Marketo 管理者</td>
  <td>Marketo から Marketo Sales アカウントへのデータ同期の開始</td>
 </tr>
 <tr>
  <td>Marketo 管理者</td>
  <td>ユーザを MSI-Actions に招待する</td>
 </tr>
 <tr>
  <td>Salesforce 管理者</td>
  <td>Salesforce での MSI パッケージのインストール／アップグレード</td>
 </tr>
 <tr>
  <td>Salesforce 管理者</td>
  <td>Salesforce での MSI アクションの設定</td>
 </tr>
</table>

## Marketo Sales アカウントの設定 {#set-up-marketo-sales-account}

1. Marketo で、「**管理者**」をクリックします。

   ![](assets/msi-actions-admin-guide-1.png)

1. 「**Sales Insight**」をクリックし、「**アクション設定**」をクリックします。Marketo 管理者のリストから選択し、「**招待を送信**」をクリックして招待します。

   ![](assets/msi-actions-admin-guide-2.png)

アカウントにアクセスする手順が記載されたメールがユーザに送信されます。

>[!NOTE]
>
>追加のユーザーは、Marketo からは追加されず、代わりに Sales アカウントのユーザー管理ページから追加されます。ユーザーの追加について詳しくは、[こちらをクリック](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md){target="_blank"}してください。

## Marketo Sales アカウントの Salesforce への接続 {#connect-marketo-sales-account-to-salesforce}

1. Marketo Sales アカウントで、歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/msi-actions-admin-guide-3.png)

1. 管理設定で、**Salesforce** をクリックします。

   ![](assets/msi-actions-admin-guide-4.png)

1. 「接続とカスタマイズ」タブで、「**接続**」をクリックします。

   ![](assets/msi-actions-admin-guide-5.png)

1. 「**OK**」をクリックします。

   ![](assets/msi-actions-admin-guide-6.png)

既に Salesforce にログインしている場合は、Salesforce に接続されます。まだログインしていない場合は、ログインするように求められます。

## Marketo をセールスアプリアカウントに接続 {#connect-marketo-to-your-sales-apps-account}

1. Marketo Sales アカウントで、歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/msi-actions-admin-guide-7.png)

1. 「管理者設定」で、「**Marketo**」をクリックします。

   ![](assets/msi-actions-admin-guide-8.png)

1. 「**接続**」をクリックします。アカウントが接続されます。

   ![](assets/msi-actions-admin-guide-9.png)

>[!NOTE]
>
>接続できない場合は、Marketo Sales Insight の「アクション設定」タブから資格情報をコピーし、「設定」タブにペーストします。

## データ同期の開始 {#initiate-data-sync}

Sales Insight Actions のデータ統合フィールドの同期により、Marketo Engage データベースから Sales Insight Actions データベースに個人情報を取り込み、個人データを最新の状態に保ち、Marketo と Salesforce で適切なレコードにアクティビティを記録できます。

>[!CAUTION]
>
>データ同期を開始したら、Sales Insight Actions インスタンスから元のユーザを&#x200B;**削除しない**&#x200B;ようにします。これは、最初の招待が送信されたユーザです。

1. Marketo で、「**管理者**」をクリックします。

   ![](assets/msi-actions-admin-guide-10.png)

1. 「**Sales Insight**」をクリックします。

   ![](assets/msi-actions-admin-guide-11.png)

1. 「**アクション設定**」タブをクリックします。「アクションフィールドを同期」カードで、「**同期**」をクリックします。

   ![](assets/msi-actions-admin-guide-12.png)

1. 同期されるフィールドのプレビューが表示されます。「**同期の開始**」をクリックします。

   ![](assets/msi-actions-admin-guide-13.png)

Marketo と Salesforce に存在する人物レコードが、Marketo Sales アプリアカウントと同期されます。

>[!NOTE]
>
>Sales Insight Actions、Marketo、Salesforce 間の人物とアクティビティのデータ同期について詳しくは、[こちらをクリック](/help/marketo/product-docs/marketo-sales-insight/actions/admin/actions-data-sync-faq.md){target="_blank"}してください。

## 個々のユーザを MSI Actions に招待する {#invite-individual-users-to-msi-actions}

1. Marketo Sales アカウントで、歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/msi-actions-admin-guide-14.png)

1. 「管理者設定」で、「**ユーザ管理**」を選択します。

   ![](assets/msi-actions-admin-guide-15.png)

1. 「**Actions**」をクリックし、「**ユーザを招待する**」を選択します。

   ![](assets/msi-actions-admin-guide-16.png)

1. メールアドレスを入力し、「**招待する**」をクリックします。

   ![](assets/msi-actions-admin-guide-17.png)

>[!NOTE]
>
>デフォルトでは、すべての新規メンバーが全員チームに追加されます。

確認メッセージが表示されます。

## CSV 経由で MSI アクションにユーザを招待する {#invite-users-via-csv-to-msi-actions}

1. Marketo Sales アカウントで、歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/msi-actions-admin-guide-18.png)

1. 「管理者設定」で、「**ユーザ管理**」を選択します。

   ![](assets/msi-actions-admin-guide-19.png)

1. 「**Actions**」をクリックし、「**CSV 経由でユーザを招待する**」を選択します。

   ![](assets/msi-actions-admin-guide-20.png)

1. PC 上の CSV ファイルを参照して選択し、「**次へ**」をクリックします。

   ![](assets/msi-actions-admin-guide-21.png)

1. フィールドが正しくマッピングされていることを確認し、「**次へ**」をクリックします。

   ![](assets/msi-actions-admin-guide-22.png)

招待が送信されると、確認メッセージが表示されます。

>[!NOTE]
>
>これが完了したら、既存の MSI パッケージをアップグレードするか、新しいパッケージをインストールして、[Salesforce での MSI アクションの設定](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-configuration/sales-insight-actions-configuration-in-salesforce.md){target="_blank"}に進みます。
