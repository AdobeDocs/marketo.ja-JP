---
description: Microsoft Dynamics 2016／Dynamics 365 オンプレミス向け Marketo インストール手順 3 / 3 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 2016／Dynamics 365 オンプレミス向け Marketo インストール手順 3 / 3
exl-id: ae801a59-8e29-479c-84c5-a18c7511f21f
feature: Microsoft Dynamics
source-git-commit: 2d3264ab75d2327f9226373aad383e7a51508589
workflow-type: ht
source-wordcount: '414'
ht-degree: 100%

---

# 手順 3 / 3：Marketo Dynamics（2016 オンプレミス／Dynamics 365 オンプレミス）の接続 {#step-of-connect-marketo-dynamics-on-premises-2016}

>[!PREREQUISITES]
>
>* [Microsoft Dynamics 2016／Dynamics 365 オンプレミス向け Marketo インストール手順 1 / 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"}
>* [Microsoft Dynamics 2016／Dynamics 365 オンプレミス向け Marketo インストール手順 2 / 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md){target="_blank"}

>[!NOTE]
>
>**管理者権限が必要**

## Dynamics 同期ユーザ情報の入力 {#enter-dynamics-sync-user-information}

1. Marketo にログインし、「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/login-admin.png)

1. 「**[!UICONTROL CRM]**」をクリックします。

   ![](assets/image2015-3-16-9-47-34.png)

1. **[!DNL Microsoft]** を選択します。

   ![](assets/image2015-3-16-9-50-6.png)

1. 「**[!UICONTROL 資格情報を入力]**」で「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >送信後に後続のスキーマの変更を元に戻すことができないので、資格情報が正しいことを確認してください。間違った資格情報を保存した場合は、新しい Marketo サブスクリプションを取得する必要があります。

1. 「**[!UICONTROL ユーザー名]**」、「**[!UICONTROL パスワード]**」と Microsoft Dynamics の「**[!UICONTROL URL]**」、「**クライアント ID／シークレット**」を入力します。終了したら「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* 2020年10月より前に Marketo がプロビジョニングされている場合、「クライアント ID 」と「シークレット」はオプションのフィールドです。それ以外の場合は、必須です。この情報の取得方法は、使用している MSD のバージョンによって異なります。
   >* Marketo のユーザー名は、CRM の同期ユーザーのユーザー名と一致する必要があります。形式は、`user@domain.com` または DOMAIN\user です。
   >* URL がわからない場合は、[こちらで見つける方法をご確認ください](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}。

   >[!TIP]
   >
   >URL がわからない場合は、こちらの [Dynamics 組織サービス URL](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) の検索方法をご覧ください。

## 同期するフィールドを選択 {#select-fields-to-sync}

1. 「**[!UICONTROL 同期するフィールドを選択]**」で「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-3-16-9-51-28.png)

1. Marketo と同期するフィールドを選択すると、事前に選択されるようになります。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2016-8-25-15-3a14-3a28.png)

>[!NOTE]
>
>Marketo は、同期するフィールドへの参照を保存します。Dynamics でフィールドを削除する場合は、[同期無効](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"}の状態で実行することをお勧めします。次に、[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"}を編集および保存して、Marketo のスキーマを更新します。

## カスタムフィルターのフィールドを同期する {#sync-fields-for-a-custom-filter}

カスタムフィルターを作成した場合は、Marketo と同期する新しいフィールドを選択するようにします。

1. 「管理」に移動し、「**[!DNL Microsoft Dynamics]**」を選択します。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 「フィールド同期の詳細」で「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 下にスクロールしてフィールドを確認します。実際の名前は new_synctomkto にする必要がありますが、表示名は任意の名前にすることができます。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## 同期を有効にする {#enable-sync}

1. 「**[!UICONTROL 同期の有効化]**」で「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo は、Microsoft Dynamics の同期や、人物を手動で入力した場合には、自動的に重複排除を行いません。

1. ポップアップの内容をすべて読み、メールアドレスを入力して、「**[!UICONTROL 同期を開始]**」をクリックします。

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. レコードの数によっては、初期同期に数時間から数日かかる場合があります。完了すると、メール通知が届きます。

   ![](assets/image2015-3-16-9-59-51.png)
