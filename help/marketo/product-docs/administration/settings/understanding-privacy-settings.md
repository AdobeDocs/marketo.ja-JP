---
unique-page-id: 10617187
description: プライバシー設定について —Marketoドキュメント — 製品ドキュメント
title: プライバシー設定について
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# プライバシー設定について{#understanding-privacy-settings}

## 概要 {#overview}

Marketoは、マーケティング担当者に、Web訪問者の追跡に関する同意を得る方法を提供しています。 匿名IPで追跡する方法は2つありオプトアウト、または匿名IPで追跡する方法を選択できます。

* Web訪問者ーは、ブラウザーで「追跡しない」(DNT)機能を選択します(マーケティング担当者は、追跡しないWeb訪問者の要求に従います)
* Web訪問者ーは、Webサイト上のマーケティング担当者が提供オプトアウトするCookieを使用します。

また、マーケティング担当者は、匿名IPを使用してユーザーを追跡できます。

これらの方法は、特定の領域におけるMarketoの価値と機能に影響を与える可能性があります。 ただし、マーケター&#x200B;*がMarketoの設定内の変更を*&#x200B;行わない場合、Marketoの機能は変わりません。

## 追跡しないブラウザーの設定{#browser-settings-for-do-not-track}

Web訪問者は、「追跡しない」(DNT)を選択することで、どのWebサイトでも追跡できないようにブラウザを設定できます。 これにより、特定のブラウザーおよびデバイスでの追跡を防ぎます。 詳しくは、ブラウザーのプライバシー設定を参照してください。

Munchkinでは、マーケティング担当者は[ブラウザのDNT設定](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md)をサポートするか無視するかを決定できます。

Webパーソナライゼーションでは、マーケティング担当者がブラウザーのDNT設定](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md)を[サポートするか無視するかを決定できます。

## 特定オプトアウトのWebサイト{#opt-out-from-a-specific-website}から

また、**ブラウザー追跡を行わない**&#x200B;設定が設定されているかどうかに関係なく、Webサイトの訪問者オプトアウトに対して、WebサイトからのWebサイト追跡を許可することもできます。 これにより、サイト訪問者はWebサイトから直接トラッキングの環境設定を指定できます。

これを行うには、マンチキン追跡が有効になっているWebページのオプトアウトリンクにパラメーターを追加する必要があります。 これは任意のWebページにすることができますが、Webページのリンクに次のパラメーターを含める必要があります。

?marketo_opt_out=true

以下に、オプトアウトリンクとリンクがクリックされた後のランディングページを含むWebページの例を示します。 君は変わる。

次のWebページには、オプトアウトリンクの「?marketo_opt_out=true」パラメーターを持つボタンが表示されています。

![](assets/opt-out-1.png)

「?marketo_opt_out=true」パラメーターを持つリンクがクリックされた場合のフォローアップページとしてランディングページを作成し、公開できます。

![](assets/opt-out-2.png)

リンクをクリックすると、Marketoは&#x200B;**mkto_opt_out**&#x200B;というCookieを訪問者のブラウザに追加し、上記のパラメータを含むリンクをクリックしたサイト訪問者のMunchkin追跡を無効にします。

Cookieが植え付け可能であることを検証するには、Cookieを使用していることを確認し、リンクをクリックします。 次に、ブラウザーのCookieを確認して、**mkto_opt_out** Cookieが追加されたことを確認します。

![](assets/opt-out-3.png)

>[!NOTE]
>
>これは現在、Munchkinバージョン152以降でのみ機能します。

## 参加 {#opt-in}

マーケターは、電子メール、フォーム、ランディングページなどの方法でオプトインMarketoの機能を使用することで、ユーザーが行えるようにすることができます。

## 匿名IPを使用した追跡{#tracking-using-an-anonymized-ip}

マーケターは、匿名化されたIPアドレスを使用してユーザーを追跡することで、プライバシーを保持できます。 これを行うには、Webサイトに埋め込まれているRTPまたはMunchkin Javascriptにこのコードを追加します。

* Munchkinの場合は、init関数に{&quot;anonizeIP&quot;,true}を追加します。

   >[!NOTE]
   >
   >このパラメータを使用するには、Munchkin V2が有効になっている必要があります。 ご使用の購読で有効にするには、[Marketoサポート](https://nation.marketo.com/community/support_solutions)にお問い合わせください。

* Webパーソナライゼーション(RTP)の場合、次をjavascriptに追加します。

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
