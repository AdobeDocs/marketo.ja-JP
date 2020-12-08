---
unique-page-id: 10617187
description: プライバシー設定について — Marketto Docs — 製品ドキュメント
title: プライバシー設定について
translation-type: tm+mt
source-git-commit: efadb7eb3845012c273e1a60f9cd98ac884eb543
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---


# プライバシー設定について {#understanding-privacy-settings}

## 概要 {#overview}

マーケターに対して、Web訪問者の追跡に関する同意を得る方法を提供します。 匿名IPで追跡する方法は2つありオプトアウト、または匿名IPで追跡する方法を選択できます。

* Web訪問者ーは、ブラウザーで「追跡しない」(DNT)機能を選択します(マーケティング担当者は、追跡しないWeb訪問者の要求に従います)
* Web訪問者ーは、Webサイト上のマーケティング担当者が提供オプトアウトするCookieを使用します。

また、マーケティング担当者は、匿名IPを使用してユーザーを追跡できます。

これらの方法は、特定の領域におけるマーケティング担当者の価値と機能に影響を与える可能性があります。 ただし、マーケターがマーケティング担当者の設定 *に変更を加えない場合* 、マーケティング担当者の機能は変わりません。

## 「追跡しない」のブラウザー設定 {#browser-settings-for-do-not-track}

Web訪問者は、「追跡しない」(DNT)を選択することで、どのWebサイトでも追跡できないようにブラウザを設定できます。 これにより、特定のブラウザーおよびデバイスでの追跡を防ぎます。 詳しくは、ブラウザーのプライバシー設定を参照してください。

Munchkinでは、マーケティング担当者がブラウザーのDNT設定をサポートするか無視するかを [決定できます](edit-do-not-track-browser-support-settings.md)。

Webパーソナライゼーションでは、マーケティング担当者がブラウザーのDNT設定を [サポートするか無視するかを決定できます](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md)。

## 特定オプトアウトのWebサイトから {#opt-out-from-a-specific-website}

また、「 **ブラウザー追跡しない** 」設定が設定されているかどうかに関係なく、Webサイトの訪問者に対して、WebサイトからのWebサイト追跡を許可することもできます。 これにより、サイト訪問者はWebサイトから直接トラッキングの環境設定を指定できます。

これを行うには、マンチキン追跡が有効になっているWebページのオプトアウトリンクにパラメーターを追加する必要があります。 これは任意のWebページにすることができますが、Webページのリンクに次のパラメーターを含める必要があります。

?marketo_opt_out=true

以下に、オプトアウトリンクとリンクがクリックされた後のランディングページを含むWebページの例を示します。 君は変わる。

次のWebページには、オプトアウトリンクの「?marketo_opt_out=true」パラメーターを持つボタンが表示されています。

![](assets/opt-out-1.png)

「?marketo_opt_out=true」パラメーターを持つリンクがクリックされた場合のフォローアップページとしてランディングページを作成し、公開できます。

![](assets/opt-out-2.png)

リンクをクリックすると、Marketorは **** mkto_opt_outというCookieを訪問者のブラウザーに追加します。このCookieにより、上記のパラメーターを含むリンクをクリックしたサイト訪問者のMunchkin追跡が無効になります。

Cookieが植え付け可能であることを検証するには、Cookieを使用していることを確認し、リンクをクリックします。 次に、ブラウザーのCookieをチェックして、 **mkto_opt_out** Cookieが追加されたことを確認します。

![](assets/opt-out-3.png)

>[!NOTE]
>
>これは現在、Munchkinバージョン152以降でのみ機能します。

## オプトイン {#opt-in}

マーケターは、電子メール、フォーム、ランディングページなどの方法でオプトインマーケティング担当者の機能を使用して、ユーザーに対して実行を許可できます。

## 匿名化IPを使用した追跡 {#tracking-using-an-anonymized-ip}

マーケターは、匿名化されたIPアドレスを使用してユーザーを追跡することで、プライバシーを保持できます。 これを行うには、Webサイトに埋め込まれているRTPまたはMunchkin Javascriptにこのコードを追加します。

* Munchkinの場合は、init関数に{&quot;anonizeIP&quot;,true}を追加します。

   >[!NOTE]
   >
   >このパラメータを使用するには、Munchkin V2が有効になっている必要があります。 お使いの購読で有効にするには、 [マーケティング担当者にお問い合わせください](http://nation.marketo.com/community/support_solutions)。

* Webパーソナライゼーション(RTP)の場合、次をjavascriptに追加します。

匿名化IP :rtp(&#39;send&#39;,&#39;表示&#39;)；を呼び出す前にadd rtp(&#39;set&#39;, &#39;settings&#39;, {&#39;anonymizeIP&#39; :true});

