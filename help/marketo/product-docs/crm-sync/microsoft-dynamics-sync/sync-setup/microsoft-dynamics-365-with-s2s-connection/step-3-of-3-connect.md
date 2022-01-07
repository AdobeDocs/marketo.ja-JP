---
unique-page-id: 3571830
description: 手順 3 / 3 - Marketoソリューションを S2S 接続に接続する — Marketoドキュメント — 製品ドキュメント
title: 手順 3 / 3 - Marketoソリューションを S2S 接続に接続する
exl-id: e3ede749-f787-45d3-adb4-f71ef1221208
source-git-commit: eb200f085b41489c8d7e11bb2fd059a311e5349c
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 手順 3 / 3:Marketoソリューションと S2S 接続の接続 {#step-3-of-3-connect-microsoft-dynamics-with-marketo-solution-s2s}

これが同期の最後のステップです。 もう少しで着く！

>[!PREREQUISITES]
>
>* [手順 1/3:S2S 接続を使用したMarketoソリューションのインストール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md)
>* [手順 2 / 3:S2S 接続を使用したMarketoソリューションのセットアップ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md)


>[!NOTE]
>
>**管理者権限が必要**

>[!IMPORTANT]
>
>基本認証から OAuth にアップグレードする場合は、 [Marketoサポート](https://nation.marketo.com/t5/support/ct-p/Support) を参照してください。 この機能を有効にすると、新しい資格情報が入力され、同期が再度有効になるまで、同期が一時的に停止されます。 この機能は、古い認証モードに戻す際に（2022 年 4 月まで）無効にすることができます。

>[!NOTE]
>
>新しい資格情報を入力する前に、次の操作を実行できます。 [ここでそれらを検証する](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md).

## Dynamics 同期ユーザー情報を入力 {#enter-dynamics-sync-user-information}

1. Marketo にログインし、**管理**&#x200B;をクリックします。

   ![](assets/login-admin.png)

1. クリック **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. 選択 **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. クリック **編集** in **手順 1:資格情報を入力**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >送信後に後続のスキーマの変更を元に戻すことができないので、組織 URL が正しいことを確認してください。 誤った組織 URL が使用されている場合は、新しいMarketoサブスクリプションを取得する必要があります。 URL がわからない場合は、 [ここで見つける方法を学ぶ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

1. 次を入力します。 **ユーザー名**, **パスワード**, **クライアント ID**, **クライアント秘密鍵**、およびMicrosoft Dynamics **URL**. 終了したら「**保存**」をクリックします。

   ![](assets/step-3-of-3-connect-s2s-5.png)

   >[!NOTE]
   >
   >Marketoのユーザー名は、CRM の同期ユーザーのユーザー名と一致する必要があります。 形式は、 `user@domain.com` または DOMAIN\user.

## 同期するフィールドの選択 {#select-fields-to-sync}

1. クリック **編集** in **手順 2:同期するフィールドを選択**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Marketoと同期するフィールドを選択し、事前に選択されます。 「**保存**」をクリックします。

   ![](assets/image2016-8-25-15-3a6-3a11.png)

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

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## 同期の有効化 {#enable-sync}

1. クリック **編集** in **手順 3:同期の有効化**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketoは、Microsoft Dynamics の同期に対して、またはユーザーやリードを手動で入力した場合に、自動的に重複を排除しません。

1. ポップアップの内容をすべて読み、メールアドレスを入力して、 **同期を開始**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. 最初の同期には数時間かかる場合があります。 完了したら、電子メール通知が届きます。

   ![](assets/image2015-3-16-9-3a59-3a51.png)

できましたね。
