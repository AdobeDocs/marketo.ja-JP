---
description: Microsoft Dynamics 2016／Dynamics 365 オンプレミス向け Marketo インストール手順 3 / 3 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 2016／Dynamics 365 オンプレミス向け Marketo インストール手順 3 / 3
exl-id: ae801a59-8e29-479c-84c5-a18c7511f21f
source-git-commit: 44cc13361f6ff58d1be388fa0425a6daa63e4c7d
workflow-type: ht
source-wordcount: '390'
ht-degree: 100%

---

# 手順 3 / 3：Marketo Dynamics（2016 オンプレミス／Dynamics 365 オンプレミス）の接続 {#step-of-connect-marketo-dynamics-on-premises-2016}

>[!PREREQUISITES]
>
>* [Microsoft Dynamics 2016／Dynamics 365 オンプレミス向け Marketo インストール手順 1 / 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)
>* [Microsoft Dynamics 2016／Dynamics 365 オンプレミス向け Marketo インストール手順 2 / 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)


>[!NOTE]
>
>**管理者権限が必要**

## Dynamics 同期ユーザー情報を入力する {#enter-dynamics-sync-user-information}

1. Marketo にログインし、「**管理者**」をクリックします。

   ![](assets/login-admin.png)

1. 「**CRM**」をクリックします。

   ![](assets/image2015-3-16-9-47-34.png)

1. 「**Microsoft**」を選択します。

   ![](assets/image2015-3-16-9-50-6.png)

1. **手順 1：資格情報を入力**&#x200B;の「**編集**」をクリックします。

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >送信後に後続のスキーマの変更を元に戻すことができないので、資格情報が正しいことを確認してください。間違った資格情報が保存されている場合は、新しい Marketo サブスクリプションを取得する必要があります。

1. 「**ユーザー名**」、「**パスワード**」と Microsoft Dynamics の「**URL**」、「**クライアント ID／シークレット**」を入力します。終了したら「**保存**」をクリックします。

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* 2020年10月より前に Marketo がプロビジョニングされている場合、「クライアント ID 」と「シークレット」はオプションのフィールドです。それ以外の場合は、必須です。この情報の取得方法は、使用している MSD のバージョンによって異なります。
   >* Marketo のユーザー名は、CRM の同期ユーザーのユーザー名と一致する必要があります。形式は、`user@domain.com` または DOMAIN\user です。
   >* URL がわからない場合は、[こちらで見つける方法をご確認ください](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md)。


   >[!TIP]
   >
   >URL がわからない場合は、こちらの [Dynamics 組織サービス URL](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) の検索方法をご覧ください。

## 同期するフィールドを選択 {#select-fields-to-sync}

1. **手順 2：同期するフィールドを選択**&#x200B;の「**編集**」をクリックします。

   ![](assets/image2015-3-16-9-51-28.png)

1. Marketo と同期するフィールドを選択すると、事前に選択されるようになります。「**保存**」をクリックします。

   ![](assets/image2016-8-25-15-3a14-3a28.png)

>[!NOTE]
>
>Marketo は、同期するフィールドへの参照を保存します。Dynamics でフィールドを削除する場合は、[同期無効](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)の状態で実行することをお勧めします。次に、[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)を編集および保存して、Marketo のスキーマを更新します。

## カスタムフィルターのフィールドを同期する {#sync-fields-for-a-custom-filter}

カスタムフィルターを作成した場合は、Marketo と同期する新しいフィールドを選択するようにします。

1. 「管理者」に移動し、「**Microsoft Dynamics**」を選択します。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 「フィールド同期の詳細」で「**編集**」をクリックします。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 下にスクロールしてフィールドを確認します。実際の名前は new_synctomkto にする必要がありますが、表示名は任意の名前にすることができます。「**保存**」をクリックします。

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## 同期を有効にする {#enable-sync}

1. **手順 3：同期を有効にする**&#x200B;の「**編集**」をクリックします。

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo は、Microsoft Dynamics の同期や、人物を手動で入力した場合には、自動的に重複排除を行いません。

1. ポップアップの内容をすべて読み、メールアドレスを入力して、「**同期を開始**」をクリックします。

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 最初の同期には数時間かかる場合があります。完了後、メール通知が届きます。

   ![](assets/image2015-3-16-9-59-51.png)

これで完了です。
