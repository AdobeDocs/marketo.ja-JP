---
unique-page-id: 3571827
description: 手順2 / 3 - Dynamics - Marketto Docs — 製品ドキュメントでのユーザー同期の設定
title: 手順2/3 - DynamicsでのMarketo Syncユーザーの設定
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---


# 手順2/3:Dynamics {#step-of-set-up-marketo-sync-user-in-dynamics}でMarket Syncユーザーを設定

まず、ユーザーアカウントを作成します。

>[!PREREQUISITES]
>
>[手順1/3:Marketor Solutionのインストール（オンライン）](step-1-of-3-install.md)

## 新しいユーザーの作成{#create-a-new-user}

1. Dynamicsにログインします。 設定アイコンをクリックし、「**詳細設定**」を選択します。

   ![](assets/one.png)

1. 「**設定**」をクリックし、「**セキュリティ**」を選択します。

   ![](assets/two.png)

1. 「**ユーザー**」をクリックします。

   ![](assets/three.png)

1. 「**新規作成」をクリックします。**

   ![](assets/four.png)

1. 新しいウィンドウで&#x200B;**追加およびライセンスユーザー**&#x200B;をクリックします。

   ![](assets/five.png)

1. 新しいタブが開きます。 ページ上部の「**管理者**」をクリックします。

   ![](assets/six.png)

1. 別の新しいタブが開きます。 **追加ユーザー**&#x200B;をクリックします。

   ![](assets/seven.png)

1. すべての情報を入力します。 終了したら、**追加**&#x200B;をクリックします。

   ![](assets/eight.png)

   >[!NOTE]
   >
   >この名前は、既存のCRMユーザーのアカウントではなく、専用の同期ユーザーである必要があります。 実際の電子メールアドレスである必要はありません。

1. 新しいユーザー資格情報を受け取る電子メールを入力し、「**電子メールを送信して**&#x200B;を閉じます」をクリックします。

   ![](assets/nine.png)

## 同期ユーザーロールの割り当て{#assign-sync-user-role}

Marketor SyncユーザーロールをMarketor Syncユーザーにのみ割り当てます。 他のユーザーに割り当てる必要はありません。

>[!NOTE]
>
>これは、Marketoバージョン4.0.0.14以降に適用されます。 以前のバージョンでは、すべてのユーザーに同期ユーザーの役割が必要です。 Marketorをアップグレードするには、[Microsoft Dynamics用Marketing Solutionのアップグレード](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md)を参照してください。

1. 「有効なユーザー」タブに戻り、ユーザーリストを更新します。

   ![](assets/ten.png)

1. 新しく作成されたMarketo Syncユーザーの横にマウスポインターを置くと、チェックボックスが表示されます。 クリックして選択します。

   ![](assets/eleven.png)

1. 「**ロールの管理**」をクリックします。

   ![](assets/twelve.png)

1. 「**ユーザーを同期するマーケティングツール**」を選択し、「**OK**」をクリックします。

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >同期ユーザーがCRMで行った更新は、Marketoに&#x200B;**同期**&#x200B;されません。

## Marketto Solutionの設定{#configure-marketo-solution}

もう少しで！ 後は、新しく作成したユーザーについてマーケティング担当者に知らせるだけです。

1. 「詳細設定」セクションに戻り、「設定」の横の![](assets/image2015-5-13-15-3a49-3a19.png)アイコンをクリックし、「**Marketto Config**」を選択します。

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >設定メニューに&#x200B;**Marketto Config**&#x200B;が表示されない場合は、ページを更新します。 問題が解決しない場合は、[Marketo Solution](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) [](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations)を再度公開するか、ログアウトしてから再度ログインしてみてください。

1. 「**デフォルト**」をクリックします。

   ![](assets/fifteen.png)

1. 「**Marketto User**」フィールドの検索ボタンをクリックし、作成した同期ユーザーを選択します。

   ![](assets/sixteen.png)

1. 右下の![](assets/image2015-3-13-15-3a10-3a11.png)アイコンをクリックして、変更を保存します。

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. 右上の&#x200B;**X**&#x200B;をクリックして、画面を閉じます。

   ![](assets/seventeen.png)

1. 「設定」の横の![](assets/image2015-5-13-15-3a49-3a19-1.png)アイコンをクリックし、「**ソリューション**」を選択します。

   ![](assets/eighteen.png)

1. 「**すべてのカスタマイズを発行**」ボタンをクリックします。

   ![](assets/nineteen.png)

## 手順3に進む前に{#before-proceeding-to-step}

    *同期するレコードの数を制限する場合は、[カスタム同期フィルタを設定](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)を今すぐ行ってください。
    * [Microsoft Dynamics Syncの検証](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)プロセスを実行します。初期設定が正しく行われたことを確認できます。
    * Microsoft Dynamics CRMのMarketto Sync Userにログインします。

>[!NOTE]
>
>**関連記事**
>
>
>[手順3/3:Microsoft DynamicsとMarketoの接続（オンライン）](step-3-of-3-connect.md)
