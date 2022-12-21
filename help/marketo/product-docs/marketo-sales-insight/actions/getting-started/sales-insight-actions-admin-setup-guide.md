---
description: Sales Insight Actions 管理者設定ガイド - Marketo ドキュメント - 製品ドキュメント
title: Sales Insight Actions 管理者設定ガイド
exl-id: 339d518d-445b-4634-ab81-92c9d5541927
source-git-commit: 9f3b91e7b0626b2a229f4a98fb734e926a141ec0
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 100%

---

# Sales Insight Actions 管理者設定ガイド {#sales-insight-actions-admin-setup-guide}

>[!PREREQUISITES]
>
>* Marketo アカウントで MSI アクションが有効になっていることをカスタマーサクセスマネージャーに確認してくださいをクリックします（CSM をお持ちでない場合は、[Marketo サポートに連絡](https://nation.marketo.com/t5/support/ct-p/Support){target=&quot;_blank&quot;}してください）。
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
>追加のユーザは、Marketo からは追加されず、代わりに Sales アカウントのユーザ管理ページから追加されます。ユーザの追加について詳しくは、[こちらをクリック](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md){target=&quot;_blank&quot;}してください。

## Marketo Sales アカウントの Salesforce への接続 {#connect-marketo-sales-account-to-salesforce}

1. Marketo Sales アカウントで、歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/msi-actions-admin-guide-3.png)

1. 管理設定で、**Salesforce** をクリックします。

   ![](assets/msi-actions-admin-guide-4.png)

1. 「接続とカスタマイズ」タブで、「**接続**」をクリックします。

   ![](assets/msi-actions-admin-guide-5.png)

1. 「**OK**」をクリックします。

   ![](assets/msi-actions-admin-guide-6.png)

既に Salesforce にログインしている場合は、接続されます。そうでない場合は、ログインするように求められます。

## Marketo をセールスアプリアカウントに接続 {#connect-marketo-to-your-sales-apps-account}

1. Marketo Sales アカウントで、歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/msi-actions-admin-guide-7.png)

1. 「管理者設定」で、「**Marketo**」をクリックします。

   ![](assets/msi-actions-admin-guide-8.png)

1. 「**接続**」をクリックします。アカウントが接続されます。

   ![](assets/msi-actions-admin-guide-9.png)

>[!NOTE]
>
>接続できない場合は、資格情報を Marketo Sales Insight の「アクション設定」タブからコピーし、「設定」タブに貼り付けます。

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
>Sales Insight Actions、Marketo、Salesforce 間のユーザとアクティビティのデータの同期について詳しくは、[ここをクリック](/help/marketo/product-docs/marketo-sales-insight/actions/admin/actions-data-sync-faq.md){target=&quot;_blank&quot;}します。

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
>これが完了したら、既存の MSI パッケージをアップグレードするか、新しいパッケージをインストールして、[Salesforce での MSI アクションの設定](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-configuration/sales-insight-actions-configuration-in-salesforce.md){target=&quot;_blank&quot;}に進みます。
