---
unique-page-id: 3571830
description: 手順3/3 - Microsoft DynamicsとMarketoの接続（オンライン） - Marketto Docs — 製品ドキュメント
title: 手順3/3 - Microsoft DynamicsとMarketoの接続（オンライン）
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---


# 手順3/3:Microsoft DynamicsとMarketoの接続（オンライン） {#step-of-connect-microsoft-dynamics-with-marketo-online}

これが同期の最後のステップです。 もう少しで着く！

>[!PREREQUISITES]
>
>* [手順1/3:Marketor Solutionのインストール（オンライン）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)
>* [手順2/3:DynamicsでのMarket Syncユーザーの設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)


>[!NOTE]
>
>**必要な管理者権限**

## Dynamics Syncユーザー情報を入力{#enter-dynamics-sync-user-information}

1. Marketorにログインし、**管理者**&#x200B;をクリックします。

   ![](assets/login-admin.png)

1. **CRM**&#x200B;をクリックします。

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. 「**Microsoft**」を選択します。

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. **手順1の「**&#x200B;編集&#x200B;**」をクリックします。資格情報**&#x200B;を入力します。

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >送信後のスキーマの変更を元に戻すことができないため、資格情報が正しいことを確認してください。 正しくない資格情報を保存した場合は、新しいMarketor購読を取得する必要があります。

1. **ユーザー名**、**パスワード**、Microsoft Dynamics **URL**&#x200B;を入力します。 終了したら「**保存**」をクリックします。

   ![](assets/five-1.png)

   >[!NOTE]
   >
   >* 2020年10月より前にマーケティング担当者がプロビジョニングされていた場合、「クライアントID」と「シークレット」はオプションのフィールドです。 それ以外の場合は、必須です。 この情報の取得は、使用しているMSDのバージョンによって異なります。
   >* Marketorのユーザー名は、CRMの同期ユーザーのユーザー名と一致する必要があります。 `user@domain.com`またはDOMAIN\userの形式を使用できます。
   >* URLがわからない場合は、[URLを見つける方法を](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md)に学びます。


## 同期するフィールドを選択{#select-fields-to-sync}

1. **手順2:「同期するフィールド**」を選択します。****

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. マーケティング担当者と同期するフィールドを選択して、事前に選択されるようにします。 「**保存**」をクリックします。

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketorは、同期するフィールドへの参照を保存します。 Dynamicsでフィールドを削除する場合は、[同期が無効](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)の状態で削除することをお勧めします。 次に、[同期するフィールドの選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)を編集して保存し、Marketorのスキーマを更新します。

## カスタムフィルターのフィールドを同期{#sync-fields-for-a-custom-filter}

カスタムフィルターを作成した場合は、Marketoと同期する新しいフィールドを必ず入力して選択してください。

1. 管理者に移動し、**Microsoft Dynamics**&#x200B;を選択します。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 「フィールドの同期の詳細」で「**編集**」をクリックします。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. フィールドまで下にスクロールし、チェックします。 実際の名前はnew_synctomktoにする必要がありますが、表示名は任意の名前にすることができます。 「**保存**」をクリックします。

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## 同期を有効にする{#enable-sync}

1. **手順3の**&#x200B;編集&#x200B;**をクリックします。同期**&#x200B;を有効にします。

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketing Toは、Microsoft Dynamicsの同期に対して、またはユーザーやリードを手動で入力した場合に、自動的に重複を排除しません。

1. ポップアップの内容をすべて読み、電子メールアドレスを入力し、**開始同期**&#x200B;をクリックします。

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. 最初の同期には数時間かかる場合があります。 完了すると、電子メール通知が届きます。

   ![](assets/image2015-3-16-9-3a59-3a51.png)

素晴らしい仕事！
