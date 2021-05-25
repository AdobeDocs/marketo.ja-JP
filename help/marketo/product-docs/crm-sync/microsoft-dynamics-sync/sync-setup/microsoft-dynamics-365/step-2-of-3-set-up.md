---
unique-page-id: 3571827
description: 手順2 / 3 - DynamicsでのMarketo Syncユーザーのセットアップ — Marketoドキュメント — 製品ドキュメント
title: 手順2 / 3 - DynamicsでMarketo Syncユーザーを設定
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
source-git-commit: 5473e1a78769ba23e9c3a5926407cf42ef9685a0
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# 手順2 / 3:Dynamics {#step-of-set-up-marketo-sync-user-in-dynamics}でのMarketo同期ユーザーの設定

まず、ユーザーアカウントを作成します。

>[!PREREQUISITES]
[手順1/3:Marketo Solutionのインストール（オンライン）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)>
>

## 新しいユーザー{#create-a-new-user}を作成します。

1. Dynamicsにログインします。 設定アイコンをクリックし、「**詳細設定**」を選択します。

   ![](assets/one.png)

1. 「**設定**」をクリックし、「**セキュリティ**」を選択します。

   ![](assets/two.png)

1. 「**ユーザー**」をクリックします。

   ![](assets/three.png)

1. **新規**&#x200B;をクリックします。

   ![](assets/four.png)

1. 新しいウィンドウで&#x200B;**Add and License Users**&#x200B;をクリックします。

   ![](assets/five.png)

1. 新しいタブが開きます。 ページ上部の「**管理者**」をクリックします。

   ![](assets/six.png)

1. 別の新しいタブが開きます。 「**ユーザーを追加**」をクリックします。

   ![](assets/seven.png)

1. すべての情報を入力します。 完了したら、「**追加**」をクリックします。

   ![](assets/eight.png)

   >[!NOTE]
   この名前は、既存のCRMユーザーのアカウントではなく、専用の同期ユーザーである必要があります。 実際の電子メールアドレスである必要はありません。

1. 新しいユーザー資格情報を受け取る電子メールを入力し、「**電子メールを送信して**&#x200B;を閉じます」をクリックします。

   ![](assets/nine.png)

## 同期ユーザーロール{#assign-sync-user-role}の割り当て

Marketo同期ユーザーの役割をMarketo同期ユーザーにのみ割り当てます。 他のユーザーに割り当てる必要はありません。

>[!NOTE]
これは、Marketoバージョン4.0.0.14以降に適用されます。 以前のバージョンでは、すべてのユーザーに同期ユーザーの役割が必要です。 Marketoをアップグレードするには、[Marketo Solution for Microsoft Dynamicsのアップグレード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)を参照してください。

>[!IMPORTANT]
Sync User [の言語設定は、英語](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us)に設定する必要があります。

1. 「有効なユーザー」タブに戻り、ユーザーのリストを更新します。

   ![](assets/ten.png)

1. 新しく作成されたMarketo Syncユーザーの横にマウスポインターを置くと、チェックボックスが表示されます。 クリックして選択します。

   ![](assets/eleven.png)

1. 「**役割の管理**」をクリックします。

   ![](assets/twelve.png)

1. 「**Marketo同期ユーザー**」をオンにし、「**OK**」をクリックします。

   ![](assets/thirteen.png)

   >[!NOTE]
   同期ユーザーがCRMでおこなった更新は、Marketoに&#x200B;**同期されません**。

## Marketoソリューションの設定{#configure-marketo-solution}

もうすぐ！ ここで必要なのは、作成した新しいユーザーについてMarketo Solutionに知らせることだけです。

1. 「詳細設定」セクションに戻り、「設定」の横の![](assets/image2015-5-13-15-3a49-3a19.png)アイコンをクリックし、「**Marketo Config**」を選択します。

   ![](assets/fourteen.png)

   >[!NOTE]
   設定メニューに&#x200B;**Marketo Config**&#x200B;が表示されない場合は、ページを更新します。 問題が解決しない場合は、[Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)を公開するか、ログアウトしてから再度ログインしてみてください。

1. 「**デフォルト**」をクリックします。

   ![](assets/fifteen.png)

1. 「**Marketoユーザー**」フィールドの検索ボタンをクリックし、作成した同期ユーザーを選択します。

   ![](assets/sixteen.png)

1. 右下隅の![](assets/image2015-3-13-15-3a10-3a11.png)アイコンをクリックして、変更を保存します。

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. 右上の&#x200B;**X**&#x200B;をクリックして、画面を閉じます。

   ![](assets/seventeen.png)

1. 「設定」の横の![](assets/image2015-5-13-15-3a49-3a19-1.png)アイコンをクリックし、「**ソリューション**」を選択します。

   ![](assets/eighteen.png)

1. 「**すべてのカスタマイズを公開**」ボタンをクリックします。

   ![](assets/nineteen.png)

## 手順3に進む前に{#before-proceeding-to-step}

    *同期するレコードの数を制限する場合は、[カスタム同期フィルターを設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)を今すぐお使いください。
    * [Microsoft Dynamics Syncの検証](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)プロセスを実行します。初期設定が正しく行われたことを確認します。
    * Microsoft Dynamics CRMでMarketo同期ユーザーにログインします。

>[!MORELIKETHIS]
[手順3/3:Microsoft DynamicsとMarketoの接続（オンライン）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md)
