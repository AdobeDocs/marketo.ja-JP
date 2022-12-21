---
description: 手順 2 / 4 - リソース所有者のパスワード制御接続を使用した Marketo ソリューションの設定 - Marketo ドキュメント - 製品ドキュメント
title: 手順 2 / 4 - リソース所有者のパスワード制御接続を使用した Marketo ソリューションの設定
exl-id: 41c05910-d8e3-4fb7-8f68-17ee10294e57
source-git-commit: 19c568cdc3d31d07e42e99eb7e48f10a017b44f9
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 100%

---

# 手順 2 / 4：リソース所有者のパスワード制御接続を使用した Marketo ソリューションの設定 {#step-2-of-4-set-up-the-marketo-solution-ropc}

まず、ユーザアカウントを作成します。

>[!PREREQUISITES]
>
>[手順 1 / 4：リソース所有者のパスワード制御接続を使用した Marketo ソリューションのインストール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)

## ユーザの新規作成 {#create-a-new-user}

1. Dynamics にログインします。設定アイコンをクリックし、「**詳細設定**」を選択します。

   ![](assets/one.png)

1. 「**設定**」をクリックし、「**セキュリティ**」を選択します。

   ![](assets/two.png)

1. 「**ユーザ**」をクリックします。

   ![](assets/three.png)

1. 「**新規**」をクリックします。

   ![](assets/four.png)

1. 新しいウィンドウで「**ユーザを追加してライセンスを付与**」をクリックします。

   ![](assets/five.png)

1. 新しいタブが開きます。ページの上部にある「**管理**」をクリックします。

   ![](assets/six.png)

1. 別の新しいタブが開きます。「**ユーザを追加**」をクリックします。

   ![](assets/seven.png)

   >[!IMPORTANT]
   >
   >同期ユーザには、Marketo 設定に対する読み取り権限が必要です。

1. すべての情報を入力します。完了したら、「**追加**」をクリックします。

   ![](assets/eight.png)

   >[!NOTE]
   >
   >この名前は、既存の CRM ユーザアカウントではなく、専用の同期ユーザである必要があります。実際の電子メールアドレスである必要はありません。

1. 新しいユーザ認証情報を受け取る電子メールアドレスを入力し、「**メールを送信して閉じる**」をクリックします。

   ![](assets/nine.png)

## 同期ユーザのロールの割り当て {#assign-sync-user-role}

Marketo 同期ユーザロールを Marketo 同期ユーザにのみ割り当てます。他のユーザに割り当てる必要はありません。

>[!NOTE]
>
>これは、Marketo バージョン 4.0.0.14 以降に当てはまります。以前のバージョンでは、すべてのユーザに同期ユーザロールが必要です。Marketo をアップグレードするには、[Microsoft Dynamics 用 Marketo ソリューションのアップグレード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)を参照してください。

>[!IMPORTANT]
>
>同期ユーザの言語設定は[英語に設定する必要](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us)があります。

1. 「有効なユーザ」タブに戻り、ユーザリストを更新します。

   ![](assets/ten.png)

1. 新規作成した Marketo 同期ユーザの横にポインタを合わせると、チェックボックスが表示されます。クリックして選択します。

   ![](assets/eleven.png)

1. 「**ロールを管理**」をクリックします。

   ![](assets/twelve.png)

1. 「**Marketo 同期ユーザ**」のチェックをオンにして、「**OK**」をクリックします。

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >同期ユーザが CRM で行った更新は Marketo に同期&#x200B;**されません**。

## Marketo ソリューションの設定 {#configure-marketo-solution}

もう少しです。あとは、作成した新しいユーザについて Marketo ソルーションに知らせるだけです。

1. 詳細設定セクションに戻り、「設定」の横にある![](assets/image2015-5-13-15-3a49-3a19.png)アイコンをクリックし、「**Marketo 設定**」を選択します。

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >設定メニューで「**Marketo 設定**」が表示されていない場合、ページを更新します。うまくいかない場合は、再度 [Marketo Solution を公開](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)するか、ログアウトしてから再度ログインしてください。

1. 「**デフォルト**」をクリックします。

   ![](assets/fifteen.png)

1. **Marketo ユーザ**&#x200B;フィールドの検索ボタンをクリックして、作成した同期ユーザを選択します。

   ![](assets/sixteen.png)

1. 右下隅にある![](assets/image2015-3-13-15-3a10-3a11.png)アイコンをクリックして、変更を保存します。

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. 右上にある「**X**」をクリックして画面を閉じます。

   ![](assets/seventeen.png)

1. 「設定」の横にある![](assets/image2015-5-13-15-3a49-3a19-1.png)アイコンをクリックし、「**ソリューション**」を選択します。

   ![](assets/eighteen.png)

1. 「**すべてのカスタマイズを公開**」ボタンをクリックします。

   ![](assets/nineteen.png)

>[!MORELIKETHIS]
>
>[手順 3／4：Marketo ソリューションとリソース所有者パスワード制御接続の接続](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md)
