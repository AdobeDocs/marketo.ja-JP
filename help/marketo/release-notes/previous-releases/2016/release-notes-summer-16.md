---
unique-page-id: 11380218
description: リリースノート - 2016 年夏 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2016 年夏
exl-id: 3843668e-c729-42aa-b05c-55c33ee0d783
TQID: https://experienceleague.adobe.com/8CDFBAF3ww-2MEGQ4ypWIZclmfCj6ncATdebtubOUk4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: e0eb8757-182f-49f3-94a4-1587d16f5094id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eddd9b14-83bd-4ff4-9072-54a4a484abb7id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 799
ht-degree: 93%

---

# リリースノート：2016年夏 {#release-notes-summer}

2016 年夏リリースには、次の機能が含まれています。 お客様のご契約により、制限やオプションの契約が必要なものがあります。詳細は担当の営業にお問い合わせください。 各機能の詳細な記事を表示するには、タイトルリンクをクリックしてください。

## [アカウントベースドマーケティング](https://docs.marketo.com/display/docs/account+based+marketing) {#account-based-marketing}

Marketo のアカウントベースドマーケティングは、1 つの統合プラットフォームですべての基本事項を提供します。

* **ターゲット** - 顧客検出、リードから顧客への照合、アカウントリスト
* **エンゲージ** - アカウントベースのパーソナライゼーション、クロスチャネルのエンゲージメント、アカウント固有のワークフロー
* **測定** — 顧客とリストレベルのインサイト、顧客のエンゲージメントスコア、パイプラインと売上高への影響

![](assets/abm-5-acme.png)

>[!NOTE]
>
>ABM は Marketo サブスクリプションのアドオンとして利用できるので、実装するには営業担当にお問い合わせください。

## [監査記録](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md) {#audit-trail}

監査記録は、Marketo サブスクリプション内でおこなわれた変更の包括的な履歴を提供します。 これにより、ユーザーや管理者間で説明責任を作成し、予期しない行動の原因を特定し、誰がいつ何をしているかを知るセキュリティが確保されます。 この情報は、いつでも使用可能で、次のような質問に回答するために使用できます。

* このアセットまたは設定に何が起きたか、最後に更新したのは誰か。
* ユーザー X は何をしているのか。
* アカウントにログインしているのは誰か。

![](assets/audit-trail.png)

## Marketo-Vibes SMS LaunchPoint の統合

Marketo 内で SMS メッセージを簡単に作成できます。 リッチ Marketo データを使用してメッセージをパーソナライズおよびターゲット設定し、SMS メッセージダッシュボードを使用してパフォーマンスを簡単に監視します。

>[!NOTE]
>
>この機能を使用するには、既存の [!DNL Vibes SMS] アカウントが必要です。

![](assets/vibes-sms2.png)

## [Email 2.0 の強化](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-enhancements}

**モジュールレベルの変数**

以前は、メール 2.0 テンプレートで指定されたすべての変数の範囲は「グローバル」でした。 モジュール内で変数を使用する場合、モジュールの複数のインスタンスを使用する予定がある場合は、必ずしも望ましくありません。 このリリースでは、変数を「モジュールレベル」として指定できるようになり、ユーザが使用するモジュールごとに一意の値を設定できるようになります。

![](assets/module-level-variables.png)

**構文の更新**

* メール 2.0 テンプレートで指定されたモジュールで「mktoAddByDefault」を使用して、新しいメールにデフォルトで表示するモジュールを指定できるようになりました。 これは、多数のモジュールを含むメールテンプレートを作成する場合に、はるかに便利です。
* 画像要素で、基になる `<img>` HTML 要素の「height」および「width」プロパティは、エンドユーザに対してロックするまたは編集可能にする必要があります。 「mktoLockImgSize=“true”」を指定すると、画像が変更された場合でも高さと幅がロックされます。 同様に、「mktoLockImgStyle=“true”」を指定すると、「style」プロパティがロックされます。

**コード検索**

新しい検索機能を使用して、メールコード内のコンテンツを効率的に検索および置換できます。 この機能は、メールテンプレートエディターでも使用できます。

![](assets/2nd-screenshot.png)

**画像要素でのトークンのサポート**

トークンを画像挿入エクスペリエンスの「外部 URL」領域で使用できるようになりました。 `{{my.tokens}}`で画像を指定した場合、メールエディター2.0内でこれらのトークンを参照できるようになりました。 電子メールエディター2.0のキャンバスでは、画像が破損したままになります。 ただし、メールを送信する前に、プレビューとサンプルの送信でレンダリングされているのが確認できます。

## 複数のブランディングドメイン {#multiple-branding-domains}

メールトラッキングリンクを複数のブランディングドメインでブランディングできるようになりました。 複数のブランディングドメインを追加して、消費者の信頼感を高め、より合理化された外観を作成してブランドに焦点を当て、メールの配信品質を向上させ、メール単位で各メールのトラッキングリンクに対してどのブランディングドメインを使用するかを選択できるようになりました。

![](assets/multiple-branding-domains.png)

## [プログラムトークン](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) {#program-tokens}

プログラムの新しいトークンの種類が作成されました。 アセットとスマートキャンペーンのフローステップで、プログラム名、説明および ID をレンダリングできるようになりました。

![](assets/program-tokens.png)

## [エンタープライズキー](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/authorize-the-marketo-outlook-plugin.md) {#enterprise-key}

セールスチームの各メンバーに [!DNL Outlook] 用の [!DNL Sales Insight] プラグインをインストールするよう要求するのは、面倒で手間がかかります。 エンタープライズキーを使用して [!DNL Outlook] 用のプラグインをリモートでインストールする新しい方法が導入されました。 [!UICONTROL 管理者]の Marketo [!DNL Sales Insight] セクションにある固有のキーを IT チームに送信し、残りの作業を行ってもらいます。

![](assets/enterprise-key.png)

## [Web パーソナライゼーションキャンペーン](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) {#web-personalization-campaigns}

ウェブサイト上で web キャンペーンが反応するまでの時間を指定します。

![](assets/dialog-campaign-delay.png)

## [コンテンツ分析＆レコメンデーションのエクスポート](/help/marketo/product-docs/web-personalization/understanding-web-personalization/understanding-content-analytics.md) {#content-analytics-and-recommendations-export}

コンテンツ分析＆レコメンデーションデータをオンラインで表示.

## [Email Editor 2.0 用の API サポート](https://developers.marketo.com/documentation/asset-api/) {#api-support-for-email-editor}

以前は v1.0 のメールとテンプレートとのみ互換性があった、既存の Asset API が v2.0 のメールアセットで有効になりました。

## [Marketo デベロッパーサイト](https://developers.marketo.com/) {#marketo-developers-site}

デベロッパーサイトをリニューアル

## [プライバシー設定](/help/marketo/product-docs/administration/settings/understanding-privacy-settings.md) {#privacy-settings}

マーケターは、プライバシー設定を使用して、[!DNL Munchkin] と web パーソナライゼーション機能を使用して訪問者を追跡するかどうかを決定できます。 トラッキングレベルは、ブラウザーの「Do Not Track」設定、オプトアウト Cookie、特定でない IP を使用して制御します。 これらの方法は、特定の分野での Marketo の価値や機能に影響を与える可能性がありますが、マーケターが何も変更しない場合、Marketo の機能は変わりません。

この機能は、6 週間の間に徐々にリリースされます。 すぐに必要な場合は、Marketo サポートにお問い合わせください。
