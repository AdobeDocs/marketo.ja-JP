---
unique-page-id: 3571819
description: 手順 3 / 3 - Marketo と Dynamics（2013 オンプレミス）の接続 - Marketo ドキュメント - 製品ドキュメント
title: 手順 3 / 3 - Marketo と Dynamics（2013 オンプレミス）の接続
exl-id: e28f1cc3-ee15-4981-a537-6c4a1682c4c1
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 72%

---

# 手順 3/3:Marketoと [!DNL Dynamics] を接続する（2013 オンプレミス） {#step-of-connect-marketo-and-dynamics-on-premises}

これまで、ソリューションをインストールし、同期ユーザーを設定しました。次に、Marketoと [!DNL Dynamics] を接続する必要があります。

>[!PREREQUISITES]
>
>* [ 手順 1/3:Marketo ソリューションを  [!DNL Dynamics]  （2013 オンプレミス）にインストールする ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md)
>* [手順 2 / 3：Marketo（2013 オンプレミス）の同期ユーザーの設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md)

>[!NOTE]
>
>**管理者権限が必要**

## 同期ユーザー情報 [!DNL Dynamics] 入力 {#enter-dynamics-sync-user-information}

1. Marketo にログインし、「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/login-admin.png)

1. 「**[!UICONTROL CRM]**」をクリックします。

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. **[!DNL Microsoft]** を選択します。

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. **[!UICONTROL 手順 1：資格情報を入力]**&#x200B;の「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >送信後に後続のスキーマの変更を元に戻すことができないので、資格情報が正しいことを確認してください。間違った資格情報を保存した場合は、新しい Marketo サブスクリプションを取得する必要があります。

1. **[!UICONTROL ユーザー名]**、**[!UICONTROL パスワード]**、[!DNL Microsoft Dynamics]&#x200B;**URL** を入力し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >* Marketo のユーザ名は、CRM の同期ユーザのユーザ名と一致する必要があります。形式は、`user@domain.com` または DOMAIN\user です。
   >* URL がわからない場合は、[こちらで見つける方法をご確認ください](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}。

## 同期するフィールドを選択 {#select-fields-to-sync}

同期するフィールドを選択する必要があります。

1. **[!UICONTROL 手順 2：同期するフィールドを選択]**&#x200B;の「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Marketo と同期するフィールドを選択すると、事前に選択されるようになります。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2016-8-25-15-3a10-3a17.png)

   >[!NOTE]
   >
   >Marketo は、同期するフィールドへの参照を保存します。[!DNL Dynamics] でフィールドを削除する場合は、[ 同期を無効 ](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md) にして行うことをお勧めします。 次に、[[!UICONTROL 同期するフィールドを選択]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)を編集および保存して、Marketo のスキーマを更新します。

## カスタムフィルターのフィールドを同期する {#sync-fields-for-a-custom-filter}

カスタムフィルターを作成した場合は、Marketo と同期する新しいフィールドを選択するようにします。

1. [!UICONTROL &#x200B; 管理者 &#x200B;] に移動し、「**[!UICONTROL Microsoft Dynamics]**」を選択します。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. **[!UICONTROL フィールド同期の詳細]** で [!UICONTROL &#x200B; 編集 &#x200B;] をクリックします。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 下にスクロールしてフィールドを確認します。実際の名前は new_synctomkto にする必要がありますが、表示名は任意の名前にすることができます。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## 同期を有効にする {#enable-sync}

1. **[!UICONTROL 手順 3：同期を有効にする]**&#x200B;の「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketoは、[!DNL Microsoft Dynamics] ーザー同期や、ユーザーやリードを手動で入力した場合に、自動的に重複排除を行いません。

1. ポップアップの内容をすべて読み、メールアドレスを入力して、「**[!UICONTROL 同期を開始]**」をクリックします。

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. レコードの数によっては、初期同期に数時間から数日かかる場合があります。完了すると、メール通知が届きます。

   ![](assets/image2014-12-11-11-3a55-3a15.png)

できましたね。これで、Marketoと [!DNL Microsoft Dynamics] の間の双方向同期の機能が利用できるようになりました。 [!DNL Marketo Sales Insight] を購入すると、より楽しい体験ができます。

>[!MORELIKETHIS]
>
>[ インストールと設定  [!DNL Marketo Sales Insight] in [!DNL Microsoft Dynamics] 2013](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)
