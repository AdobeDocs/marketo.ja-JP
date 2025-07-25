---
description: Marketo for [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 オンプレミスのインストール手順 2/3 - Marketo ドキュメント – 製品ドキュメント
title: Marketo for [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 オンプレミスのインストール手順 2 / 3
exl-id: c789b977-7ada-4f5d-8488-e1b58963f7e3
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 80%

---

# 手順 2/3 Marketo for [!DNL Dynamics] の設定（2016 オンプレミス/[!DNL Dynamics] 365 オンプレミス）{#step-of-set-up-for-marketo-on-premises-2016}

前の手順を完了させたら、先に進みましょう。

>[!PREREQUISITES]
>
>[Marketo for [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 オンプレミスのインストール手順 1/3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## 新規ユーザを作成 {#create-a-new-user}

1. [!DNL Dynamics] にログインします。 「設定」アイコンをクリックし、「詳細設定」を選択します。

   ![](assets/step-2-of-3-marketo-on-premises-2016-1.png)

1. 「**[!UICONTROL 設定]**」を選択し、「**[!UICONTROL セキュリティ]**」を選択します。

   ![](assets/step-2-of-3-marketo-on-premises-2016-2.png)

1. 「**[!UICONTROL ユーザー]**」をクリックします。

   ![](assets/step-2-of-3-marketo-on-premises-2016-3.png)

1. 「**[!UICONTROL 新規]**」をクリックします。

   ![](assets/step-2-of-3-marketo-on-premises-2016-4.png)

1. 「**[!UICONTROL ユーザーの追加とライセンス]**」をクリックします。新しいタブが開きます。

   ![](assets/step-2-of-3-marketo-on-premises-2016-5.png)

1. ページの上部にある「**[!UICONTROL 管理者]**」をクリックします。別の新しいタブが開きます。

   ![](assets/step-2-of-3-marketo-on-premises-2016-6.png)

1. 「**[!UICONTROL ユーザーを追加]**」をクリックします。

   ![](assets/step-2-of-3-marketo-on-premises-2016-7.png)

1. すべての情報を入力します。完了したら、「**[!UICONTROL 追加]**」をクリックします。

   ![](assets/step-2-of-3-marketo-on-premises-2016-8.png)

   >[!NOTE]
   >
   >この名前は、既存の CRM ユーザアカウントではなく、専用の同期ユーザである必要があります。実際のメールアドレスである必要はありません。

1. 新しいユーザー資格情報を受け取るメールアドレスを入力し、「メールを送信して閉じる」をクリックします。

   ![](assets/step-2-of-3-marketo-on-premises-2016-9.png)

## 新しいクライアントアプリケーションを作成する {#create-a-new-client-application}

新しいクライアントアプリケーションを作成し、権限を付与するには、[この Microsoft 記事](https://docs.microsoft.com/ja-jp/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later)の手順に従ってください。[!DNL Dynamics] クライアントアプリケーションのクライアント ID と秘密鍵をメモしておいてください。

## 同期ユーザのロールの割り当て {#assign-sync-user-role}

Marketo 同期ユーザロールを Marketo 同期ユーザにのみ割り当てます。他のユーザに割り当てる必要はありません。

>[!NOTE]
>
>これは、Marketo バージョン 4.0.0.14 以降に適用されます。以前のバージョンでは、すべてのユーザに同期ユーザロールが必要です。Marketoをアップグレードするには、[Marketo ソリューションのアップグレード  [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) を参照してください。

>[!IMPORTANT]
>
>同期ユーザの言語設定は[英語に設定する必要があります](https://learn.microsoft.com/ja-jp/power-platform/admin/enable-languages){target="_blank"}。

1. 「**[!UICONTROL 設定]**」で、「**[!UICONTROL セキュリティ]**」をクリックします。

   ![](assets/assign1.png)

1. 「**[!UICONTROL ユーザ]**」をクリックします。

   ![](assets/assign2.png)

1. ユーザのリストが表示されます。専用の Marketo 同期ユーザを選択するか、[Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"}（ADFS）管理者に問い合わせて、Marketo 専用ユーザの作成を依頼します。

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 同期ユーザを選択します。「**[!UICONTROL ロールを管理]**」をクリックします。

   ![](assets/assign4.png)

1. 「Marketo 同期ユーザ」のチェックをオンにして、「**[!UICONTROL OK]**」をクリックします。

   ![](assets/assign5.png)

   >[!TIP]
   >
   >ロールが表示されない場合は、[手順 1 / 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) に戻ってソリューションをインポートします。

   >[!NOTE]
   >
   >同期ユーザが CRM で行った更新は Marketo に同期&#x200B;_されません_。

## Marketo ソリューションの設定 {#configure-marketo-solution}

あと少しで完了です。次の記事に進む前に、最後の部分を設定しましょう。

1. 「**[!UICONTROL 設定]**」で、「**[!UICONTROL Marketo 設定]**」をクリックします。

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Marketo 設定が見つからない場合は、ページを更新してみてください。問題が解決しない場合は、、[Marketo ソリューションを公開](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"}するか、またはログアウトしてから再度ログインしてみてください。

1. 「**[!UICONTROL デフォルト]**」をクリックします。

   ![](assets/configure2.png)

1. 「**[!UICONTROL Marketo ユーザ]**」フィールドをクリックし、同期ユーザを選択します。

   ![](assets/configure3.png)

1. 右下隅の「保存」アイコンをクリックします。

   ![](assets/configure4.png)

1. 「**[!UICONTROL すべてのカスタマイズを公開]**」をクリックします。

   ![](assets/publish-all-customizations1.png)

## 手順 3 に進む前に {#before-proceeding-to-step}

* 同期するレコード数を制限する場合は、[カスタム同期フィルターを設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)します。
* [Validate [!DNL Microsoft Dynamics] Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) プロセスを実行します。 初期設定が正しく行われたことを確認します。
* [!DNL Microsoft Dynamics] CRM でMarketo同期ユーザーにログインします。

>[!MORELIKETHIS]
>
>[Marketo for [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 オンプレミスのインストール手順 3 / 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
