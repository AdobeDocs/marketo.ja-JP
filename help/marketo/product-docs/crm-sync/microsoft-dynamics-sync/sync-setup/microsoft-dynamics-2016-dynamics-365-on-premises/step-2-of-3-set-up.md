---
description: Microsoft Dynamics 2016/Dynamics 365 オンプレミスステップ 2 / 3 - Marketoドキュメント — 製品ドキュメント
title: Microsoft Dynamics 2016/Dynamics 365 オンプレミスステップ 2/3 のMarketoのインストール
exl-id: c789b977-7ada-4f5d-8488-e1b58963f7e3
source-git-commit: 3fb93520a653109845c3b40aba20304c6163214f
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 2%

---

# 手順 2 / 3 Dynamics 用のMarketoのセットアップ (2016 On-Premis/Dynamics 365 On-Premises){#step-of-set-up-for-marketo-on-premises-2016}

前の手順を完了した優れたジョブ。 これからも続けていきましょう

>[!PREREQUISITES]
>
>[Microsoft Dynamics 2016/Dynamics 365 オンプレミスステップ 1/3 のMarketoのインストール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## 新しいユーザーの作成 {#create-a-new-user}

1. Dynamics にログインします。 設定アイコンをクリックし、「詳細設定」を選択します。

   ![](assets/step-2-of-3-marketo-on-premises-2016-1.png)

1. クリック **設定** を選択し、 **セキュリティ**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-2.png)

1. 「**ユーザー**」をクリックします。

   ![](assets/step-2-of-3-marketo-on-premises-2016-3.png)

1. 「**新規**」をクリックします。

   ![](assets/step-2-of-3-marketo-on-premises-2016-4.png)

1. クリック **ユーザーの追加とライセンス**. 新しいタブが開きます。

   ![](assets/step-2-of-3-marketo-on-premises-2016-5.png)

1. クリック **管理者** をクリックします。 別の新しいタブが開きます。

   ![](assets/step-2-of-3-marketo-on-premises-2016-6.png)

1. クリック **ユーザーの追加**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-7.png)

1. すべての情報を入力します。 完了したら、「 **追加**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-8.png)

   >[!NOTE]
   >
   >この名前は、既存の CRM ユーザーアカウントではなく、専用の同期ユーザーである必要があります。 実際の電子メールアドレスである必要はありません。

1. 新しいユーザー資格情報を受け取る電子メールアドレスを入力し、「電子メールを送信して閉じる」をクリックします。

   ![](assets/step-2-of-3-marketo-on-premises-2016-9.png)

## 新しいクライアントアプリケーションを作成 {#create-a-new-client-application}

詳しくは、 [このMicrosoft記事](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later) をクリックして、新しいクライアントアプリケーションを作成し、権限を付与します。 Dynamics クライアントアプリケーションのクライアント ID/シークレットをメモしておいてください。

## 同期ユーザーロールの割り当て {#assign-sync-user-role}

Marketo同期ユーザーの役割をMarketo同期ユーザーにのみ割り当てます。 他のユーザーに割り当てる必要はありません。

>[!NOTE]
>
>これは、Marketoバージョン 4.0.0.14 以降に当てはまります。 以前のバージョンでは、すべてのユーザーに同期ユーザーの役割が必要です。 Marketoをアップグレードするには、 [Microsoft Dynamics 用Marketoソリューションのアップグレード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>同期ユーザーの言語設定 [は英語に設定する必要があります](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. の下 **設定**&#x200B;をクリックし、 **セキュリティ**.

   ![](assets/assign1.png)

1. 「**ユーザー**」をクリックします。

   ![](assets/assign2.png)

1. ユーザーのリストがここに表示されます。 専用のMarketo Sync ユーザーを選択するか、 [Active Directory フェデレーションサービス](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS) 管理者：Marketo専用のユーザーを作成します。

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 同期ユーザーを選択します。 クリック **役割の管理**.

   ![](assets/assign4.png)

   「 Marketo Sync User 」をオンにし、「 OK 」をクリックします。

   ![](assets/assign5.png)

   >[!TIP]
   >
   >の役割が表示されない場合は、に戻ります。 [手順 1 / 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) ソリューションを読み込みます。

   >[!NOTE]
   >
   >同期ユーザーが CRM でおこなった更新はすべて次のとおりです **not** をMarketoに同期し直します。

## Marketo Solution の設定 {#configure-marketo-solution}

ほぼ完了です！ 次の記事に進む前に、設定の最後の部分をいくつか用意します。

1. 「**設定**」で、「**Marketo 設定**」をクリックします。

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Marketo Config が見つからない場合は、ページを更新してみてください。 問題が解決しない場合は、 [Marketo Solution の公開](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) または、ログアウトしてから再度ログインしてみてください。

1. クリック **デフォルト**.

   ![](assets/configure2.png)

1. 次をクリック： **Marketo User** 「 」フィールドをクリックし、同期ユーザーを選択します。

   ![](assets/configure3.png)

1. 右下隅の保存アイコンをクリックします。

   ![](assets/configure4.png)

1. クリック **すべてのカスタマイズを公開**.

   ![](assets/publish-all-customizations1.png)

## 手順 3 に進む前に {#before-proceeding-to-step}

* 同期するレコード数を制限する場合は、 [カスタム同期フィルターの設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 今すぐ。
* を実行します。 [Microsoft Dynamics 同期の検証](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) プロセス。 初期設定が正しく行われたことを確認します。
* Microsoft Dynamics CRM でMarketo同期ユーザーにログインします。

>[!MORELIKETHIS]
>
>[Microsoft Dynamics 2016/Dynamics 365 オンプレミスステップ 3/3 のMarketoのインストール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
