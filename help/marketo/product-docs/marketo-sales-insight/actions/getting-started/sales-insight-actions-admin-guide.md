---
description: Sales Insight Actions 管理ガイド — Marketoドキュメント — 製品ドキュメント
title: Sales Insight アクション管理ガイド
exl-id: 339d518d-445b-4634-ab81-92c9d5541927
source-git-commit: fc94cd3b62b0afd8122c56773d420f385d30dabd
workflow-type: tm+mt
source-wordcount: '588'
ht-degree: 11%

---

# Sales Insight アクション管理ガイド {#sales-insight-actions-admin-guide}

>[!PREREQUISITES]
>
>* Marketoアカウントで MSI アクションが有効になっていることをカスタマーサクセスマネージャーに確認してください (CSM をお持ちでない場合は、 [Marketoサポートに連絡](https://nation.marketo.com/t5/support/ct-p/Support)) をクリックします。
>* Marketo/Salesforce 同期を設定する必要があります。


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
  <td>Marketo Admin または <br/>Salesforce 管理者</td>
  <td>Marketoセールスアカウントを Salesforce に接続</td>
 </tr>
 <tr>
  <td>Marketo 管理者</td>
  <td>Marketo Sales アカウントをMarketoに接続</td>
 </tr>
 <tr>
  <td>Marketo 管理者</td>
  <td>MarketoからMarketoセールスアカウントへのデータ同期の開始</td>
 </tr>
 <tr>
  <td>Marketo 管理者</td>
  <td>ユーザを MSI-Actions に招待する</td>
 </tr>
 <tr>
  <td>Salesforce 管理者</td>
  <td>Salesforce での MSI パッケージのインストール/アップグレード</td>
 </tr>
 <tr>
  <td>Salesforce 管理者</td>
  <td>Salesforce での MSI-Actions の設定</td>
 </tr>
</table>

## Marketoセールスアカウントの設定 {#set-up-marketo-sales-account}

1. Marketo で、「**管理者**」をクリックします。

   ![](assets/msi-actions-admin-guide-1.png)

1. クリック **Sales Insight**&#x200B;を、 **アクション設定**. 招待するMarketo管理者のリストから選択し、 **招待の送信**.

   ![](assets/msi-actions-admin-guide-2.png)

アカウントにアクセスする手順が記載された電子メールがユーザーに送信されます。

>[!NOTE]
>
>追加のユーザーは、Marketoからは追加されず、代わりにセールスアカウントのユーザー管理ページから追加されます。 [ここをクリック](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md) を参照して、ユーザーの追加について確認してください。

## Marketoセールスアカウントを Salesforce に接続 {#connect-marketo-sales-account-to-salesforce}

1. Marketo Sales アカウントで、歯車アイコンをクリックし、 **設定**.

   ![](assets/msi-actions-admin-guide-3.png)

1. 管理設定で、**Salesforce** をクリックします。

   ![](assets/msi-actions-admin-guide-4.png)

1. 「接続とカスタマイズ」タブで、「**接続**」をクリックします。

   ![](assets/msi-actions-admin-guide-5.png)

1. 「**OK**」をクリックします。

   ![](assets/msi-actions-admin-guide-6.png)

既に Salesforce にログインしている場合は、連携します。 ログインしていない場合は、ログインするように求められます。

## Marketoをセールスアプリアカウントに接続 {#connect-marketo-to-your-sales-apps-account}

1. Marketo Sales アカウントで、歯車アイコンをクリックし、 **設定**.

   ![](assets/msi-actions-admin-guide-7.png)

1. 管理者設定で、 **Marketo**.

   ![](assets/msi-actions-admin-guide-8.png)

1. クリック **接続**. アカウントが接続されます。

   ![](assets/msi-actions-admin-guide-9.png)

>[!NOTE]
>
>接続できない場合は、資格情報をMarketo Sales Insight の「Actions Config」タブからコピーし、「設定」タブに貼り付けます。

## データ同期の開始 {#initiate-data-sync}

Sales Insight Actions のデータ統合フィールドの同期により、Marketo Engageデータベースから Sales Insight Actions データベースに個人情報を取り込み、個人データを最新の状態に保ち、Marketoと Salesforce で適切なレコードにアクティビティを記録できます。

>[!CAUTION]
>
>データ同期を開始したら、以下を実行する必要があります。 **not** Sales Insight Actions インスタンスから元のユーザーを削除します。 これは、最初の招待が送信されたユーザーです。

1. Marketo で、「**管理者**」をクリックします。

   ![](assets/msi-actions-admin-guide-10.png)

1. 「**Sales Insight**」をクリックします。

   ![](assets/msi-actions-admin-guide-11.png)

1. 次をクリック： **アクション設定** タブをクリックします。 「アクションフィールドの同期」カードで、 **同期**.

   ![](assets/msi-actions-admin-guide-12.png)

1. 同期されるフィールドのプレビューが表示されます。 「**同期の開始**」をクリックします。

   ![](assets/msi-actions-admin-guide-13.png)

Marketoと Salesforce に存在する担当者レコードは、Marketoセールスアプリアカウントと同期されます。

>[!NOTE]
>
>Sales Insight Actions、Marketo、Salesforce 間のユーザーとアクティビティのデータの同期の詳細 [ここをクリック](/help/marketo/product-docs/marketo-sales-insight/actions/admin/actions-data-sync-faq.md).

## 個々のユーザを MSI アクションに招待する {#invite-individual-users-to-msi-actions}

1. Marketo Sales アカウントで、歯車アイコンをクリックし、 **設定**.

   ![](assets/msi-actions-admin-guide-14.png)

1. 管理設定で、「**ユーザー管理**」を選択します。

   ![](assets/msi-actions-admin-guide-15.png)

1. クリック **アクション** を選択し、 **ユーザーの招待**.

   ![](assets/msi-actions-admin-guide-16.png)

1. 電子メールアドレスを入力し、 **招待**.

   ![](assets/msi-actions-admin-guide-17.png)

>[!NOTE]
>
>デフォルトでは、すべての新規メンバーが「全員」チームに追加されます。

確認メッセージが表示されます。

## CSV 経由で MSI アクションにユーザを招待する {#invite-users-via-csv-to-msi-actions}

1. Marketo Sales アカウントで、歯車アイコンをクリックし、 **設定**.

   ![](assets/msi-actions-admin-guide-18.png)

1. 管理設定で、「**ユーザー管理**」を選択します。

   ![](assets/msi-actions-admin-guide-19.png)

1. クリック **アクション** を選択し、 **CSV でユーザーを招待**.

   ![](assets/msi-actions-admin-guide-20.png)

1. コンピューター上の CSV を参照し、選択して、 **次へ**.

   ![](assets/msi-actions-admin-guide-21.png)

1. フィールドが正しくマッピングされていることを確認し、 **招待**.

   ![](assets/msi-actions-admin-guide-22.png)

招待が送信されると、確認メッセージが表示されます。

>[!NOTE]
>
>これが完了したら、既存の MSI パッケージをアップグレードするか、新しいパッケージをインストールして、次の手順に進みます。 [Salesforce での MSI アクションの設定](/help/marketo/product-docs/marketo-sales-insight/actions/salesforce-configuration/sales-insight-actions-configuration-in-salesforce.md).
