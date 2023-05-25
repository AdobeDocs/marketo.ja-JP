---
unique-page-id: 2360356
description: ポータルへのシングルサインオンの追加 - Marketo ドキュメント - 製品ドキュメント
title: ポータルへのシングルサインオンの追加
exl-id: 72f96239-7252-4cbc-bbe1-84ac7ae7f92e
source-git-commit: 1a6f029b8c9665ecd7fcc066004d88ee6c915505
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 94%

---

# ポータルへのシングルサインオンの追加 {#add-single-sign-on-to-a-portal}

ユーザを認証するディレクトリサービスをご利用の場合は、Marketo へのシングルサインオン（SSO）を許可することができます。この機能は、 [!DNL Security Assertion Markup Language] (SAML) バージョン 2.0 以降。

Marketo は SAML サービスプロバイダー（SP）として機能し、ユーザの認証には外部 ID プロバイダー（IdP）を使用します。

SSO を有効にすると、IdP がユーザの認証情報を検証できるようになります。ユーザが Marketo ソフトウェアを使おうとすると、SP として機能する Marketo に対して IdP が署名済み SAML メッセージを送信します。このメッセージは、当該ユーザが Marketo ソフトウェアの使用権限を持つことを Marketo に対して保証するものです。

>[!NOTE]
>
>**管理者権限が必要**

>[!NOTE]
>
>あなたは [!DNL Microsoft Azure] ユーザー？ 確認する [統合チュートリアル](https://azure.microsoft.com/ja-jp/documentation/articles/active-directory-saas-marketo-tutorial/){target="_blank"}.

## リクエストの送信方法 {#how-to-send-the-request}

* SAML 応答である SSO リクエストを `https://login.marketo.com/saml/assertion/<your-munchkin-id>` に送信します。
* SP のオーディエンス URL として次の URL を使用します。`http://saml.marketo.com/sp`
* SPNameQualifier 属性を使用している場合は、Subject の NameID 要素に次の値を設定します。`http://saml.marketo.com/sp`
* 複数の Marketo サブスクリプションを同じ SSO プロバイダーに統合する場合は、各 Marketo サブに対して `http://saml.marketo.com/sp/<munchkin_id>` 形式の一意の SP URL を使用できます

>[!NOTE]
>
>Marketo は、Identity Provider-initiated（IdP-initiated とも呼ばれます）のみをサポートします。この ID プロバイダーでは、ユーザが最初に Idp ログインページを起動し、認証してから My Marketo に移動します。

## そのほかの備考 {#additional-notes}

* **同期時間** - 新しいユーザの場合、最初の SSO リクエストが処理されるまでに約 10 分の遅延があります。
* **ユーザプロビジョニング** - ユーザは Marketo を使用して手動でプロビジョニングします。
* **認証** - ユーザ権限は Marketo 内で維持されます。
* **OAuth サポート** - Marketo は現在 OAuth をサポートしていません。
* **自動ユーザ反映** - 「ジャストインタイムプロビジョニング」とも呼ばれ、ユーザの最初の SAML ログインが、アクセスしている web アプリケーション（Marketo など）でユーザを作成でき、手動の管理操作は不要です。現時点では、Marketo ではサポートされていません。
* **暗号化** - Marketo は現在暗号化をサポートしていません。

>[!NOTE]
>
>開始する前に、X.509 形式、および拡張子 .crt、.der、.cer のいずれかの形式で ID プロバイダーの証明書を用意します。

## SAML 設定の更新 {#update-saml-settings}

SSO はデフォルトで無効になっています。SAML を有効にして設定するには、次の手順に従います。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/add-single-sign-on-to-a-portal-1.png)

1. 「**[!UICONTROL シングルサインオン]**」をクリックします。

   ![](assets/add-single-sign-on-to-a-portal-2.png)

   >[!NOTE]
   >
   >見えない場合 **[!UICONTROL シングルサインオン]** under **[!UICONTROL 管理者]**，連絡先 [Marketoサポート](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. 「**[!UICONTROL SAML 設定]**」セクションで、「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/add-single-sign-on-to-a-portal-3.png)

1. 「**[!UICONTROL SAML シングルサインオン]**」を&#x200B;**[!UICONTROL 有効]**&#x200B;に変更します。

   ![](assets/add-single-sign-on-to-a-portal-4.png)

1. 「**[!UICONTROL 発行者 ID]**」、「**[!UICONTROL エンティティ ID]**」を入力し、**[!UICONTROL ユーザ ID の場所]**&#x200B;を選択して、「**[!UICONTROL 参照]**」をクリックします。

   ![](assets/add-single-sign-on-to-a-portal-5.png)

1. **[!UICONTROL ID プロバイダー証明書]**&#x200B;ファイルを選択します。

   ![](assets/add-single-sign-on-to-a-portal-6.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/add-single-sign-on-to-a-portal-7.png)

## リダイレクトページ設定の更新 {#update-redirect-page-settings}

1. 「**[!UICONTROL ページをリダイレクト]**」セクションで、「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/add-single-sign-on-to-a-portal-8.png)

   >[!NOTE]
   >
   >ユニバーサル ID と SSO を使用するお客様は、ID プロバイダーのログイン URL を「**[!UICONTROL ログイン URL]**」フィールドに入力する必要があります。

1. 「**[!UICONTROL ログアウト URL]**」を入力します。これは、Marketo からログアウトしたときにユーザを転送する先の URL です。

   ![](assets/add-single-sign-on-to-a-portal-9.png)

1. 「**[!UICONTROL エラー URL]**」を入力します。これは、Marketo へのログインが失敗した場合にユーザを転送する先の URL です。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/add-single-sign-on-to-a-portal-10.png)

   >[!NOTE]
   >
   >これらのページは、どちらも一般公開されている必要があります。

>[!MORELIKETHIS]
>
>* [サブスクリプションログインでのユニバーサル ID の使用](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md){target="_blank"}
>* [ユーザーログインを SSO のみに制限](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md){target="_blank"}
>* [ユニバーサル ID を使用して、2 つのインスタンスに Marketo ユーザーを招待](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122){target="_blank"}

