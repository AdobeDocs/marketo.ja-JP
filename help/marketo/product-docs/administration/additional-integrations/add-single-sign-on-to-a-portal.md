---
unique-page-id: 2360356
description: ポータルへ追加のシングルサインオン — Marketto Docs — 製品ドキュメント
title: ポータル追加へのシングルサインオン
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---


# ポータルへ追加のシングルサインオン{#add-single-sign-on-to-a-portal}

ユーザーを認証するディレクトリサービスがある場合、Marketorへのシングルサインオン(SSO)を許可できます。 Security Assertion Markup Language(SAML)バージョン2.0以降を使用して、この機能をサポートしています。

マーケティング担当者はSAMLサービスプロバイダー(SP)として機能し、ユーザーを認証するために外部IDプロバイダー(IdP)に依存します。

SSOを有効にすると、IdPはユーザーの秘密鍵証明書を検証できます。 ユーザーがMarketoソフトウェアを使用したい場合、IdPは署名済みのSAMLメッセージをMarketoに送信し、SPとして機能します。 このメッセージは、ユーザーがMarketoソフトウェアを使用する権限を持つMarketoに伝達されます。

>[!NOTE]
>
>**必要な管理者権限**

>[!NOTE]
>
>Microsoft Azureユーザーですか？ [統合チュートリアル](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/)を見てください。

## リクエストの送信方法{#how-to-send-the-request}

* SAML応答であるSSO要求を`https://login.marketo.com/saml/assertion/<your-munchkin-id>`に送信します
* SPのオーディエンスURLとして使用する。 `https://saml.marketo.com/sp`を使用
* SPNameQualifier属性を使用する場合、SubjectのNameID要素を`https://saml.marketo.com/sp`に設定します
* 複数のMarketor購読を同じSSOプロバイダーに統合する場合、`https://saml.marketo.com/sp/<munchkin_id>`の形式で各Marketorサブに一意のSP URLを使用できます。

>[!NOTE]
>
>ユーザーが最初にIdpログインページを起動し、認証してから「マーケティング担当者」に移動する、IDプロバイダーが開始する（IdPが開始するとも呼ばれます）操作のみがサポートされます。

## 追加のメモ{#additional-notes}

* **同期アップ時間**  — 新規ユーザーの場合、最初のSSO要求が処理されるまでに約10分の遅延があります。
* **ユーザープロビジョニング**  — ユーザーは、Marketing Targetによって手動でプロビジョニングされます。
* **認証**  — ユーザー権限はMarketor内で保持されます。
* **OAuthサポート** - Marketorは現在OAuthをサポートしていません。
* **ユーザーの自動伝播** - 「ジャストインタイムプロビジョニング」とも呼ばれます。これは、ユーザーの最初のSAMLログインが、アクセスしているWebアプリケーション（例：Marketo）でユーザーを作成でき、手動の管理操作は不要な場合です。現時点では、Marketorはこの機能をサポートしていません。
* **暗号化** - Marketorは現在、暗号化をサポートしていません。

>[!NOTE]
>
>起動する前に、IDプロバイダ証明書をX.509形式、.crt、.der、または.cer拡張子で入手してください。

## SAML設定の更新{#update-saml-settings}

SSOはデフォルトで無効になっています。 SAMLを有効にして設定するには、次の手順に従います。

1. **管理者**&#x200B;に移動し、**シングルサインオン**&#x200B;をクリックします。

   ![](assets/image2014-9-24-14-3a36-3a50.png)

   >[!NOTE]
   >
   >**管理者**&#x200B;の下に&#x200B;**シングルサインオン**&#x200B;が表示されない場合は、[マーケティング担当者](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。

1. 「**SAML設定**」セクションで、「**編集**」をクリックします。

   ![](assets/image2014-9-24-14-3a37-3a3.png)

1. **SAMLシングルサインオン**&#x200B;を&#x200B;**有効**&#x200B;に変更します。

   ![](assets/image2014-9-24-14-3a37-3a17.png)

1. **発行者ID**、**エンティティID**&#x200B;を入力し、**ユーザーIDの場所**&#x200B;を選択して、**参照**&#x200B;をクリックします。

   ![](assets/image2014-9-24-14-3a37-3a32.png)

1. **IDプロバイダー証明書**&#x200B;ファイルを選択します。

   ![](assets/image2014-9-24-14-3a38-3a8.png)

1. 「**保存**」をクリックします。

   ![](assets/image2014-9-24-14-3a38-3a22.png)

## リダイレクトページ設定の更新{#update-redirect-page-settings}

1. 「**ページをリダイレクト**」セクションで、「**編集**」をクリックします。

   ![](assets/seven.png)

   >[!NOTE]
   >
   >ユニバーサルIDとSSOを使用するお客様は、IDプロバイダーのログインURLを&#x200B;**Login URL**&#x200B;フィールドに入力する必要があります。

1. **ログアウトURL**&#x200B;を入力します。 これは、ユーザーがMarketoからログアウトしたときに表示するURLです。

   ![](assets/eight.png)

1. **エラーURL**&#x200B;を入力します。 これは、Marketorへのログインに失敗した場合にユーザーに転送するURLです。 「**保存**」をクリックします。

   ![](assets/nine.png)

   >[!NOTE]
   >
   >これらのページはどちらも公開されている必要があります。

>[!MORELIKETHIS]
>
>* [購読ログインでのユニバーサルIDの使用](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [ユーザーログインをSSOのみに制限](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
>* [ユニバーサルIDを持つ2つのインスタンスへのマーケティングユーザーの招待](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

