---
unique-page-id: 3571809
description: 手順3/3 - Microsoft DynamicsとMarketoの接続（2011オンプレミス） - Marketto Docs — 製品ドキュメント
title: 手順3/3 - Microsoft DynamicsとMarketoの接続（2011オンプレミス）
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---


# 手順3/3:Microsoft DynamicsとMarketoの接続（2011オンプレミス） {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

>[!NOTE]
>
>**FYI**
>
>Marketoは現在、すべての購読で言語を標準化しているので、購読およびdocs.marketo.comの人物/人物にリード/リードを表示できます。 これらの用語は同じことを意味し、記事の説明には影響しません。 他にも変化がある。 [詳細情報](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

よし！ ソリューションをインストールし、同期ユーザーを構成しました。 次に、MarketoとDynamicsを結び付ける必要があります。

>[!PREREQUISITES]
>
>* [手順1/3:Marketo Solution(2011 On-Premises)のインストール](step-1-of-3-install.md)
>* [手順2/3:Dynamics (2011 On-Premises)でMarketo Syncユーザーを設定](step-2-of-3-set-up.md)


>[!NOTE]
>
>**必要な管理者権限**

## Dynamics Syncユーザー情報の入力 {#enter-dynamics-sync-user-information}

1. Marketorにログインし、「 **管理者**」をクリックします。

   ![](assets/login-admin.png)

1. 「 **CRM**」をクリックします。

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. 「 **Microsoft**」をクリックします。

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. **手順1で****「編集」をクリックします。資格情報を入力します。**

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >送信後のスキーマの変更を元に戻すことができないため、資格情報が正しいことを確認してください。 正しくない資格情報を保存した場合は、新しいMarketor購読を取得する必要があります。

1. ユー **ザー名**、 **パスワード** 、CRM **URLを入力し、「******&#x200B;保存」をクリックします。

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >Marketorのユーザー名は、CRMの同期ユーザーのユーザー名と一致する必要があります。 形式は、DOMAIN\user [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#a0d5d3c5d2e0c4cfcdc1c9ce8ec3cfcd) またはDOMAIN\userです。

   >[!TIP]
   >
   >URLがわからない？ ここで、 [Dynamics組織サービスのURLを見つける方法を示します](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) 。

## 同期するフィールドの選択 {#select-fields-to-sync}

次に、同期するフィールドを選択する必要があります。

1. 手順2 **で**「編集」**をクリックします。「同期するフィールド」を選択します。**

   ![](assets/image2015-3-16-9-51-28a.png)

1. 事前に選択されたフィールドが同期されます。 必要に応じて、追加「 **保存**」をクリックします。

   ![](assets/image2016-8-25-13-3a26-3a14.png)

## カスタムフィルターのフィールドを同期 {#sync-fields-for-a-custom-filter}

カスタムフィルターを作成した場合は、Marketoと同期する新しいフィールドを必ず入力して選択してください。

1. 「管理者」に移動し、「 **Microsoft Dynamics**」を選択します。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 「フィールドの同期の詳細を **編集** 」をクリックします。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. フィールドまで下にスクロールし、チェックします。 実際の名前はnew_synctomktoにする必要がありますが、表示名は任意の名前にすることができます。 「 **保存**」をクリックします。

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## 同期を有効にする {#enable-sync}

1. **手順3で****「編集」をクリックします。同期を有効にします**。

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketing Toは、Microsoft Dynamicsの同期に対して、またはユーザーやリードを手動で入力した場合に、自動的に重複を排除しません。

1. ポップアップの内容をすべて読み、電子メールを入力し、「 **開始同期**」をクリックします。

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 最初の同期には数時間かかる場合があります。 完了すると、電子メール通知が届きます。

   ![](assets/image2014-12-11-11-3a55-3a15.png)

   素晴らしい仕事！
