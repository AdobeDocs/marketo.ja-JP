---
unique-page-id: 7504744
description: Marketo for Dynamics 2015オンプレムおよび2016 365オンプレムステップ3 / 3 - Marketo Docs — 製品ドキュメントのインストール
title: Marketo for Dynamics 2015オンプレムおよび2016 365オンプレムのインストール手順3/3
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---


# Marketo for Dynamics 2015オンプレムおよび2016 365オンプレムステップ3 / 3 {#install-marketo-for-dynamics-on-prem-and-on-prem-step-of}のインストール

>[!PREREQUISITES]
>
>* [Marketo for Dynamics 2015オンプレムおよび2016 365オンプレムのインストール手順1/3](step-1-of-3-install.md)
>* [Marketo for Dynamics 2015オンプレムおよび2016 365オンプレムのインストール手順2/3](step-2-of-3-set-up.md)

>



>[!NOTE]
>
>**必要な管理者権限**

## Dynamics Syncユーザー情報を入力{#enter-dynamics-sync-user-information}

1. Marketorにログインし、**管理者**&#x200B;をクリックします。

   ![](assets/login-admin.png)

1. 「**CRM**」をクリックします。

   ![](assets/image2015-3-16-9-47-34.png)

1. 「**Microsoft**」を選択します。

   ![](assets/image2015-3-16-9-50-6.png)

1. **手順1の「**&#x200B;編集&#x200B;**」をクリックします。資格情報**&#x200B;を入力します。

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >送信後のスキーマの変更を元に戻すことができないため、資格情報が正しいことを確認してください。 正しくない資格情報を保存した場合は、新しいMarketor購読を取得する必要があります。

1. **ユーザー名**、**パスワード**、Microsoft Dynamics **URL**、およびオプションの&#x200B;**クライアントID**&#x200B;を入力します。 終了したら「**保存**」をクリックします。

   ![](assets/client-id.png)

   >[!NOTE]
   >
   >Marketorのユーザー名は、CRMの同期ユーザーのユーザー名と一致する必要があります。 形式は[`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#8cf9ffe9fecce8e3e1ede5e2a2efe3e1)またはDOMAIN\userです。

   >[!TIP]
   >
   >URLがわからない？ [Dynamics組織サービスのURL](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md)を見つける方法を紹介します。

## 同期するフィールドを選択{#select-fields-to-sync}

1. **手順2:「同期するフィールド**」を選択します。****

   ![](assets/image2015-3-16-9-51-28.png)

1. マーケティング担当者と同期するフィールドを選択して、事前に選択されるようにします。 「**保存**」をクリックします。

   ![](assets/image2016-8-25-15-3a14-3a28.png)

## カスタムフィルターのフィールドを同期{#sync-fields-for-a-custom-filter}

カスタムフィルターを作成した場合は、Marketoと同期する新しいフィールドを必ず入力して選択してください。

1. 管理者に移動し、**Microsoft Dynamics**&#x200B;を選択します。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 「フィールドの同期の詳細」で「**編集**」をクリックします。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. フィールドまで下にスクロールし、チェックします。 実際の名前はnew_synctomktoにする必要がありますが、表示名は任意の名前にすることができます。 「**保存**」をクリックします。

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## 同期を有効にする{#enable-sync}

1. **手順3の**&#x200B;編集&#x200B;**をクリックします。同期**&#x200B;を有効にします。

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketing Toは、Microsoft Dynamicsの同期に対して、またはユーザーを手動で入力した場合に、自動的に重複を排除しません。

1. ポップアップの内容をすべて読み、電子メールを入力し、**開始同期**&#x200B;をクリックします。

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 最初の同期には数時間かかる場合があります。 完了すると、電子メール通知が届きます。

   ![](assets/image2015-3-16-9-59-51.png)

素晴らしい仕事！
