---
unique-page-id: 10617187
description: プライバシー設定について - Marketo ドキュメント - 製品ドキュメント
title: プライバシー設定について
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
source-git-commit: bd6f049d5959356a99314e81bb6cfe517c2efdfa
workflow-type: ht
source-wordcount: '521'
ht-degree: 100%

---

# プライバシー設定について {#understanding-privacy-settings}

## 概要 {#overview}

Marketo は、web 訪問者のトラックに対する同意をマーケターに提供します。オプトアウトする方法は 2 つあります。また、匿名化した IP でトラッキングする方法を選択することもできます。

* Web 訪問者は、ブラウザーでトラッキング拒否（DNT）機能を選択します（マーケターは、web 訪問者のトラッキング拒否リクエストに従います）。
* Web 訪問者は、web サイトのマーケターによって提供されたオプトアウト cookie を使用します

または、マーケターは、匿名化した IP を使用してユーザをトラックできます。

これらの方法は、特定の領域での Marketo の価値や機能に影響を与える可能性があります。ただし、マーケターが Marketo の設定内容を&#x200B;*変更しない*&#x200B;場合は、Marketo の機能は変わりません。

## トラックしないためのブラウザー設定 {#browser-settings-for-do-not-track}

Web 訪問者は、ブラウザーで「トラックしない」（DNT）を選択することで、どの web サイトでもトラッキングされないように設定できます。これにより、この特定のブラウザーおよびデバイスでのトラッキングを防ぐことができます。詳しくは、ブラウザーのプライバシー設定を参照してください。

Munchkin では、マーケターは[ブラウザーの DNT 設定をサポートするか無視するかを決定する](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md)ことができます。

Web パーソナライゼーションでは、マーケターは[ブラウザーの DNT 設定をサポートするか無視する](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md)かを決定することができます。

## 特定の web サイトからのオプトアウト {#opt-out-from-a-specific-website}

**ブラウザーをトラックしない**&#x200B;設定の有無にかかわらず、サイト訪問者が web サイトからのトラッキングをオプトアウトできるようにすることも可能です。これにより、サイト訪問者は、web サイトから直接トラッキング設定を指定できます。

これを行うには、munchkin トラッキングが有効になっている web ページのオプトアウトリンクにパラメーターを追加する必要があります。任意の web ページを指定できますが、web ページのリンクには次のパラメーターを含める必要があります。

?marketo_opt_out=true

以下に、オプトアウトリンクおよびリンクがクリックされた後のランディングページを含む web ページの例を示します。ご自身の場合とは異なります。

これは、オプトアウトリンクに「?marketo_opt_out=true」パラメーターを持つボタンを含む web ページです。

![](assets/understanding-privacy-settings-1.png)

「?marketo_opt_out=true」パラメーターを含むリンクがクリックされた場合のフォローアップページとして、ランディングページを作成して公開できます。

![](assets/understanding-privacy-settings-2.png)

リンクがクリックされると、Marketo は **mkto_opt_out** という cookie を訪問者のブラウザーに追加し、上記のパラメーターでリンクをクリックしたサイト訪問者の Munchkin トラッキングを無効にするようにします。

Cookie を設置できることを検証するには、自分が cookie を設定したリードであることを確認し、リンクをクリックします。次に、ブラウザーの cookie を参照して、**mkto_opt_out** cookie が追加されたことを確認します。

![](assets/understanding-privacy-settings-3.png)

>[!NOTE]
>
>現在、これは Munchkin のバージョン 152 以降でのみ機能します。

## 参加 {#opt-in}

マーケターは、Marketo の機能を使用して、メール、フォーム、ランディングページなどの方法でユーザがオプトインできるようにすることができます。

## 匿名化した IP を使用したトラッキング {#tracking-using-an-anonymized-ip}

マーケターは、匿名化した IP アドレスでユーザをトラックすることで、プライバシーを保持できます。これを行うには、このコードを web サイトに埋め込まれている RTP または Munchkin JavaScript に追加します。

* Munchkin の場合、init 関数に {&quot;anonymizeIP&quot;,true} を追加するだけです。

   >[!NOTE]
   >
   >このパラメーターを使用するには、Munchkin V2 を有効にする必要があります。これをお使いのサブスクリプションで有効にするには、[Marketo サポート](https://nation.marketo.com/community/support_solutions)にお問い合わせください。

* Web パーソナライゼーション（RTP）の場合は、これを javascript に追加します。

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
