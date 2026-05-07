---
unique-page-id: 3571809
description: 最後のステップでは、Microsoft Dynamics 2011 オンプレミスをMarketoに接続する方法について説明します。 Marketo Adminにユーザー情報を同期を入力し、同期を有効にします。
title: 手順 3／3 -  [!DNL Microsoft Dynamics]  と Marketo（2011 オンプレミス）の接続
exl-id: e6a5d49d-025a-4899-9e92-7a4c32086c67
feature: Microsoft Dynamics
source-git-commit: d20c398cd1f5ed2646f56995c35a57630c3f2e95
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 76%

---

# 手順 3／3 - [!DNL Microsoft Dynamics] と Marketo（2011 オンプレミス）の接続 {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

ソリューションがインストールされ、同期ユーザーが設定されます。 次に、Marketoと[!DNL Dynamics]を接続します。

>[!PREREQUISITES]
>
>* [手順 1／3：Marketo ソリューション（2011 オンプレミス版）のインストール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md)
>* [手順 2／3： [!DNL Dynamics] （2011 オンプレミス）での Marketo 同期ユーザの設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md)

>[!NOTE]
>
>**管理者権限が必要**

## [!DNL Dynamics] 同期ユーザ情報の入力 {#enter-dynamics-sync-user-information}

1. Marketo にログインし、**[!UICONTROL 管理]**&#x200B;をクリックします。

   ![](assets/login-admin.png)

1. 「**[!UICONTROL CRM]**」をクリックします。

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. 「**[!UICONTROL Microsoft]**」をクリックします。

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. **[!UICONTROL 手順 1：資格情報を入力]**&#x200B;で「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >資格情報が正しいことを確認します。 送信後に後続のスキーマ変更を元に戻すことはできません。 誤った資格情報が保存された場合は、新しいMarketo サブスクリプションが必要になります。

1. 「**[!UICONTROL ユーザ名]**」、「**[!UICONTROL パスワード]**」と CRM の「**[!UICONTROL URL]**」を入力し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >* Marketo の[!UICONTROL ユーザ名]は、CRM の同期ユーザのユーザ名と一致する必要があります。 形式は、`user@domain.com` または DOMAIN\user です。
   >* URL がわからない場合は、[こちらで見つける方法をご確認ください](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md)。

## 同期するフィールドを選択 {#select-fields-to-sync}

同期するフィールドを選択します。

1. **[!UICONTROL 手順 2：同期するフィールドを選択]**&#x200B;の「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-3-16-9-51-28a.png)

1. 同期されるフィールドは事前に選択されています。 必要に応じて追加し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2016-8-25-13-3a26-3a14.png)

   >[!NOTE]
   >
   >Marketo は、同期するフィールドへの参照を保存します。 [!DNL Dynamics] でフィールドを削除する場合は、[同期無効](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)の状態で実行することをお勧めします。 次に、「[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)」を編集および保存して、Marketo のスキーマを更新します。

## カスタムフィルターのフィールドを同期する {#sync-fields-for-a-custom-filter}

カスタムフィルターを作成した場合は、に移動し、Marketoと同期する新しいフィールドを選択します。

1. 「管理者」に移動し、「**[!UICONTROL Microsoft Dynamics]**」を選択します。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 「[!UICONTROL フィールド同期の詳細]」で「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 下にスクロールしてフィールドを確認します。 実際の名前は new_synctomkto にする必要がありますが、表示名は任意の名前にすることができます。 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## 同期を有効にする {#enable-sync}

1. **[!UICONTROL 手順 3：同期を有効にする]**&#x200B;の「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo は、[!DNL Microsoft Dynamics] の同期に対して、または人物やリードを手動で入力した場合には、自動的に重複排除を行いません。

1. ポップアップの内容をすべて読み、メールアドレスを入力して、「**[!UICONTROL 同期を開始]**」をクリックします。

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. レコードの数によっては、初期同期に数時間から数日かかる場合があります。 完了すると、メール通知が届きます。

   ![](assets/image2014-12-11-11-3a55-3a15.png)
