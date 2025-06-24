---
unique-page-id: 2951056
description: リリースノート - 2013年9月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2013年9月
exl-id: 43428813-0405-4c35-9165-f189fbb5ffb7
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 71%

---

# リリースノート：2013年9月 {#release-notes-september}

9 月のリリースには、次の機能が含まれています。

## URL の短縮 {#shorter-urls}

メールの URL は受信者がクリックしやすいように短縮されました。トラッキング機能はすべて保持されています

>[!CAUTION]
>
>短縮 URL に切り替えると、9 月のリリースより前に送信された電子メール内のリンクは、このリリースから 90 日で期限が切れます。

Marketo のカスタムオブジェクトのデータを使用するか、Velocity テンプレート言語を使用してメールコンテンツに条件ロジックを追加します。

![](assets/image2014-9-22-17-3a10-3a56.png)

## テスト送信をサンプル送信に変更 {#change-send-test-to-send-sample}

テストを送信アクションの名前を、サンプルを送信に変更しました。

## パーソナライズ [!UICONTROL  サンプルメールの送信 ] {#personalized-send-sample-email}

メールサンプルを送信するときに、リード名を選択してサンプルメールをパーソナライズすることができます。

![](assets/image2014-9-22-17-3a11-3a22.png)

## [!DNL GoToWebinar] の追加フィールド同期 {#additional-field-sync-for-gotowebinar}

Marketo フォームから [!DNL GoToWebinar] に会社名と役職を同期できます。 これらの追加フィールドを有効にするには、イベントパートナーに移動し、「追加フィールドを有効にする」をオンにします。

![](assets/image2014-9-22-17-3a11-3a53.png)

## ユーザーログインを SSO のみに制限 {#restrict-user-login-to-sso-only}

Marketo ユーザーが通常のログイン画面ではなく、SSO のみを使用してログインするようにサブスクリプションを設定します

## アップロード済みファイルのウィルススキャン {#virus-scan-of-uploaded-files}

デザインスタジオにアップロードされたファイルが自動的にスキャンされ、ファイルにウィルスが含まれている場合はブロックされます

## 商談の影響アナライザーのエクスポート {#export-opportunity-influence-analyzer}

これで、Opportunity Influence Analyzer のデータを [!DNL Excel] にエクスポートできます。 書き出される各 [!DNL Excel] ファイルには、すべてのリード（オポチュニティに役割がないリードを含む）のすべてのマーケティングインタラクションと、アナライザーで選択したアカウントのすべてのオポチュニティが含まれます。 商談の行は緑色でハイライト表示されます。特定のリードやマーケティングアクティビティに焦点を当てる必要がある場合は、[!DNL Excel] のネイティブのデータフィルタリング機能を使用できます。

![](assets/image2014-9-22-17-3a12-3a23.png)

## プログラムの属性設定 {#program-attribution-settings}

アカウントベースの属性付けを行う機能を含め、最初のタッチとマルチタッチの属性指標で、Marketo が連絡先と商談を連携する方法を変更できます。これらの設定は、プログラム商談分析エリアと商談分析エリアの下にある [!UICONTROL  収益エクスプローラー ] レポートのアトリビューション指標に影響を与えます。 また、プログラムアナライザーの属性指標にも影響します。

プログラムの属性設定は、3 つの選択肢の中から 1 つに変更できます。この設定を変更しても、Marketo または CRM データは変更されません。単にレポートの実行方法が変更され、いつでも元に戻すことができます。

「明示」設定では、役割を持つ連絡先のみを調べます（現在の動作）。「暗黙」設定では、役割に関係なく、アカウントに関連付けられたすべての連絡先を調べます。可能であれば、「明示」モードを使用することを強くお勧めします。「暗黙」を使用すると、商談に実際の影響を与えないにもかかわらず、商談に対してクレジットを持つ人という偽陽性を生み出す可能性があります。

![](assets/image2014-9-22-17-3a12-3a43.png)

## [!UICONTROL Insightの販売 ] フランス語およびドイツ語で提供（[!DNL Salesforce] のみ） {#sales-insight-available-in-french-and-german-salesforce-only}

Marketo Lead Management とMarketo[!UICONTROL Sales Insight] の最新版を [!DNL AppExchange] からダウンロードして、フランス語とドイツ語の販売員が [!UICONTROL Sales Insight] のコンテンツを優先言語で閲覧できるようにします。

![](assets/image2014-9-22-17-3a13-3a12.png)

## Cobalt ユーザーインターフェイス {#cobalt-user-interface}

向こう数か月のうちに、アプリケーションの様々な部分の新規テーマが公開される予定です。今月は、新しい青いモーダルウィンドウがさらに表示される場合があります。
