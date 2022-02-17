---
description: 手順 2 / 4 — リソース所有者のパスワード制御接続を使用したMarketoソリューションのセットアップ — Marketoドキュメント — 製品ドキュメント
title: 手順 2/4 — リソース所有者のパスワード制御接続を使用してMarketoソリューションをセットアップする
exl-id: 41c05910-d8e3-4fb7-8f68-17ee10294e57
source-git-commit: 19c568cdc3d31d07e42e99eb7e48f10a017b44f9
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# 手順 2/4:リソース所有者のパスワード制御接続を使用したMarketoソリューションのセットアップ {#step-2-of-4-set-up-the-marketo-solution-ropc}

まず、ユーザーアカウントを作成します。

>[!PREREQUISITES]
>
>[手順 1/4:リソース所有者のパスワード制御接続を使用したMarketoソリューションのインストール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)

## 新しいユーザーを作成 {#create-a-new-user}

1. Dynamics にログインします。 設定アイコンをクリックし、「 **詳細設定**.

   ![](assets/one.png)

1. クリック **設定** を選択し、 **セキュリティ**.

   ![](assets/two.png)

1. 「**ユーザー**」をクリックします。

   ![](assets/three.png)

1. クリック **新規：**

   ![](assets/four.png)

1. クリック **ユーザーの追加とライセンス** 新しいウィンドウで

   ![](assets/five.png)

1. 新しいタブが開きます。 クリック **管理者** をクリックします。

   ![](assets/six.png)

1. 別の新しいタブが開きます。 クリック **ユーザーの追加**.

   ![](assets/seven.png)

   >[!IMPORTANT]
   >
   >同期ユーザーには、Marketo設定に対する読み取り権限が必要です。

1. すべての情報を入力します。 完了したら、「 **追加**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >この名前は、既存の CRM ユーザーアカウントではなく、専用の同期ユーザーである必要があります。 実際の電子メールアドレスである必要はありません。

1. 新しいユーザー資格情報を受け取る電子メールアドレスを入力し、「 **メールを送信して閉じる**.

   ![](assets/nine.png)

## 同期ユーザーロールの割り当て {#assign-sync-user-role}

Marketo同期ユーザーの役割をMarketo同期ユーザーにのみ割り当てます。 他のユーザーに割り当てる必要はありません。

>[!NOTE]
>
>これは、Marketoバージョン 4.0.0.14 以降に当てはまります。 以前のバージョンでは、すべてのユーザーに同期ユーザーの役割が必要です。 Marketoをアップグレードするには、 [Microsoft Dynamics 用Marketoソリューションのアップグレード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>同期ユーザーの言語設定 [は英語に設定する必要があります](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. 「有効なユーザー」タブに戻り、ユーザーリストを更新します。

   ![](assets/ten.png)

1. 新しく作成したMarketo同期ユーザーの横にマウスポインターを置くと、チェックボックスが表示されます。 クリックして選択します。

   ![](assets/eleven.png)

1. クリック **役割の管理**.

   ![](assets/twelve.png)

1. チェック **Marketo同期ユーザー** をクリックし、 **OK**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >同期ユーザーが CRM でおこなった更新はすべて次のとおりです **not** をMarketoに同期し直します。

## Marketo Solution の設定 {#configure-marketo-solution}

もう少しです！ あとは、作成した新しいユーザーについてMarketo Solution に知らせるだけです。

1. 「詳細設定」セクションに戻り、 ![](assets/image2015-5-13-15-3a49-3a19.png) [ 設定 ] の横にあるアイコンをクリックし、 **Marketo Config**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >見えない場合 **Marketo Config** 設定メニューで、ページを更新します。 うまくいかない場合は、 [Marketo Solution の公開](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md) 再度ログアウトするか、ログアウトしてから再度ログインします。

1. クリック **デフォルト**.

   ![](assets/fifteen.png)

1. 「 **Marketo User** 「 」フィールドを開き、作成した同期ユーザーを選択します。

   ![](assets/sixteen.png)

1. 次をクリック： ![](assets/image2015-3-13-15-3a10-3a11.png) アイコンを使用して、変更を保存します。

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. 次をクリック： **X** をクリックして画面を閉じます。

   ![](assets/seventeen.png)

1. 次をクリック： ![](assets/image2015-5-13-15-3a49-3a19-1.png) [ 設定 ] の横にあるアイコンをクリックし、 **ソリューション**.

   ![](assets/eighteen.png)

1. 次をクリック： **すべてのカスタマイズを公開** 」ボタンをクリックします。

   ![](assets/nineteen.png)

>[!MORELIKETHIS]
>
>[手順 3/4:Marketoソリューションとリソース所有者のパスワード制御接続の接続](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md)
