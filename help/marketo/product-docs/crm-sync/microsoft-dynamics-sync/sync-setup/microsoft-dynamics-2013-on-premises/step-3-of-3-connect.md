---
unique-page-id: 3571819
description: 手順3/3 - MarkettoとDynamicsの接続（2013オンプレミス） - Marketto Docs — 製品ドキュメント
title: 手順3/3 - MarkettoとDynamicsの接続（2013オンプレミス）
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---


# 手順3/3:MarketoとDynamicsの接続(2013 On-Premises) {#step-of-connect-marketo-and-dynamics-on-premises}

>[!NOTE]
>
>**FYI**
>
>Marketoは現在、すべての購読で言語を標準化しているので、購読およびdocs.marketo.comの人物/人物にリード/リードを表示できます。 これらの用語は同じことを意味し、記事の説明には影響しません。 他にも変化がある。 [詳細情報](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

よし！ ソリューションをインストールし、同期ユーザーを構成しました。 次に、MarketoとDynamicsを結び付ける必要があります。

>[!PREREQUISITES]
>
>* [手順1/3:Dynamics(2013 On-Premises)にMarketo Solutionをインストールする](step-1-of-3-install.md)
>* [手順2/3:Marketor用の同期ユーザーの設定(2013 On-Premises)](step-2-of-3-configure.md)

>



>[!NOTE]
>
>**必要な管理者権限**

## Dynamics Syncユーザー情報の入力 {#enter-dynamics-sync-user-information}

1. Marketorにログインし、「 **管理者**」をクリックします。

   ![](assets/login-admin.png)

1. 「 **CRM**」をクリックします。

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. 「 **Microsoft**」を選択します。

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. **手順1で** 「 **編集」をクリックします。資格情報を入力します**。

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >送信後のスキーマの変更を元に戻すことができないため、資格情報が正しいことを確認してください。 正しくない資格情報を保存した場合は、新しいMarketor購読を取得する必要があります。

1. ユー **ザー名**、 **パスワード** 、Microsoft Dynamics **URLを入力し、「******&#x200B;保存」をクリックします。

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >Marketorのユーザー名は、CRMの同期ユーザーのユーザー名と一致する必要があります。 形式は、DOMAIN\user [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#631610061123070c0e020a0d4d000c0e) またはDOMAIN\userです。

   >[!TIP]
   >
   >URLがわからない？ ここで、 [Dynamics組織サービスのURLを見つける方法を示します](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) 。

## 同期するフィールドの選択 {#select-fields-to-sync}

次に、同期するフィールドを選択する必要があります。

1. 手 **順2で**編集**をクリックします。「同期するフィールド」を選択します**。

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. マーケティング担当者と同期するフィールドを選択して、事前に選択されるようにします。 「 **保存**」をクリックします。

   ![](assets/image2016-8-25-15-3a10-3a17.png)

## カスタムフィルターのフィールドを同期 {#sync-fields-for-a-custom-filter}

カスタムフィルターを作成した場合は、Marketoと同期する新しいフィールドを必ず入力して選択してください。

1. 「管理者」に移動し、「 **Microsoft Dynamics**」を選択します。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 「フィールドの同期の詳細を **編集** 」をクリックします。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. フィールドまで下にスクロールし、チェックします。 実際の名前はnew_synctomktoにする必要がありますが、表示名は任意の名前にすることができます。 「 **保存**」をクリックします。

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## 同期を有効にする {#enable-sync}

1. 手 **順3で**編集**をクリックします。同期を有効にします**。

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketing Toは、Microsoft Dynamicsの同期に対して、またはユーザーやリードを手動で入力した場合に、自動的に重複を排除しません。

1. ポップアップの内容をすべて読み、電子メールを入力し、 **開始同期をクリックします**。

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 最初の同期には数時間かかる場合があります。 完了すると、電子メール通知が届きます。

   ![](assets/image2014-12-11-11-3a55-3a15.png)

素晴らしい仕事！ MarketoとMicrosoft Dynamicsの間の双方向同期の機能を解放しました。 Marketo Sales Insightを購入済みの場合は、以下のような楽しさがあります。

>[!NOTE]
>
>**関連記事**
>
>* [Microsoft Dynamics 2013でのMarketo Sales Insightのインストールと構成](../../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)

>



