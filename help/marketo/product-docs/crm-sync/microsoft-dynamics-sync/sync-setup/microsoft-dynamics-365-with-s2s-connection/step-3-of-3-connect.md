---
unique-page-id: 3571830
description: 手順 3／3 - サーバー間接続を使用した Marketo ソリューションの接続 - Marketo ドキュメント - 製品ドキュメント
title: 手順 3／3 - サーバー間接続を使用した Marketo ソリューションの接続
exl-id: e3ede749-f787-45d3-adb4-f71ef1221208
source-git-commit: 5536b35d71506f11fdf32bf7149bf5c61174ab34
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 92%

---

# 手順 3／3：サーバー間接続を使用した Marketo ソリューションの接続 {#step-3-of-3-connect-microsoft-dynamics-with-marketo-solution-s2s}

これが同期の最後のステップです。もう少しです。

>[!PREREQUISITES]
>
>* [手順 1／3 - サーバー間接続を使用した Marketo ソリューションのインストール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md)
>* [手順 2／3 - サーバー間接続を使用した Marketo ソリューションの設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md)


>[!NOTE]
>
>**管理者権限が必要**

>[!IMPORTANT]
>
>基本認証から OAuth にアップグレードする場合は、追加のパラメーターのアップデートについて [Marketo サポート](https://nation.marketo.com/t5/support/ct-p/Support)にお問い合わせください。この機能を有効にすると、新しい認証情報が入力されて同期が再度有効にされるまで、同期が一時的に停止されます。この機能は、古い認証モードに戻る際には（2022 年 4 月まで）無効にすることができます。

>[!NOTE]
>
>新しい認証情報を入力する前に、[こちらでそれらを検証](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)できます。

## Dynamics 同期ユーザー情報を入力 {#enter-dynamics-sync-user-information}

1. Marketo にログインし、**管理**&#x200B;をクリックします。

   ![](assets/login-admin.png)

1. 「**CRM**」をクリックします。

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. 「**Microsoft**」を選択します。

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. **手順 1:資格情報を入力**&#x200B;で「**編集**」をクリックします。

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >送信後に後続のスキーマの変更を元に戻すことができないので、組織 URL が正しいことを確認してください。誤った組織 URL が使用された場合、新しい Marketo サブスクリプションを取得する必要があります。URL がわからない場合は、[ここで見つける方法を学んでください](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md)。

1. Dynamics 同期ユーザ情報を入力し、 **保存** 完了したら、

   ![](assets/step-3-of-3-connect-s2s-5.png)

   >[!NOTE]
   >
   >Marketoのユーザー名は、 [電子メールアドレス](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) 」と入力します。 形式は、`user@domain.com` または DOMAIN\user です。

## 同期するフィールドの選択 {#select-fields-to-sync}

1. **手順 2：同期するフィールドを選択**&#x200B;の「**編集**」をクリックします。

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Marketo と同期するフィールドを選択すると、事前に選択されるようになります。「**保存**」をクリックします。

   ![](assets/image2016-8-25-15-3a6-3a11.png)

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

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## 同期を有効にする {#enable-sync}

1. **手順 3：同期を有効にする**&#x200B;の「**編集**」をクリックします。

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo は、Microsoft Dynamics の同期や、手動で入力されたリードの場合には、自動的に重複排除をおこないません。

1. ポップアップの内容をすべて読み、メールアドレスを入力して、「**同期を開始**」をクリックします。

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. 初回の同期には数時間かかる場合があります。完了したら、電子メール通知が届きます。

   ![](assets/image2015-3-16-9-3a59-3a51.png)

できましたね。
