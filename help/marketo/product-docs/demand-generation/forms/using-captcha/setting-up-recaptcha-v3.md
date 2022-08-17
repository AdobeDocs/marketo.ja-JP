---
description: reCAPTCHA v3 の設定 — Marketoドキュメント — 製品ドキュメント
title: reCAPTCHA v3 のセットアップ
hide: true
hidefromtoc: true
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
source-git-commit: 1803d6355747f4b6300509a3d361bf235dd56f44
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 4%

---

# reCAPTCHA の設定 {#setting-up-recaptcha}

導入テキスト

## reCAPTCHA v3 のセットアップ {#setting-up-recaptcha-v3}

テキスト：v3 の説明 — 次の手順は、Marketo Engage外で実行します。

1. に移動します。 [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target=&quot;_blank&quot;} をクリックし、v3Admin Consoleをクリックします。

1. Googleアカウントでログイン/サインアップします。

1. 「作成」（+記号）ボタンをクリックして、新しいキーを作成します。

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

1. Marketoで、 **管理者** を選択し、 **CAPTCHA**.

PICC

1. クリック **編集** をクリックします。

PICC

1. 「 CAPTCHA 」ドロップダウンをクリックし、「 reCAPTCHA v3 」を選択します。

PICC

1. 秘密鍵とサイトキーを挿入します。 終了したら「**保存**」をクリックします。

PICC
