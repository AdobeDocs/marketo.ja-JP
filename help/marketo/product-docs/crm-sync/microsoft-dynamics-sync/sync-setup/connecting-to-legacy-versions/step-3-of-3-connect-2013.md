---
unique-page-id: 3571819
description: 手順 3/3 -Marketoと Dynamics の接続（2013 オンプレミス） - Marketoドキュメント — 製品ドキュメント
title: 手順 3/3 -Marketoと Dynamics の接続（2013 オンプレミス）
exl-id: e28f1cc3-ee15-4981-a537-6c4a1682c4c1
source-git-commit: 2568d3414c8aaec882b79442f6312bae3b9514ab
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 30%

---

# 手順 3 / 3：Marketo と Dynamics（2013 オンプレミス）の接続 {#step-of-connect-marketo-and-dynamics-on-premises}

よし！ ソリューションをインストールし、同期ユーザーを設定しました。 次に、Marketoと Dynamics を接続する必要があります。

>[!PREREQUISITES]
>
>* [手順 1 / 3：Dynamics（2013 オンプレミス）での Marketo ソリューションのインストール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)
>* [手順 2 / 3：Marketo（2013 オンプレミス）の同期ユーザーの設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-2-of-3-configure.md)


>[!NOTE]
>
>**管理者権限が必要**

## Dynamics 同期ユーザー情報を入力 {#enter-dynamics-sync-user-information}

1. Marketo にログインし、**管理**&#x200B;をクリックします。

   ![](assets/login-admin.png)

1. クリック **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. 選択 **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. クリック **編集** in **手順 1:資格情報を入力**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >送信後に後続のスキーマの変更を元に戻すことができないので、資格情報が正しいことを確認してください。 間違った資格情報が保存されている場合は、新しいMarketoサブスクリプションを取得する必要があります。

1. 次を入力します。 **ユーザー名**, **パスワード** とMicrosoft Dynamics **URL** 次に、 **保存**.

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >* Marketoのユーザー名は、CRM の同期ユーザーのユーザー名と一致する必要があります。 user@domain.comまたは DOMAIN\user の形式を使用できます。
   >* URL がわからない場合は、 [ここで見つける方法を学ぶ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).


## 同期するフィールドの選択 {#select-fields-to-sync}

次に、同期するフィールドを選択する必要があります。

1. クリック **編集** in **手順 2:同期するフィールドを選択**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Marketoと同期するフィールドを選択し、事前に選択されます。 「**保存**」をクリックします。

   ![](assets/image2016-8-25-15-3a10-3a17.png)

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

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## 同期の有効化 {#enable-sync}

1. クリック **編集** in **手順 3:同期の有効化**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketoは、Microsoft Dynamics の同期に対して、またはユーザーやリードを手動で入力した場合に、自動的に重複を排除しません。

1. ポップアップの内容をすべて読み、メールアドレスを入力して、 **同期を開始**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 最初の同期には数時間かかる場合があります。 完了後、電子メール通知が届きます。

   ![](assets/image2014-12-11-11-3a55-3a15.png)

できましたね。MarketoとMicrosoft Dynamics 間の双方向同期の機能を解放しました。 Marketo Sales Insight を購入済みの場合は、以下をお楽しみいただけます。

>[!MORELIKETHIS]
>
>[Marketo Sales Insight の Microsoft Dynamics 2013 へのインストールと設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)
