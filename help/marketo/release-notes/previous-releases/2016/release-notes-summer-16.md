---
unique-page-id: 11380218
description: リリースノート — 16年夏 — Marketoドキュメント — 製品ドキュメント
title: リリースノート — Summer '16
exl-id: 3843668e-c729-42aa-b05c-55c33ee0d783
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 8%

---

# リリースノート：16年夏 {#release-notes-summer}

Summer &#39;16リリースには、次の機能が含まれています。 お客様のご契約により、制限やオプションの契約が必要なものがあります。詳細は担当の営業にお問い合わせください。各機能の詳細な記事を表示するには、タイトルリンクをクリックしてください。

## [アカウントベースドマーケティング](https://docs.marketo.com/display/docs/account+based+marketing) {#account-based-marketing}

Marketoのアカウントベースのマーケティングは、1つの統合プラットフォームですべての基本事項を提供します。

* **Target**  — アカウントの検出、リードツーアカウントの照合、名前付きアカウントのリスト
* **エンゲージメント**  — アカウントベースのパーソナライゼーション、クロスチャネルのエンゲージメント、アカウント固有のワークフロー
* **測定**  — アカウントとリストレベルのインサイト、アカウントのエンゲージメントスコア、パイプラインと売上高への影響

![](assets/abm-5-acme.png)

>[!NOTE]
>
>ABMはMarketoサブスクリプションのアドオンとしてご利用いただけますので、実装するには営業担当にお問い合わせください。

## [監査証跡](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md) {#audit-trail}

監査証跡は、Marketoサブスクリプション内でおこなわれた変更の包括的な履歴を提供します。 ユーザーや管理者間で説明責任を生み出し、予期しない行動の原因を特定し、誰が何をいつ実行しているかを知るセキュリティを提供します。 この情報は、いつでも入手でき、次のような質問に答えるために使用できます。

* このアセットまたは設定に何が起きたか、最後に更新したのは誰か。
* Xは何をしてた？
* 誰がアカウントにログインするの？

![](assets/audit-trail.png)

## [MarketoとVibes SMS LaunchPointの統合](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md) {#marketo-vibes-sms-launchpoint-integration}

Marketo内でSMSメッセージを簡単に作成できます。 リッチなMarketoデータを使用してメッセージをパーソナライズおよびターゲット設定し、SMSメッセージダッシュボードを使用してメッセージのパフォーマンスを簡単に監視します。

>[!NOTE]
>
>この機能を使用するには、既存のVibes SMSアカウントが必要です。

![](assets/vibes-sms2.png)

## [Email 2.0 の強化](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-enhancements}

**モジュールレベルの変数**

以前は、 Eメール2.0テンプレートで指定されたすべての変数が、範囲内で「グローバル」でした。 モジュール内で変数を使用する場合、モジュールの複数のインスタンスを使用する予定がある場合は、必ずしもこの方法が望ましいとは限りません。 このリリースでは、変数を「モジュールレベル」として指定できるようになりました。これにより、ユーザーが使用する各モジュールに一意の値を設定できるようになります。

![](assets/module-level-variables.png)

**構文の更新**

* Email 2.0テンプレートで指定されたモジュールで「mktoAddByDefault」を使用して、新しいEメールにデフォルトで表示するモジュールを指定できるようになりました。 これは、多数のモジュールを含むEメールテンプレートを作成する場合に、はるかに便利です。
* 画像要素で、基になる`<img>` HTML要素の「height」および「width」プロパティをエンドユーザーに対してロックダウンするか編集可能にするかを指定できるようになりました。 mktoLockImgSize=&quot;true&quot;を指定すると、画像が変更された場合でも高さと幅がロックされます。 同様に、 mktoLockImgStyle=&quot;true&quot;は、&quot;style&quot;プロパティをロックします。

**コード検索**

新しい検索機能を使用して、電子メールコード内のコンテンツを効率的に検索および置換できます。 この機能は、 Eメールテンプレートエディターでも使用できます。

![](assets/2nd-screenshot.png)

**画像要素でのトークンのサポート**

「画像を挿入」エクスペリエンスの「外部URL」領域でトークンを使用できるようになりました。 `{{my.tokens}}`で画像を指定した場合は、Eメールエディター2.0内でこれらのトークンを参照できます。Eメールエディター2.0のキャンバスには、画像が壊れたまま表示されます。 ただし、Eメールを送信する前に、プレビューおよびサンプルを送信でレンダリングされるのが確認できます。

## 複数のブランディングドメイン {#multiple-branding-domains}

電子メールトラッキングリンクがブランディングドメインのみでブランド化できる日はなくなりました。 複数のブランディングドメインを追加して、消費者の信頼感を高め、より合理化された外観を作成してブランドに集中し、Eメールの配信品質を向上させ、Eメールごとに、各Eメールのトラッキングリンクに使用するブランディングドメインを選択できるようになりました。

![](assets/multiple-branding-domains.png)

## [プログラムトークン](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) {#program-tokens}

プログラム用の新しいトークンの種類が作成されました。 アセットとスマートキャンペーンのフローステップで、プログラム名、説明およびIDをレンダリングできるようになりました。

![](assets/program-tokens.png)

## [エンタープライズキー](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/authorize-the-marketo-outlook-plugin.md) {#enterprise-key}

Outlook用のSales Insightプラグインをセールスチームにインストールする必要は、面倒な作業です。 エンタープライズキーを使用してOutlook用のプラグインをリモートでインストールする新しい方法が導入されました。 管理者の「 Marketo Sales Insight 」セクションにある固有のキーをITチームに送信し、残りの操作を実行させます。

![](assets/enterprise-key.png)

## [Web パーソナライゼーションキャンペーン](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) {#web-personalization-campaigns}

WebキャンペーンがWebサイト上で反応するまでの時間を指定します。

![](assets/dialog-campaign-delay.png)

## [コンテンツ分析とRecommendationsの書き出し](/help/marketo/product-docs/web-personalization/understanding-web-personalization/understanding-content-analytics.md) {#content-analytics-and-recommendations-export}

コンテンツ分析＆レコメンデーションデータをオンラインで表示.

## [Email Editor 2.0 用の API サポート](https://developers.marketo.com/documentation/asset-api/) {#api-support-for-email-editor}

以前はv1.0の電子メールとテンプレートとのみ互換性があった既存のアセットAPIが、v2.0の電子メールアセットで有効になりました。

## [Marketo Developersサイト](https://developers.marketo.com/) {#marketo-developers-site}

開発者サイトをリニューアル

## [プライバシー設定](/help/marketo/product-docs/administration/settings/understanding-privacy-settings.md) {#privacy-settings}

マーケターは、プライバシー設定を使用して、MunchkinおよびWebパーソナライゼーション機能を使用して訪問者を追跡するかどうかを決定できます。 トラッキングレベルは、ブラウザーの「追跡しない」設定、オプトアウトCookie、または特定のIP以外を使用して制御します。 これらの方法は、特定の分野でのMarketoの価値と機能に影響を与える可能性がありますが、マーケターが何も変更しない場合、Marketoの機能は変わりません。

この機能は、6週間の間に徐々にリリースされる予定です。 すぐに必要な場合は、Marketoサポートにお問い合わせください。
