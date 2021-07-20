---
unique-page-id: 2360356
description: ポータルへのシングルサインオンの追加 — Marketoドキュメント — 製品ドキュメント
title: ポータルへのシングルサインオンの追加
exl-id: 72f96239-7252-4cbc-bbe1-84ac7ae7f92e
source-git-commit: e4d581ab258a875747a6d5323764e8b4a3949cba
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 1%

---

# ポータルへのシングルサインオンの追加 {#add-single-sign-on-to-a-portal}

ユーザーを認証するディレクトリサービスがある場合は、Marketoへのシングルサインオン(SSO)を許可できます。 この機能は、Security Assertion Markup Language(SAML)バージョン2.0以降を使用してサポートされています。

MarketoはSAMLサービスプロバイダー(SP)として機能し、外部のIDプロバイダー(IdP)に依存してユーザーを認証します。

SSOが有効になると、IdPはユーザーの資格情報を検証できます。 ユーザーがMarketoソフトウェアを使用する場合、IdPは署名済みのSAMLメッセージをMarketoに送信し、SPとして機能します。 このメッセージは、ユーザーがMarketoソフトウェアを使用する権限を持っていることをMarketoに伝えます。

>[!NOTE]
>
>**管理者権限が必要**

>[!NOTE]
>
>Microsoft Azureユーザーですか？ [統合のチュートリアル](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/)をご覧ください。

## リクエストの送信方法 {#how-to-send-the-request}

* SAML応答であるSSOリクエストを`https://login.marketo.com/saml/assertion/<your-munchkin-id>`に送信します。
* SPのオーディエンスURL。 使用 `http://saml.marketo.com/sp`
* SPNameQualifier属性を使用する場合は、SubjectのNameID要素を`http://saml.marketo.com/sp`に設定します。
* 複数のMarketoサブスクリプションを同じSSOプロバイダーに統合する場合は、各Marketoサブに対して`http://saml.marketo.com/sp/<munchkin_id>`という形式の一意のSP URLを使用できます

>[!NOTE]
>
>Marketoは、IDプロバイダーが開始する（IdP開始とも呼ばれます）のみをサポートします。このIDプロバイダーでは、ユーザーが最初にIdpログインページを起動し、認証してからMy Marketoに移動します。

## 追加情報 {#additional-notes}

* **同期アップ時間**  — 新しいユーザーの場合、最初のSSOリクエストが処理されるまでに約10分の遅延があります。
* **ユーザープロビジョニング**  — ユーザーはMarketoによって手動でプロビジョニングされます。
* **認証**  — ユーザー権限はMarketo内で維持されます。
* **OAuthのサポート**  - Marketoは現在OAuthをサポートしていません。
* **自動ユーザー伝播**  - 「ジャストインタイムプロビジョニング」とも呼ばれ、ユーザーの最初のSAMLログインが、アクセスしているWebアプリケーション(Marketoなど)でユーザーを作成でき、手動の管理操作は不要です。現時点では、Marketoではサポートされていません。
* **暗号化**  - Marketoは現在暗号化をサポートしていません。

>[!NOTE]
>
>開始する前に、IDプロバイダー証明書をX.509形式で、.crt、.der、または.cer拡張子で入手します。

## SAML設定の更新 {#update-saml-settings}

SSOはデフォルトで無効になっています。 SAMLを有効にして設定するには、次の手順に従います。

1. **管理**&#x200B;に移動し、「**シングルサインオン**」をクリックします。

   ![](assets/image2014-9-24-14-3a36-3a50.png)

   >[!NOTE]
   >
   >**管理者**&#x200B;の下に&#x200B;**シングルサインオン**&#x200B;が表示されない場合は、[Marketoサポート](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。

1. 「**SAML設定**」セクションで、「**編集**」をクリックします。

   ![](assets/image2014-9-24-14-3a37-3a3.png)

1. **SAMLシングルサインオン**&#x200B;を&#x200B;**有効**&#x200B;に変更します。

   ![](assets/image2014-9-24-14-3a37-3a17.png)

1. **発行者ID**、**エンティティID**&#x200B;を入力し、**ユーザーIDの場所**&#x200B;を選択して、「**参照**」をクリックします。

   ![](assets/image2014-9-24-14-3a37-3a32.png)

1. **IDプロバイダーの証明書**&#x200B;ファイルを選択します。

   ![](assets/image2014-9-24-14-3a38-3a8.png)

1. 「**保存**」をクリックします。

   ![](assets/image2014-9-24-14-3a38-3a22.png)

## リダイレクトページ設定の更新 {#update-redirect-page-settings}

1. 「**ページをリダイレクト**」セクションで、「**編集**」をクリックします。

   ![](assets/seven.png)

   >[!NOTE]
   >
   >ユニバーサルIDとSSOを使用するお客様は、IDプロバイダーのログインURLを&#x200B;**Login URL**&#x200B;フィールドに入力する必要があります。

1. **ログアウトURL**&#x200B;を入力します。 これは、ユーザーがMarketoからログアウトしたときに表示されるURLです。

   ![](assets/eight.png)

1. **エラーURL**&#x200B;を入力します。 Marketoへのログインに失敗した場合にユーザーに表示するURLです。 「**保存**」をクリックします。

   ![](assets/nine.png)

   >[!NOTE]
   >
   >これらのページは両方とも公開されている必要があります。

>[!MORELIKETHIS]
>
>* [購読ログインでのユニバーサルIDの使用](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
* [ユーザ ログインを SSO のみに制限](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
* [ユニバーサルIDを使用した2つのインスタンスへのMarketoユーザーの招待](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

