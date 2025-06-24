---
unique-page-id: 12255606
description: リリースノート - 17年冬 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 17年冬
exl-id: b76dab24-43be-4d13-b4dc-b199e3e8f9a2
source-git-commit: 2b72932606a93d061eb2f57c0ff3256b94a0c20c
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 71%

---

# リリースノート：2017年冬 {#release-notes-winter}

17年冬リリースには、次の機能が含まれています。利用可能な機能についてはお使いの Marketo のエディションをご確認ください。

各機能の詳細な記事を表示するには、タイトルリンクをクリックしてください。

>[!NOTE]
>
>トピックに複数のサブ見出しが含まれる場合、リンクはそこに配置されます。

## [Facebook カスタムオーディエンスの詳細照合](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) {#advanced-matching-for-facebook-custom-audiences}

「基本的な一致」ではメールアドレスのみが使用されますが、新しい「高度な一致」では 7 つのフィールドが追加され、コンバージョン率が向上します。

![](assets/fb-custom-audiences-schebsches.png)

## [カスタムオブジェクト読み込み API](https://developers.marketo.com/rest-api/lead-database/custom-objects/) {#custom-object-import-api}

この API は、カスタムオブジェクトを Marketo に同期する高速なインターフェイスを提供します。CSV、TSV または SSV スプレッドシートファイルは、カスタムオブジェクトとして Marketo に読み込むことができます。

## [ウェブパーソナライズキャンペーンの書き出し](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/export-web-campaign-data.md) {#web-personalization-campaigns-export}

すべての web キャンペーンの詳細と分析を CSV 形式で書き出します。その後、データを便利なレイアウトで表示できます。

![](assets/web-personalization-csv-download-hand.png)

## 多言語化対応 {#localization}

Web Personalization、[!UICONTROL &#x200B; 予測コンテンツ &#x200B;] およびメールインサイトの各アプリが、日本語、ドイツ語、スペイン語で利用できるようになりました。 [言語とロケールを選択](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md)して、これらの言語でコンテンツを表示します。

![](assets/japanese-web-personalization.png)

## アカウントベースのマーケティングの強化 {#account-based-marketing-enhancements}

**[重点顧客のインポート](/help/marketo/product-docs/target-account-management/target/named-accounts/import-named-accounts.md)**

[!UICONTROL &#x200B; 指定アカウント &#x200B;] 読み込みオプションを使用し、CSV アップロードで一度に複数のレコードを作成または更新します。

![](assets/inatwo.png)

**[メールインサイトのサポート](/help/marketo/product-docs/reporting/email-insights/filtering-in-email-insights.md)**

メールインサイトのディメンションとして [!UICONTROL &#x200B; 名前付きアカウント &#x200B;] または [!UICONTROL &#x200B; アカウントリスト &#x200B;] を使用します。

![](assets/ei.png)

## [!UICONTROL &#x200B; 予測コンテンツ &#x200B;] 機能の強化 {#predictive-content-enhancements}

**[有効なSource[!UICONTROL &#x200B; でフィルタリング]](/help/marketo/product-docs/predictive-content/working-with-predictive-content/understanding-predictive-content.md)**

[!UICONTROL &#x200B; メール &#x200B;]、[!UICONTROL &#x200B; リッチメディア &#x200B;] または [!UICONTROL &#x200B; レコメンデーションバー [!UICONTROL &#x200B; に対して有効な &#x200B;] 予測コンテンツ &#x200B;] をフィルタリングします。

![](assets/predictive-content-enabled-source.png)

**[フィルター [!UICONTROL Sourceによる Analytics]](/help/marketo/product-docs/predictive-content/working-with-predictive-content/understanding-predictive-content.md)**

特定のソース（[!UICONTROL &#x200B; メール &#x200B;]、[!UICONTROL &#x200B; リッチメディア &#x200B;]、または [!UICONTROL &#x200B; レコメンデーションバー &#x200B;] に対するフィルター [!UICONTROL &#x200B; 予測コンテンツ &#x200B;] 分析。

![](assets/predictive-content-analytics-by-source.png)

**[!UICONTROL 予測コンテンツ &#x200B;] エディター**

編集エクスペリエンスとレイアウトが改善され、ソース（[!UICONTROL &#x200B; メール &#x200B;]、[!UICONTROL &#x200B; リッチメディア &#x200B;]、[!UICONTROL &#x200B; レコメンデーションバー &#x200B;] によってコンテンツの準備が分割されます。

![](assets/predictive-content-editor.png)

**[予測のためのコンテンツ自動検出](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md)**

コンテンツの自動検出プロセスで、画像 URL とメタデータが使用されるようになりました。

## [SDK の強化](https://developers.marketo.com/mobile/) {#sdk-enhancements}

開発者は、新しい SDK API 呼び出しを追加して、プッシュ通知の配信を制御できるようになりました。これにより、開発者はプッシュトークンを削除することができます。

## Vibes SMS LaunchPoint の統合

新しいフィルターオプション「Vibes リストのメンバー」でターゲティングを強化します。

## [レガシーリッチテキストエディターおよびフォームエディター 1.0 の廃止](https://nation.marketo.com/docs/DOC-4315) {#legacy-rich-text-editor-and-form-editor-deprecation}

2017年8月1日以降、従来のリッチテキストエディターとフォームエディター 1.0 をまだ使用しているお客様は、新しいエクスペリエンスに自動的に移行されます。

## [Marketo アクティビティ API](https://developers.marketo.com/blog/important-change-activity-records-marketo-apis/) {#marketo-activity-apis}

Marketo のアクティビティ API に重要な変更が予定されています。準備はよろしいでしょうか。
