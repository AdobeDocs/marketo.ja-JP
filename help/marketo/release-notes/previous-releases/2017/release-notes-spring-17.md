---
unique-page-id: 12977439
description: リリースノート — Spring '17 - Marketoドキュメント — 製品ドキュメント
title: リリースノート — Spring '17
exl-id: 61873d1f-41dd-4f5c-94d0-65f0bcacff75
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 11%

---

# リリースノート：春17 {#release-notes-spring}

Spring &#39;17リリースには、次の機能が含まれています。 お客様のご契約により、制限やオプションの契約が必要なものがあります。詳細は担当の営業にお問い合わせください。

各機能の詳細な記事を表示するには、タイトルリンクをクリックしてください。**注意**:トピックに複数のサブ見出しが含まれる場合、リンクはそこに配置されます。

## [linkedInリードジェンForms](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-forms}

[linkedIn Lead Gen Forms](https://business.linkedin.com/marketing-solutions/native-advertising/lead-gen-ads) は、LinkedIn上でリードジェネレーションキャンペーンを実行する、より直接的な方法です。ユーザーは製品やサービスに関心を示すためのフォームに入力でき、ビジネスでユーザーの詳細を取得し、Marketoに同期できます。この場合、追跡プロセスやリードルーティングの自動化が可能です。

MarketoとLinkedIn Lead Gen Formsの統合により、リードがリードジェンフォーム内で提供する情報が自動的に取り込まれます。 その後、新しい&#x200B;**Fills Out LinkedIn Lead Gen Form**&#x200B;トリガーとフィルターを使用して、フォローアップアクションと通知を自動化できます。

![](assets/release-notes-image.png)

## [MSI テンプレートの有効期限設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/publish-an-email-to-sales-insight.md) {#expire-msi-template}

Sales Insightで古くなったテンプレートをクリーンアップする日々はなくなりました。 Eメールを公開する際に有効期限を設定し、有効期限が切れた際には非公開にします。

>[!NOTE]
>
>5/31/17の有効期限を設定すると、5/31/17の終了時にSales Insightからテンプレートが削除されます。

![](assets/four-281-29.png)

## [ユーザーおよびアクティビティ用の一括抽出API](https://developers.marketo.com/rest-api/bulk-extract/) {#bulk-extract-apis-for-people-and-activities}

Marketoから外部システムに大量の人物およびアクティビティデータを簡単に転送できます。

## ABM の機能拡張 {#abm-enhancements}

**[ABM名前付きアカウントのカスタムフィールド](https://docs.marketo.com/x/1wnG)**

Marketo ABMで、名前付きアカウントに最大10個のカスタムフィールドを作成できるようになりました。 これらのカスタムフィールドをCRMアカウントオブジェクトのフィールドにマップすると、Marketo ABMがデータを同期し、ABM名前付きアカウントを拡張してマーケティングを促進できます。

**[ABM名前付きアカウントのパーセンタイル・スコアリング](https://docs.marketo.com/display/docs/assets/abmpercentiles.png)**

名前付きアカウントのスコアは大きく異なる場合があります。 Marketo ABMでは、各スコアのパーセンタイルが自動的に計算されるようになり、各ネームドアカウントが他のネームドアカウントの中でランク付けされた場所を一目で確認できます。

**[ABMアカウントリストAPI](https://developers.marketo.com/rest-api/lead-database/named-account-lists/)**

ABMパートナーとの豊富で堅牢な統合を活用し、名前付きアカウントリストの強化APIサポートを実現します。

## ウェブパーソナライゼーションの機能拡張 {#web-personalization-enhancements}

![](assets/dialogoptions.png)

**[スクロール時のWebキャンペーン](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/set-how-your-web-campaign-displays.md)**

新しいWebキャンペーンの効果により、Web訪問者は、よりパーソナライズされたエクスペリエンスを得ることができます。 Web訪問者がWebページを下にスクロールした場合にのみ表示されるように、パーソナライズしたWebキャンペーンを設定します。 次の項目に基づいて、スクロール時に表示するダイアログWebキャンペーンを設定できます。

* スクロールされたページの割合
* ピクセル到達
* ページのフォールドの下にスクロール

**[ウェブキャンペーン エグジット・インテント](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/set-how-your-web-campaign-displays.md)**

訪問者がページを閉じる前に、訪問者の注意を引きます。 訪問者がページを離れることを示すマウスジェスチャーの場合にのみ表示されるように、パーソナライズされたWebキャンペーンを設定します。

**[ウェブキャンペーン用アニメーション効果](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)**

ダイアログWebキャンペーンのアニメーション効果を設定して、Webページの開始または終了時のキャンペーンの表示方法をカスタマイズします。 6つの異なるエフェクトから選択し、ダイアログのタイミングと方向を制御できます。

![](assets/animationoptins.png)

**[ダイアログクローズボタンのカスタマイズ](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)**

ダイアログボックスの閉じるボタンをカスタマイズします。 透明ダイアログスタイルのWebキャンペーンで使用する様々なオプションから選択します。 閉じるボタンのアイコン、色、位置を選択します。 独自のボタン画像を追加することもできます。

![](assets/dialog-button-fill-5b1-5d.png)

**[ウェブキャンペーンのアーカイブ](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/archive-a-web-campaign.md)**

アーカイブは、Webキャンペーンをアーカイブし、デフォルトのWebキャンペーン表示で非表示にできる、新しいWebキャンペーンステータスです。 これにより、最も関連性の高いアクティブなキャンペーンに焦点を当て、古いアーカイブ済みキャンペーンをオンデマンドで取得できます。

![](assets/archive-campaign-5b2-5d.png)

**[多言語化対応](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md)**

Marketoでサポートされているすべての言語（英語、日本語、ドイツ語、スペイン語、フランス語、ポルトガル語）でWebパーソナライゼーションが提供されるようになりました。

## 予測の強化 {#predictive-enhancements}

**[多言語化対応](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md)**

予測コンテンツは、Marketoでサポートされているすべての言語（英語、日本語、ドイツ語、スペイン語、フランス語、ポルトガル語）で提供されるようになりました。

## [レガシーリッチテキストエディターおよびフォームエディター 1.0 の廃止](https://nation.marketo.com/docs/DOC-4315) {#legacy-rich-text-editor-and-form-editor-deprecation}

2017年8月1日以降、従来のリッチテキストエディターとフォームエディター 1.0 をまだ使用しているお客様は、新しいエクスペリエンスに自動的に移行されます。
