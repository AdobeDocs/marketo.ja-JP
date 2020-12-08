---
unique-page-id: 3571830
description: 手順3/3 - Microsoft DynamicsとMarketoの接続（オンライン） - Marketto Docs — 製品ドキュメント
title: 手順3/3 - Microsoft DynamicsとMarketoの接続（オンライン）
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---


# 手順3/3:Microsoft DynamicsとMarketoの接続（オンライン） {#step-of-connect-microsoft-dynamics-with-marketo-online}

>[!NOTE]
>
>**FYI**
>
>Marketoは現在、すべての購読で言語を標準化しているので、購読およびdocs.marketo.comの人物/人物にリード/リードを表示できます。 これらの用語は同じことを意味し、記事の説明には影響しません。 他にも変化がある。 [詳細情報](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

これが同期の最後のステップです。 もう少しで着く！

>[!NOTE]
>
>**前提条件**
>
>* [手順1/3:Marketor Solutionのインストール（オンライン）](step-1-of-3-install.md)
   >
   >
* [手順2/3:DynamicsでのMarket Syncユーザーの設定](step-2-of-3-set-up.md)

>



>[!NOTE]
>
>**必要な管理者権限**

## Dynamics Syncユーザー情報を入力 {#enter-dynamics-sync-user-information}

1. Marketorにログインし、「 **管理者**」をクリックします。

   ![](assets/login-admin.png)

1. 「 **CRM**」をクリックします。

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. 「 **Microsoft**」を選択します。

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. **手順1で****「編集」をクリックします。資格情報を入力します**。

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >送信後のスキーマの変更を元に戻すことができないため、資格情報が正しいことを確認してください。 正しくない資格情報を保存した場合は、新しいMarketor購読を取得する必要があります。

1. ユー **ザー名**、 **パスワード**、Microsoft Dynamics **** URLを入力します（クライアントIDとクライアントシークレットはオプションです）。 終了したら **「保存** 」をクリックします。

   ![](assets/five-1.png)

   >[!NOTE]
   >
   >Marketorのユーザー名は、CRMの同期ユーザーのユーザー名と一致する必要があります。 形式は、DOMAIN\user [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#bcc9cfd9cefcd8d3d1ddd5d292dfd3d1) またはDOMAIN\userです。

## 同期するフィールドの選択 {#select-fields-to-sync}

1. **手順2で****「編集」をクリックします。「同期するフィールド」を選択します**。

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. マーケティング担当者と同期するフィールドを選択して、事前に選択されるようにします。 「 **保存**」をクリックします。

   ![](assets/image2016-8-25-15-3a6-3a11.png)

## カスタムフィルターのフィールドを同期 {#sync-fields-for-a-custom-filter}

カスタムフィルターを作成した場合は、Marketoと同期する新しいフィールドを必ず入力して選択してください。

1. 「管理者」に移動し、「 **Microsoft Dynamics**」を選択します。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 「フィールドの同期の詳細を **編集** 」をクリックします。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. フィールドまで下にスクロールし、チェックします。 実際の名前はnew_synctomktoにする必要がありますが、表示名は任意の名前にすることができます。 「 **保存**」をクリックします。

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## 同期を有効にする {#enable-sync}

1. **手順3で****「編集」をクリックします。同期を有効にします**。

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketing Toは、Microsoft Dynamicsの同期に対して、またはユーザーやリードを手動で入力した場合に、自動的に重複を排除しません。

1. ポップアップの内容をすべて読み、電子メールアドレスを入力し、「 **開始同期**」をクリックします。

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. 最初の同期には数時間かかる場合があります。 完了すると、電子メール通知が届きます。

   ![](assets/image2015-3-16-9-3a59-3a51.png)

素晴らしい仕事！
