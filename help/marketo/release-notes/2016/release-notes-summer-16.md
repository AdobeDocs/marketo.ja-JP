---
unique-page-id: 11380218
description: リリースノート —Summer '16 - Marketto Docs — 製品ドキュメント
title: リリースノート — 16年夏
translation-type: tm+mt
source-git-commit: efadb7eb3845012c273e1a60f9cd98ac884eb543
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 0%

---


# リリースノート：Summer &#39;16 {#release-notes-summer}

16年夏リリースには次の機能が含まれています。 Marketing Editionで機能が使用できるかどうかを確認します。 タイトルリンクをクリックすると、各機能に関する表示の詳細記事が表示されます。

## [アカウントベースのマーケティング](http://docs.marketo.com/display/docs/account+based+marketing) {#account-based-marketing}

Markettoアカウントベースのマーケティングは、1つの統合されたプラットフォームにすべての重要な要素を提供します。

* **ターゲット** ：アカウントの検出、リード・ツー・アカウントの照合、名前付きアカウントのリスト
* **エンゲージメント**  — アカウントベースのパーソナライゼーション、チャネル間のエンゲージメント、アカウント固有のワークフロー
* **測定**  — アカウントおよびリストレベルのインサイト、アカウント関与スコア、パイプラインおよび売上高への影響

![](assets/abm-5-acme.png)

>[!NOTE]
>
>ABMはMarketo購読のアドオンとして使用できるので、セールス担当者に連絡して導入を依頼してください。

## [監査証跡](http://docs.marketo.com/display/docs/audit+trail) {#audit-trail}

監査証跡は、マーケティング購読内で行われた変更の包括的な履歴を提供します。 ユーザーと管理者の間で説明責任を作り、予期しない行動の原因を特定し、誰が何をいつ実行しているかを知るセキュリティを提供します。 この情報はいつでも入手でき、次のような質問に答えるのに使用できます。

* このアセットまたは設定はどうなりましたか。また、最後に更新したのは誰ですか。
* Xが何を企んでいる？
* 誰がアカウントにログインしているか。

![](assets/audit-trail.png)

## [Marketo Vibes SMS LaunchPoint統合](http://docs.marketo.com/display/docs/vibes+sms+messages) {#marketo-vibes-sms-launchpoint-integration}

Marketo内で簡単にSMSメッセージを作成できます。 リッチなマーケティングデータを使用してメッセージをパーソナライズおよびターゲットし、SMSメッセージダッシュボードを使用してパフォーマンスを簡単に監視できます。

>[!NOTE]
>
>この機能を使用するには、既存のVibe SMSアカウントが必要です。

![](assets/vibes-sms2.png)

## [Email 2.0の機能強化](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-enhancements}

**モジュールレベル変数**

以前は、Email 2.0 Templatesで指定されたすべての変数は、スコープ内では「グローバル」でした。 モジュール内で変数を使用する場合、モジュールの複数のインスタンスを使用する予定がある場合は、この方法が適していないことがあります。 このリリースでは、変数を「モジュールレベル」として指定できるようになりました。これにより、使用する各モジュールに対して一意の値を設定できる必要があることをユーザーに示すことができます。

![](assets/module-level-variables.png)

**構文の更新**

* Email 2.0 Templatesで指定されたモジュールで「mktoAddByDefault」を使用して、デフォルトで新しい電子メールに表示するモジュールを指定できるようになりました。 これは、多数のモジュールを含む電子メールテンプレートを作成する場合に、はるかに便利です。
* 画像要素で、基になる`<img>` HTML要素の「height」プロパティと「width」プロパティを、エンドユーザーに対してロックダウンするか編集可能にするかを指定できるようになりました。 mktoLockImgSize=&quot;true&quot;を指定すると、高さ/幅がロックされます（画像が変更された場合でも）。 同様に、mktoLockImgStyle=&quot;true&quot;を指定すると、&quot;style&quot;プロパティがロックされます。

**コード検索**

新しい検索機能を使用して、電子メールのコード内のコンテンツを効率的に検索および置換できます。 この機能は、電子メールテンプレートエディターでも使用できます。

![](assets/2nd-screenshot.png)

**画像要素でのトークンのサポート**

トークンを、挿入画像エクスペリエンスの「外部URL」領域で使用できるようになりました。 `{{my.tokens}}`で画像を指定した場合、電子メールエディタ2.0内でこれらのトークンを参照できるようになりました。電子メールエディタ2.0のキャンバスには、画像が壊れて表示されます。 ただし、電子メールを送信する前に、プレビューおよびサンプルの送信内に表示されます。

## [複数のブランドドメイン](http://docs.marketo.com/display/docs/add+multiple+branding+domains) {#multiple-branding-domains}

E メールトラッキングログのリンクが単一のブランディングドメインでのみブランド化できる日々はなくなりました。 複数のブランディングドメインを追加して、消費者の信頼感を高め、ブランドに焦点を当てて合理化された外観を作成し、電子メールの配信品質を向上させ、各電子メールのトラッキングリンクに使用するブランディングドメインを電子メール単位で選択できるようになりました。

![](assets/multiple-branding-domains.png)

## [プログラムトークン](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) {#program-tokens}

プログラム用に新しいトークンタイプを作成しました。 アセットおよびスマートキャンペーンのフローステップで、プログラム名、説明およびIDをレンダリングできるようになりました。

![](assets/program-tokens.png)

## [エンタープライズキー](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/authorize-the-marketo-outlook-plugin.md) {#enterprise-key}

Outlook用のSales Insightプラグインをセールスチームの各担当者がインストールする必要は、退屈な作業です。 エンタープライズキーを使用してリモートでOutlook用のプラグインをインストールする新しい方法が導入されました。 管理者の「Marketo Sales Insight」セクションにある固有のキーをITチームに送信し、残りの作業を行わせます。

![](assets/enterprise-key.png)

## [Webパーソナライゼーションキャンペーン](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) {#web-personalization-campaigns}

WebキャンペーンがWebサイト上で反応する遅延時間を指定します。

![](assets/dialog-campaign-delay.png)

## [コンテンツ分析とRecommendationsのエクスポート](/help/marketo/product-docs/web-personalization/understanding-web-personalization/understanding-content-analytics.md) {#content-analytics-and-recommendations-export}

表示コンテンツ分析とレコメンデーションデータをオフラインで使用できます。

## [電子メールエディター2.0のAPIサポート](http://developers.marketo.com/documentation/asset-api/) {#api-support-for-email-editor}

以前はv1.0の電子メールおよびテンプレートとのみ互換性があった既存のアセットAPIが、v2.0の電子メールアセットで有効になりました。

## [マーケティング開発者サイト](http://developers.marketo.com/) {#marketo-developers-site}

新しく改善されました。

## [プライバシー設定](/help/marketo/product-docs/administration/settings/understanding-privacy-settings.md) {#privacy-settings}

マーケターは、プライバシー設定を使用して、Munchkin機能とWebパーソナライゼーション機能を使用して訪問者を追跡するかどうかを決定できます。 追跡レベルは、ブラウザーの「追跡しない」設定、オプトアウトCookieまたは特定のIP以外を使用して制御します。 これらの方法は、特定の領域におけるマーケティング担当者の価値と機能に影響を与える可能性がありますが、マーケティング担当者が何も変更しない場合、マーケティング担当者の機能は変わりません。

この機能は、6週間にわたって徐々にリリースされる予定です。 すぐに必要な場合は、マーケティング担当者にお問い合わせください。
