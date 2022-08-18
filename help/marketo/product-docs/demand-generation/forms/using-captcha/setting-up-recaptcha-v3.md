---
description: reCAPTCHA v3 の設定 — Marketoドキュメント — 製品ドキュメント
title: reCAPTCHA v3 のセットアップ
hide: true
hidefromtoc: true
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
source-git-commit: 24942664d613fa2851bad7a0dd3862027deacf37
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 4%

---

# reCAPTCHA v3 のセットアップ {#setting-up-recaptcha-v3}

導入テキスト

## reCAPTCHA v3 の初期設定 {#initial-recaptcha-v3-setup}

テキスト：v3 の説明 — 次の手順は、Marketo Engage外で実行します。

1. に移動します。 [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target=&quot;_blank&quot;} をクリックし、v3Admin Consoleをクリックします。

1. Googleアカウントでログイン/サインアップします。

1. 「作成」ボタン（+記号）をクリックして、新しいキーを作成します。

1. Marketo Engageに使用するキーを識別するラベルを作成します。

1. タイプを選択 **reCAPTCHA v3**. Marketo Engageは現在、reCAPTCHA v2 をサポートしていません。

1. Marketo Engage購読が使用する各ドメインを追加します。 ここで設定されていないドメインは、reCAPTCHA が有効なフォームでエラーを返します。

   * 123-ABC-456.mktoweb.com
   * app-pod.marketo.com
   * 配信登録で設定されたランディングページのドメインとエイリアス

1. このサービスに関するアラートを受け取る所有者と追加の電子メールアドレスを設定します。

1. reCAPTCHA サービス利用条件に同意します。

1. 「**送信**」をクリックします。

>[!NOTE]
>
>サイトキーと秘密鍵をMarketo Engage設定用に用意します。

## Marketo Engageでの CAPTCHA の設定 {#setting-up-captcha-in-marketo-engage}

1. Marketo で、「**管理者**」をクリックします。

   ![](assets/setting-up-recaptcha-v3-1.png)

1. 選択 **CAPTCHA** を設定します。

   ![](assets/setting-up-recaptcha-v3-2.png)

1. クリック **編集** をクリックします。

   ![](assets/setting-up-recaptcha-v3-3.png)

1. 「 CAPTCHA 」ドロップダウンをクリックし、「 reCAPTCHA v3 」を選択します。

   ![](assets/setting-up-recaptcha-v3-4.png)

1. 秘密鍵とサイトキーを挿入します。 終了したら「**保存**」をクリックします。

   ![](assets/setting-up-recaptcha-v3-5.png)
