---
unique-page-id: 7504744
description: 最後の手順では、MarketoをDynamics 2015 オンプレミスに接続する方法について説明します。 Marketo Adminでsync user credentialsを入力し、syncを有効にします。
title: Microsoft Dynamics 2015 オンプレミス向け Marketo インストール手順 3 / 3
exl-id: 054bf725-7a80-4114-8360-2d86e2e33dd7
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/yOVhPjsnivOpFEkXYcVLy97Upm3yrBipP6NkSjsAw2Q
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 409
ht-degree: 79%

---

# 手順 3／3：Marketo と [!DNL Dynamics]（2015 オンプレミス）の接続 {#step-of-connect-marketo-dynamics-on-premises-2015}

>[!PREREQUISITES]
>
>* [ [!DNL Microsoft Dynamics]  2015 オンプレミス向け Marketo インストール手順 1／3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md)
>* [ [!DNL Microsoft Dynamics]  2015 オンプレミス向け Marketo インストール手順 2／3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2015.md)

>[!NOTE]
>
>**管理者権限が必要**

## [!DNL Dynamics] 同期ユーザ情報の入力 {#enter-dynamics-sync-user-information}

1. Marketo にログインし、**[!UICONTROL 管理]**&#x200B;をクリックします。

   ![](assets/login-admin.png)

1. 「**[!UICONTROL CRM]**」をクリックします。

   ![](assets/image2015-3-16-9-47-34.png)

1. 「**[!UICONTROL Microsoft]**」を選択します。

   ![](assets/image2015-3-16-9-50-6.png)

1. **[!UICONTROL 手順 1：資格情報を入力]**&#x200B;で「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >資格情報が正しいことを確認します。 送信後に後続のスキーマ変更を元に戻すことはできません。 誤った資格情報が保存された場合は、新しいMarketo サブスクリプションが必要になります。

1. **[!UICONTROL ユーザ名]**、**[!UICONTROL パスワード]**、[!DNL Microsoft Dynamics] **URL** および **[!UICONTROL クライアント ID]／[!UICONTROL クライアント秘密鍵]**&#x200B;を入力します。 終了したら「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* 2020年10月より前に Marketo がプロビジョニングされている場合、「クライアント ID 」と「シークレット」はオプションのフィールドです。 それ以外の場合は、必須です。 この情報を取得するには、使用しているMSDのバージョンによって異なります。
   >* Marketo のユーザ名は、CRM の同期ユーザのユーザ名と一致する必要があります。 形式は、`user@domain.com` または DOMAIN\user です。
   >* URL がわからない場合は、[こちらで見つける方法をご確認ください](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}。

   >[!TIP]
   >
   >URL がわからない場合は、 こちらの [Dynamics 組織サービス URL](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"} の検索方法をご覧ください。

## 同期するフィールドの選択 {#select-fields-to-sync}

1. **[!UICONTROL 手順 2：同期するフィールドを選択]**&#x200B;の「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-3-16-9-51-28.png)

1. Marketo と同期するフィールドを選択すると、事前に選択されるようになります。 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2016-8-25-15-3a14-3a28.png)

>[!NOTE]
>
>Marketo は、同期するフィールドへの参照を保存します。 [!DNL Dynamics] でフィールドを削除する場合は、[同期無効](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)の状態で実行することをお勧めします。 次に、「[[!UICONTROL 同期するフィールドを選択]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)」を編集および保存して、Marketo のスキーマを更新します。

## カスタムフィルターのフィールドを同期する {#sync-fields-for-a-custom-filter}

カスタムフィルターを作成した場合は、に移動し、Marketoと同期する新しいフィールドを選択します。

1. 「[!UICONTROL 管理者]」に移動し、「**[!UICONTROL Microsoft Dynamics]**」を選択します。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 「[!UICONTROL フィールド同期の詳細]」で「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 下にスクロールしてフィールドを確認します。 実際の名前は new_synctomkto にする必要がありますが、表示名は任意の名前にすることができます。 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## 同期を有効にする {#enable-sync}

1. **[!UICONTROL 手順 3：同期を有効にする]**&#x200B;の「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo は、[!DNL Microsoft Dynamics] の同期や、人物を手動で入力した場合には、自動的に重複排除を行いません。

1. ポップアップの内容をすべて読み、メールアドレスを入力して、「**[!UICONTROL 同期を開始]**」をクリックします。

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. レコードの数によっては、初期同期に数時間から数日かかる場合があります。 完了すると、メール通知が届きます。

   ![](assets/image2015-3-16-9-59-51.png)
