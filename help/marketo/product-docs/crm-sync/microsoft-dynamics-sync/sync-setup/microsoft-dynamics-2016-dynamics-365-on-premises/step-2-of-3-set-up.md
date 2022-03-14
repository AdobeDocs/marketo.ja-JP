---
description: Microsoft Dynamics 2016／Dynamics 365 オンプレミス向け Marketo インストール手順 2 / 3 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 2016／Dynamics 365 オンプレミス向け Marketo インストール手順 2 / 3
exl-id: c789b977-7ada-4f5d-8488-e1b58963f7e3
source-git-commit: 3fb93520a653109845c3b40aba20304c6163214f
workflow-type: ht
source-wordcount: '492'
ht-degree: 100%

---

# 手順 2 / 3 Dynamics（2016 オンプレミス／Dynamics 365 オンプレミス）向け Marketo の設定{#step-of-set-up-for-marketo-on-premises-2016}

前の手順を完了させたら、先に進みましょう。

>[!PREREQUISITES]
>
>[Microsoft Dynamics 2016／Dynamics 365 オンプレミス向け Marketo インストール手順 1 / 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## ユーザーを新規作成する {#create-a-new-user}

1. Dynamics にログインします。「設定」アイコンをクリックし、「詳細設定」を選択します。

   ![](assets/step-2-of-3-marketo-on-premises-2016-1.png)

1. 「**設定**」を選択し、「**セキュリティ**」を選択します。

   ![](assets/step-2-of-3-marketo-on-premises-2016-2.png)

1. 「**ユーザー**」をクリックします。

   ![](assets/step-2-of-3-marketo-on-premises-2016-3.png)

1. 「**新規**」をクリックします。

   ![](assets/step-2-of-3-marketo-on-premises-2016-4.png)

1. 「**ユーザーの追加とライセンス**」をクリックします。新しいタブが開きます。

   ![](assets/step-2-of-3-marketo-on-premises-2016-5.png)

1. ページの上部にある「**管理者**」をクリックします。別の新しいタブが開きます。

   ![](assets/step-2-of-3-marketo-on-premises-2016-6.png)

1. 「**ユーザーを追加**」をクリックします。

   ![](assets/step-2-of-3-marketo-on-premises-2016-7.png)

1. すべての情報を入力します。完了したら、「**追加**」をクリックします。

   ![](assets/step-2-of-3-marketo-on-premises-2016-8.png)

   >[!NOTE]
   >
   >この名前は、既存の CRM ユーザーアカウントではなく、専用の同期ユーザーである必要があります。実際のメールアドレスである必要はありません。

1. 新しいユーザー資格情報を受け取るメールアドレスを入力し、「メールを送信して閉じる」をクリックします。

   ![](assets/step-2-of-3-marketo-on-premises-2016-9.png)

## 新しいクライアントアプリケーションを作成する {#create-a-new-client-application}

新しいクライアントアプリケーションを作成し、権限を付与するには、[この Microsoft 記事](https://docs.microsoft.com/ja-jp/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later)の手順に従ってください。Dynamics クライアントアプリケーションのクライアント ID／シークレットをメモしておいてください。

## 同期ユーザー役割を割り当てる {#assign-sync-user-role}

Marketo 同期ユーザー役割を Marketo 同期ユーザーにのみ割り当てます。他のユーザーに割り当てる必要はありません。

>[!NOTE]
>
>これは、Marketo バージョン 4.0.0.14 以降に当てはまります。以前のバージョンでは、すべてのユーザーに同期ユーザー役割が必要です。お使いの Marketo をアップグレードするには、[Microsoft Dynamics 用 Marketo ソリューションのアップグレード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)を参照してください。

>[!IMPORTANT]
>
>同期ユーザーの言語設定は[英語に設定する必要があります](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us)。

1. 「**設定**」で、「**セキュリティ**」をクリックします。

   ![](assets/assign1.png)

1. 「**ユーザー**」をクリックします。

   ![](assets/assign2.png)

1. ユーザーのリストが表示されます。専用の Marketo 同期ユーザーを選択するか、[Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx)（ADFS）管理者に問い合わせて、Marketo 専用ユーザーの作成を依頼します。

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 同期ユーザーを選択します。「**役割を管理**」をクリックします。

   ![](assets/assign4.png)

   「Marketo 同期ユーザー」をクリックし、「OK」をクリックします。

   ![](assets/assign5.png)

   >[!TIP]
   >
   >役割が表示されない場合は、[手順 1 / 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) に戻ってソリューションをインポートします。

   >[!NOTE]
   >
   >同期ユーザーが CRM で実行した更新は、再度 Marketo に&#x200B;**同期されません**。

## Marketo ソリューションを設定する {#configure-marketo-solution}

あと少しで完了です。次の記事に進む前に、最後の部分を設定しましょう。

1. 「**設定**」で、「**Marketo 設定**」をクリックします。

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Marketo 設定が見つからない場合は、ページを更新してみてください。問題が解決しない場合は、、[Marketo ソリューションを公開](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)するか、またはログアウトしてから再度ログインしてみてください。

1. 「**デフォルト**」をクリックします。

   ![](assets/configure2.png)

1. 「**Marketo ユーザー**」フィールドをクリックし、同期ユーザーを選択します。

   ![](assets/configure3.png)

1. 右下隅の「保存」アイコンをクリックします。

   ![](assets/configure4.png)

1. 「**すべてのカスタマイズを公開**」をクリックします。

   ![](assets/publish-all-customizations1.png)

## 手順 3 に進む前に {#before-proceeding-to-step}

* 同期するレコード数を制限する場合は、[カスタム同期フィルターを設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)します。
* [Microsoft Dynamics 同期を検証](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)プロセスを実行します。初期設定が正しく行われたことを確認します。
* Microsoft Dynamics CRM で、Marketo 同期ユーザーにログインします。

>[!MORELIKETHIS]
>
>[Microsoft Dynamics 2016／Dynamics 365 オンプレミス向け Marketo インストール手順 3 / 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
