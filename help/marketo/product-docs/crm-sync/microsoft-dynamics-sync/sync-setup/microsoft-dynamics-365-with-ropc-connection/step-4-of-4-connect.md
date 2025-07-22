---
description: 手順 4 / 4 - Marketo ソリューションとリソース所有者のパスワード制御接続の接続 - Marketo ドキュメント - 製品ドキュメント
title: 手順 4 / 4 - Marketo ソリューションとリソース所有者のパスワード制御接続の接続
exl-id: 71a52a3e-f31e-45ee-8196-d536528e42ca
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 79%

---

# 手順 4 / 4：Marketo ソリューションとリソース所有者のパスワード制御接続の接続 {#step-4-of-4-connect-the-marketo-solution-ropc}

これが同期の最後のステップです。もう少しです！

>[!PREREQUISITES]
>
>* [手順 1 / 4：リソース所有者のパスワード制御接続を使用した Marketo ソリューションのインストール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)
>* [手順 2 / 4：リソース所有者のパスワード制御接続を使用した Marketo ソリューションの設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)
>* [ 手順 3/4:MS でのクライアントアプリのセットアップ  [!DNL Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md)

>[!NOTE]
>
>**管理者権限が必要**

>[!NOTE]
>
>基本認証から [!DNL OAuth] 認証にアップグレードする場合は、[ この記事 ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md) を使用して認証を再設定できます。

## 同期ユーザー情報 [!DNL Dynamics] 入力 {#enter-dynamics-sync-user-information}

1. Marketo にログインし、「**[!UICONTROL 管理]**」をクリックします。

   ![](assets/login-admin.png)

1. 「**[!UICONTROL CRM]**」をクリックします。

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. 「**[!UICONTROL Microsoft]**」を選択します。

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. **[!UICONTROL 手順 1：資格情報を入力]**&#x200B;で「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >送信後に後続のスキーマの変更を元に戻すことができないので、組織 URL が正しいことを確認してください。誤った組織 URL が使用された場合、新しい Marketo サブスクリプションを取得する必要があります。URL がわからない場合は、[こちらで見つける方法をご確認ください](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}。

   >[!NOTE]
   >
   >新しい資格情報を入力する前に、[こちらでそれらを検証](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}できます。

1. **[!UICONTROL ユーザー名]**、**[!UICONTROL パスワード]**、[!DNL Microsoft Dynamics] **[!UICONTROL URL]**、**[!UICONTROL クライアント ID]**、および **[!UICONTROL クライアントシークレット]** を入力します。 終了したら「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/step-4-of-4-connect-ropc-5.png)

   >[!NOTE]
   >
   >Marketo のユーザ名は、CRM の同期ユーザのユーザ名と一致する必要があります。形式は、`user@domain.com` または DOMAIN\user です。

## 同期するフィールドの選択 {#select-fields-to-sync}

1. **[!UICONTROL 手順 2：同期するフィールドを選択]**&#x200B;の「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Marketo と同期するフィールドを選択すると、事前に選択されるようになります。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo は、同期するフィールドへの参照を保存します。[!DNL Dynamics] でフィールドを削除する場合は、[ 同期を無効 ](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md) にして行うことをお勧めします。 次に、[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)を編集および保存して、Marketo のスキーマを更新します。

## カスタムフィルターのフィールドを同期する {#sync-fields-for-a-custom-filter}

カスタムフィルターを作成した場合は、Marketo と同期する新しいフィールドを選択するようにします。

1. [!UICONTROL &#x200B; 管理者 &#x200B;] に移動し、「**[!UICONTROL Microsoft Dynamics]**」を選択します。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. **[!UICONTROL フィールド同期の詳細]** で [!UICONTROL &#x200B; 編集 &#x200B;] をクリックします。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 下にスクロールしてフィールドを確認します。実際の名前は new_synctomkto にする必要がありますが、表示名は任意の名前にすることができます。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## 同期を有効にする {#enable-sync}

1. **[!UICONTROL 手順 3：同期を有効にする]**&#x200B;の「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketoは、[!UICONTROL Microsoft Dynamics] との同期、またはユーザーやリードを手動で入力した場合には、自動的に重複排除を行いません。

1. ポップアップの内容をすべて読み、メールアドレスを入力して、「**[!UICONTROL 同期を開始]**」をクリックします。

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. レコードの数によっては、初期同期に数時間から数日かかる場合があります。完了すると、メール通知が届きます。

   ![](assets/image2015-3-16-9-3a59-3a51.png)

>[!MORELIKETHIS]
>
>[Reconfigure [!DNL Dynamics] Authentication メソッド ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md)
