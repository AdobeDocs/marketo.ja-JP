---
description: Microsoft Dynamics 2016/Dynamics 365 オンプレミスステップ 3 / 3 - Marketoドキュメント — 製品ドキュメント
title: Microsoft Dynamics 2016/Dynamics 365 オンプレミスステップ 3/3 のMarketoのインストール
source-git-commit: 7b1f0d0d45bbfe3d8b781282e0a4ef1884a2bf40
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 24%

---

# 手順 3/3:Marketo Dynamics (2016 On Premise/Dynamics 365 On-Premises) に接続 {#step-of-connect-marketo-dynamics-on-premises-2016}

>[!PREREQUISITES]
>
>* [Microsoft Dynamics 2016/Dynamics 365 オンプレミスステップ 1/3 のMarketoのインストール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)
>* [Microsoft Dynamics 2016/Dynamics 365 オンプレミスステップ 2/3 のMarketoのインストール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)


>[!NOTE]
>
>**管理者権限が必要**

## Dynamics 同期ユーザー情報を入力 {#enter-dynamics-sync-user-information}

1. Marketo にログインし、**管理**&#x200B;をクリックします。

   ![](assets/login-admin.png)

1. 「**CRM**」をクリックします。

   ![](assets/image2015-3-16-9-47-34.png)

1. 選択 **Microsoft**.

   ![](assets/image2015-3-16-9-50-6.png)

1. クリック **編集** in **手順 1:資格情報を入力**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >送信後に後続のスキーマの変更を元に戻すことができないので、資格情報が正しいことを確認してください。 間違った資格情報が保存されている場合は、新しいMarketoサブスクリプションを取得する必要があります。

1. 次を入力します。 **ユーザー名**, **パスワード** Microsoft Dynamics **URL**、および **クライアント ID/秘密鍵**. 終了したら「**保存**」をクリックします。

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* 2020 年 10 月より前にMarketoがプロビジョニングされている場合、「クライアント ID 」と「暗号鍵」はオプションのフィールドです。 それ以外の場合は、必須です。 この情報の取得方法は、使用している MSD のバージョンによって異なります。
   >* Marketoのユーザー名は、CRM の同期ユーザーのユーザー名と一致する必要があります。 形式は、 `user@domain.com` または DOMAIN\user.
   >* URL がわからない場合は、 [ここで見つける方法を学ぶ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).


   >[!TIP]
   >
   >URL がわからない場合 お客様の検索方法をご紹介します [Dynamics 組織サービス URL](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) こちら。

## 同期するフィールドの選択 {#select-fields-to-sync}

1. クリック **編集** in **手順 2:同期するフィールドを選択**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Marketoと同期するフィールドを選択し、事前に選択されます。 「**保存**」をクリックします。

   ![](assets/image2016-8-25-15-3a14-3a28.png)

>[!NOTE]
>
>Marketo は、同期するフィールドへの参照を保存します。Dynamics でフィールドを削除する場合は、[同期無効](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)の状態で実行することをお勧めします。次に、[同期するフィールドの選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)を編集および保存して、Marketo のスキーマを更新します。

## カスタムフィルターのフィールドの同期 {#sync-fields-for-a-custom-filter}

カスタムフィルターを作成した場合は、に入り、Marketoと同期する新しいフィールドを選択してください。

1. 管理者に移動し、「 」を選択します。 **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 「フィールド同期の詳細」で「**編集**」をクリックします。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 下にスクロールしてフィールドを確認します。実際の名前は new_synctomkto にする必要がありますが、表示名は任意の名前にすることができます。「**保存**」をクリックします。

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## 同期の有効化 {#enable-sync}

1. クリック **編集** in **手順 3:同期の有効化**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketoは、Microsoft Dynamics の同期に対して、またはユーザーを手動で入力した場合に、自動的に重複を排除しません。

1. ポップアップの内容をすべて読み、メールアドレスを入力して、 **同期を開始**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 最初の同期には数時間かかる場合があります。 完了後、電子メール通知が届きます。

   ![](assets/image2015-3-16-9-59-51.png)

できましたね。
