---
description: 手順 4／4 - Marketo ソリューションとリソース所有者のパスワード制御接続の接続 - Marketo ドキュメント - 製品ドキュメント
title: 手順 4／4 - Marketo ソリューションとリソース所有者のパスワード制御接続の接続
exl-id: 71a52a3e-f31e-45ee-8196-d536528e42ca
source-git-commit: b4fafa28d9a38504a29c25700496d8376c4fe47b
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 手順 4／4：Marketo ソリューションとリソース所有者のパスワード制御接続の接続 {#step-4-of-4-connect-the-marketo-solution-ropc}

これが同期の最後のステップです。もう少しです！

>[!PREREQUISITES]
>
>* [手順 1／4：リソース所有者のパスワード制御接続を使用した Marketo ソリューションのインストール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)
>* [手順 2／4：リソース所有者のパスワード制御接続を使用した Marketo ソリューションの設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)
>* [手順 3 / 4：MS Dynamics でのクライアントアプリのセットアップ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md)


>[!NOTE]
>
>**管理者権限が必要**

>[!IMPORTANT]
>
>基本認証から OAuth にアップグレードする場合は、追加のパラメーターのアップデートについて [Marketo サポート](https://nation.marketo.com/t5/support/ct-p/Support)にお問い合わせください。この機能を有効にすると、新しい認証情報が入力されて同期が再度有効にされるまで、同期が一時的に停止されます。この機能は、古い認証モードに戻る際には（2022 年 4 月まで）無効にすることができます。

## Dynamics 同期ユーザー情報を入力 {#enter-dynamics-sync-user-information}

1. Marketo にログインし、「**管理**」をクリックします。

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

   >[!NOTE]
   >
   >新しい認証情報を入力する前に、[こちらでそれらを検証](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)できます。

1. 次を入力します。 **ユーザー名**, **パスワード**, Microsoft Dynamics **URL**, **クライアント ID**、および **クライアント秘密鍵**. 終了したら「**保存**」をクリックします。

   ![](assets/step-4-of-4-connect-ropc-5.png)

   >[!NOTE]
   >
   >Marketo のユーザー名は、CRM の同期ユーザーのユーザー名と一致する必要があります。形式は、`user@domain.com` または DOMAIN\user です。

## 同期するフィールドの選択 {#select-fields-to-sync}

1. **手順 2：同期するフィールドを選択**&#x200B;で「**編集**」をクリックします。

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Marketo と同期するフィールドを選択すると、事前に選択されるようになります。「**保存**」をクリックします。

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo は、同期するフィールドへの参照を保存します。Dynamics でフィールドを削除する場合は、[同期無効](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)の状態で実行することをお勧めします。次に、[同期するフィールドの選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)を編集および保存して、Marketo のスキーマを更新します。

## カスタムフィルターのフィールドの同期 {#sync-fields-for-a-custom-filter}

カスタムフィルターを作成した場合は、中に入って、Marketo と同期する新しいフィールドを選択してください。

1. 「管理」に移動し、「**MIcrosoft Dynamics**」を選択します。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 「フィールド同期の詳細」で「**編集**」をクリックします。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 下にスクロールしてフィールドを確認します。実際の名前は new_synctomkto にする必要がありますが、表示名は任意の名前にすることができます。「**保存**」をクリックします。

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## 同期の有効化 {#enable-sync}

1. **手順 3：同期の有効化**&#x200B;で「**編集**」をクリックします。

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo は、Microsoft Dynamics の同期や、手動で入力されたリードの場合には、自動的に重複排除をおこないません。

1. ポップアップの内容をすべて読み、メールアドレスを入力して、「**同期を開始**」をクリックします。

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. 初回の同期には数時間かかる場合があります。完了したら、電子メール通知が届きます。

   ![](assets/image2015-3-16-9-3a59-3a51.png)

できましたね。

>[!MORELIKETHIS]
>
>[Dynamics 認証方法の再設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md)