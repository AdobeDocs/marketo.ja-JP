---
unique-page-id: 3571809
description: 手順3/3 - Microsoft DynamicsとMarketoの接続（2011オンプレミス） - Marketto Docs — 製品ドキュメント
title: 手順3/3 - Microsoft DynamicsとMarketoの接続（2011オンプレミス）
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---


# 手順3/3:Microsoft DynamicsとMarketo （2011オンプレミス）を接続する{#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

よし！ ソリューションをインストールし、同期ユーザーを構成しました。 次に、MarketoとDynamicsを結び付ける必要があります。

>[!PREREQUISITES]
>
>* [手順1/3:Marketo Solution(2011 On-Premises)のインストール](step-1-of-3-install.md)
>* [手順2/3:Dynamics (2011 On-Premises)でMarketo Syncユーザーを設定](step-2-of-3-set-up.md)


>[!NOTE]
>
>**必要な管理者権限**

## Dynamics Syncユーザー情報を入力{#enter-dynamics-sync-user-information}

1. Marketorにログインし、**管理者**&#x200B;をクリックします。

   ![](assets/login-admin.png)

1. **CRM**&#x200B;をクリックします。

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. 「**Microsoft**」をクリックします。

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. **手順1の「**&#x200B;編集&#x200B;**」をクリックします。資格情報を入力してください。**

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >送信後のスキーマの変更を元に戻すことができないため、資格情報が正しいことを確認してください。 正しくない資格情報を保存した場合は、新しいMarketor購読を取得する必要があります。

1. **ユーザー名**、**パスワード**、CRM **URL**&#x200B;を入力し、**保存**&#x200B;をクリックします。

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >Marketorのユーザー名は、CRMの同期ユーザーのユーザー名と一致する必要があります。 形式は[`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#a0d5d3c5d2e0c4cfcdc1c9ce8ec3cfcd)またはDOMAIN\userです。

   >[!TIP]
   >
   >URLがわからない？ [Dynamics組織サービスのURL](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md)を見つける方法をここで示します。

## 同期するフィールドを選択{#select-fields-to-sync}

次に、同期するフィールドを選択する必要があります。

1. ****&#x200B;手順2の&#x200B;**編集をクリックします。同期するフィールドを選択します。**

   ![](assets/image2015-3-16-9-51-28a.png)

1. 事前に選択されたフィールドが同期されます。 必要に応じて追加、「**保存**」をクリックします。

   ![](assets/image2016-8-25-13-3a26-3a14.png)

## カスタムフィルターのフィールドを同期{#sync-fields-for-a-custom-filter}

カスタムフィルターを作成した場合は、Marketoと同期する新しいフィールドを必ず入力して選択してください。

1. 管理者に移動し、**Microsoft Dynamics**&#x200B;を選択します。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 「フィールドの同期の詳細」で「**編集**」をクリックします。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. フィールドまで下にスクロールし、チェックします。 実際の名前はnew_synctomktoにする必要がありますが、表示名は任意の名前にすることができます。 「**保存**」をクリックします。

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## 同期を有効にする{#enable-sync}

1. **手順3の**&#x200B;編集&#x200B;**をクリックします。同期**&#x200B;を有効にします。

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketing Toは、Microsoft Dynamicsの同期に対して、またはユーザーやリードを手動で入力した場合に、自動的に重複を排除しません。

1. ポップアップの内容をすべて読み、電子メールを入力し、**開始同期**&#x200B;をクリックします。

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 最初の同期には数時間かかる場合があります。 完了すると、電子メール通知が届きます。

   ![](assets/image2014-12-11-11-3a55-3a15.png)

   素晴らしい仕事！
