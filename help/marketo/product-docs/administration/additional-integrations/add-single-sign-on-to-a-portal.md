---
unique-page-id: 2360356
description: ポータルへ追加のシングルサインオン —Marketoドキュメント — 製品ドキュメント
title: ポータル追加へのシングルサインオン
exl-id: 72f96239-7252-4cbc-bbe1-84ac7ae7f92e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 1%

---

# ポータルへ追加のシングルサインオン{#add-single-sign-on-to-a-portal}

ユーザーを認証するディレクトリサービスがある場合は、Marketoへのシングルサインオン(SSO)を許可できます。 Security Assertion Markup Language(SAML)バージョン2.0以降を使用して、この機能をサポートしています。

MarketoはSAMLサービスプロバイダー(SP)として機能し、外部IDプロバイダー(IdP)に依存してユーザーを認証します。

SSOを有効にすると、IdPはユーザーの秘密鍵証明書を検証できます。 ユーザーがMarketoソフトウェアを使用したい場合、IdPは署名済みのSAMLメッセージをMarketoに送信し、SPとして機能します。 このメッセージは、ユーザーがMarketoソフトウェアの使用を承認されたことをMarketoに伝えます。

>[!NOTE]
>
>**必要な管理者権限**

>[!NOTE]
>
>Microsoft Azureユーザーですか？ [統合チュートリアル](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/)を見てください。

## リクエストの送信方法{#how-to-send-the-request}

* SAML応答であるSSO要求を`https://login.marketo.com/saml/assertion/<your-munchkin-id>`に送信します
* SPのオーディエンスURLとして使用する。 使用 `https://saml.marketo.com/sp`
* SPNameQualifier属性を使用する場合、SubjectのNameID要素を`https://saml.marketo.com/sp`に設定します
* 複数のMarketo・購読を同じSSOプロバイダに統合する場合は、各Marketo・サブに対して`https://saml.marketo.com/sp/<munchkin_id>`の形式で一意のSP URLを使用できます

>[!NOTE]
>
>Marketoは、IDプロバイダが開始する（IdPが開始するとも呼ばれる）もののみをサポートしています。この場合、ユーザーは最初にIdpログインページを起動し、認証してからマイMarketoに移動します。

## 追加のメモ{#additional-notes}

* **同期アップ時間**  — 新規ユーザーの場合、最初のSSO要求が処理されるまでに約10分の遅延があります。
* **ユーザープロビジョニング**  — ユーザーは、Marketoによって手動でプロビジョニングされます。
* **認証**  — ユーザー権限はMarketo内で保持されます。
* **OAuthサポート** -Marketoは現在OAuthをサポートしていません。
* **ユーザーの自動伝播** - 「ジャストインタイムプロビジョニング」とも呼ばれます。これは、ユーザーの最初のSAMLログインが、アクセスしているWebアプリケーション(例：Marketo)でユーザーを作成でき、手動の管理操作が不要な場合です。現時点では、Marketoではサポートされていません。
* **暗号化** -Marketoは現在暗号化をサポートしていません。

>[!NOTE]
>
>起動する前に、IDプロバイダ証明書をX.509形式、.crt、.der、または.cer拡張子で入手してください。

## SAML設定の更新{#update-saml-settings}

SSOはデフォルトで無効になっています。 SAMLを有効にして設定するには、次の手順に従います。

1. **管理者**&#x200B;に移動し、**シングルサインオン**&#x200B;をクリックします。

   ![](assets/image2014-9-24-14-3a36-3a50.png)

   >[!NOTE]
   >
   >**管理者**&#x200B;の下に&#x200B;**シングルサインオン**&#x200B;が表示されない場合は、[Marketoサポート](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。

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

1. **エラーURL**&#x200B;を入力します。 これは、Marketoへのログインに失敗した場合にユーザーに表示するURLです。 「**保存**」をクリックします。

   ![](assets/nine.png)

   >[!NOTE]
   >
   >これらのページはどちらも公開されている必要があります。

>[!MORELIKETHIS]
>
>* [購読ログインでのユニバーサルIDの使用](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [ユーザ ログインを SSO のみに制限](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
>* [ユニバーサルIDを使用した2つのインスタンスへのMarketoユーザーの招待](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

