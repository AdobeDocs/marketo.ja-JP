---
unique-page-id: 3571819
description: 手順 3 / 3 - Marketo と Dynamics（2013 オンプレミス）の接続 - Marketo ドキュメント - 製品ドキュメント
title: 手順 3 / 3 - Marketo と Dynamics（2013 オンプレミス）の接続
exl-id: e28f1cc3-ee15-4981-a537-6c4a1682c4c1
source-git-commit: f130fa1187ccead6573f76ff947e55d42f6962e4
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 100%

---

# 手順 3 / 3：Marketo と Dynamics（2013 オンプレミス）の接続 {#step-of-connect-marketo-and-dynamics-on-premises}

これまで、ソリューションをインストールし、同期ユーザーを設定しました。次に、Marketo と Dynamics を接続する必要があります。

>[!PREREQUISITES]
>
>* [手順 1 / 3：Dynamics（2013 オンプレミス）での Marketo ソリューションのインストール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md)
>* [手順 2 / 3：Marketo（2013 オンプレミス）の同期ユーザーの設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md)


>[!NOTE]
>
>**管理者権限が必要**

## Dynamics 同期ユーザー情報を入力する {#enter-dynamics-sync-user-information}

1. Marketo にログインし、「**管理者**」をクリックします。

   ![](assets/login-admin.png)

1. 「**CRM**」をクリックします。

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. 「**Microsoft**」を選択します。

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. **手順 1：資格情報を入力**&#x200B;の「**編集**」をクリックします。

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >送信後に後続のスキーマの変更を元に戻すことができないので、資格情報が正しいことを確認してください。間違った資格情報が保存されている場合は、新しい Marketo サブスクリプションを取得する必要があります。

1. 「**ユーザー名**」、「**パスワード**」と Microsoft Dynamics の「**URL**」を入力し、「**保存**」をクリックします。

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >* Marketo のユーザー名は、CRM の同期ユーザーのユーザー名と一致する必要があります。形式は、user@domain.com または DOMAIN\user です。
   >* URL がわからない場合は、[こちらで見つける方法をご確認ください](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md)。


## 同期するフィールドを選択 {#select-fields-to-sync}

同期するフィールドを選択する必要があります。

1. **手順 2：同期するフィールドを選択**&#x200B;の「**編集**」をクリックします。

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Marketo と同期するフィールドを選択すると、事前に選択されるようになります。「**保存**」をクリックします。

   ![](assets/image2016-8-25-15-3a10-3a17.png)

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

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## 同期を有効にする {#enable-sync}

1. **手順 3：同期を有効にする**&#x200B;の「**編集**」をクリックします。

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo は、Microsoft Dynamics の同期や、人物やリードを手動で入力した場合には、自動的に重複排除を行いません。

1. ポップアップの内容をすべて読み、メールアドレスを入力して、「**同期を開始**」をクリックします。

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 最初の同期には数時間かかる場合があります。完了後、メール通知が届きます。

   ![](assets/image2014-12-11-11-3a55-3a15.png)

できましたね。Marketo と Microsoft Dynamics 間の双方向同期の機能を解放しました。Marketo Sales Insight を購入済みの場合は、以下を参照してください。

>[!MORELIKETHIS]
>
>[Marketo Sales Insight の Microsoft Dynamics 2013 へのインストールと設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)
