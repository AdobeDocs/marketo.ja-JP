---
description: reCAPTCHA v3 の設定 - Marketo ドキュメント - 製品ドキュメント
title: reCAPTCHA v3 の設定
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
feature: Forms
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 58%

---

# [!UICONTROL reCAPTCHA v3] の設定 {#setting-up-recaptcha-v3}

ReCAPTCHA v3 は、テキスト、画像、ボタンといったユーザへのチャレンジを使用せずに、フォーム送信の疑わしさを評価するストレスフリーのエクスペリエンスです。[詳細情報](https://developers.google.com/search/blog/2018/10/introducing-recaptcha-v3-new-way-to){target="_blank"}

## [!UICONTROL  データセンター ] および [!UICONTROL Munchkin ID] を取得 {#retrieve-your-data-center-and-munchkin-id}

以下の「[!UICONTROL reCAPTCHA v3] の初期設定」セクションの手順 6 では、Marketo Engage サブスクリプションの [!UICONTROL  データセンター ] と [!UICONTROL Munchkin ID] が必要になります。 確認方法は、以下のとおりです。

1. Marketo で、「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/setting-up-recaptcha-v3-1.png)

1. 「**[!UICONTROL マイアカウント]**」をクリックします。

   ![](assets/setting-up-recaptcha-v3-2.png)

1. 下方向にスクロールして [!UICONTROL  サポート情報 ] を表示します。

   ![](assets/setting-up-recaptcha-v3-3.png)

## [!UICONTROL reCAPTCHA v3] の初期設定 {#initial-recaptcha-v3-setup}

次の手順は、Marketo の外部で実行します。

1. [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target="_blank"} に移動し、v3 Admin Consoleをクリックします。

1. Google アカウントでログイン／サインアップします。

1. [!UICONTROL  作成 ] ボタン（+記号）をクリックして、新しいキーを作成します。

1. Marketo Engage に使用するキーを識別するラベルを作成します。

1. **[!UICONTROL reCAPTCHA v3]** タイプを選択します。Marketo Engage は現在、reCAPTCHA v2 をサポートしていません。

1. Marketo Engage サブスクリプションが使用する各ドメインを追加します。ここで設定されていないドメインは、reCAPTCHA が有効なフォームでエラーを返します。必ず「datacenter」と「munchkinID」という単語を、[ご自身のサブスクリプションのデータ](#retrieve-your-data-center-and-munchkin-id)と置き換えてください。

   * app-datacenter.marketo.com
   * munchkinID.mktoweb.com
   * サブスクリプションで設定されたランディングページのドメインとエイリアス

   >[!NOTE]
   >
   >例えば、アカウントの [!UICONTROL  データセンター ] が「sjst」の場合、許可リストに加えるするドメインは `app-sjst.marketo.com` です。 [!UICONTROL Munchkin 許可リストに加える ID] が 123-ABC-789 の場合、ドメインは `123-ABC-789.mktoweb.com` になります。

1. このサービスに関するアラートを受け取る所有者と追加のメールアドレスを設定します。

1. reCAPTCHA サービス利用規約に同意します。

1. 「**[!UICONTROL 送信]**」をクリックします。

   >[!NOTE]
   >
   >サイトキーと秘密鍵を Marketo Engage 設定用に準備しておきます。

## Marketo Engage での CAPTCHA の設定 {#setting-up-captcha-in-marketo-engage}

>[!IMPORTANT]
>
>以下の手順を実行し [ 最初のMarketo フォームで CAPTCHA を有効にする ](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"} したら、すぐにフォームをテストしてください。reCAPTCHA の設定ミスによってフォームが破損する可能性があるからです。

1. Marketo で、「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/setting-up-recaptcha-v3-4.png)

1. ツリーで「**[!UICONTROL CAPTCHA]**」を選択します。

   ![](assets/setting-up-recaptcha-v3-5.png)

1. **[!UICONTROL CAPTCHA]** 設定の [!UICONTROL  編集 ] をクリックします。

   ![](assets/setting-up-recaptcha-v3-6.png)

1. [!UICONTROL CAPTCHA] ドロップダウンをクリックして、「[!UICONTROL reCAPTCHA v3]」を選択します。

   ![](assets/setting-up-recaptcha-v3-7.png)

1. **[!UICONTROL 秘密鍵]** と **[!UICONTROL サイトキー]** を挿入します。 終了したら「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/setting-up-recaptcha-v3-8.png)

>[!MORELIKETHIS]
>
>[Marketo Forms で CAPTCHA を有効にする](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md)
