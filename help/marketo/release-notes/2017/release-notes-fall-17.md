---
unique-page-id: 12983280
description: リリースノート — 17年秋 — Marketoドキュメント — 製品ドキュメント
title: リリースノート — 17年秋
exl-id: 329022e6-f388-4ff9-9724-62aeed76c0b9
source-git-commit: cbfa6110e85c185a5b65342052f168d9715f2f6a
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# リリースノート：17年秋 {#release-notes-fall}

17年秋のリリースには、次の機能が含まれています。 お客様のご契約により、制限やオプションの契約が必要なものがあります。詳細は担当の営業にお問い合わせください。

各機能の詳細な記事を表示するには、タイトルリンクをクリックしてください。 注意：このリリースに含まれる機能の一部には、関連記事がありません。 トピックに複数のサブ見出しが含まれる場合、リンクはそこに配置されます。

## システムの信頼性 {#system-reliability}

Marketoの主要インフラストラクチャをさらに改善し、優れたシーケンス化、ミスマッチの削減、Munchkinの安定性の向上などを行いました。

## SFDC 同期パフォーマンス {#sfdc-sync-performance}

MarketoとSalesforceの豊富で高速な同期を活用できます。 アカウントやリードの一括更新を必要とするデータ変更は、バックログを避けるために、並列キューに分割できます。 また、イベントとタスクの同期が最大50%高速化されました。

## 分析パフォーマンスの向上 {#analytics-performance-improvements}

最近のインフラストラクチャの改善により、Marketoのレポートおよび分析ツール内の稼動時間と安定性が向上し、アドホックなレポートをより迅速に作成できます。

## [受信者タイムゾーン](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

この新機能により、ローカルのタイムゾーンに従ってEメールを保持し、配信できるようになりました。 Eメールおよびエンゲージメントプログラムは、受信者のタイムゾーンに配信するように設定でき、複数のプログラムを作成する必要がなくなります。1回送信すると、Marketoはローカル時間が正しくなるまでEメールを自動的に保持します。 グローバルに1つのプログラムを使用して、Eメール指標を改善し、ローカルのプラクティスを確認し、時間を節約します。

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>Eメールとエンゲージメントプログラムで受信者のタイムゾーンを有効にできない場合は、パニックに陥らないでください。 この機能は、徐々にすべてのお客様に対して有効化されています。

## [セグメント別サンプルメールのレビュー](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

Marketoでは、確認用にEメールのサンプルを送信する際にセグメントを選択する新しいオプションが追加されました。 リードが属するセグメントを手動で決定する必要がなくなり、動的コンテンツを含むEメールを様々なセグメントに簡単に送信できます。

## [LinkedIn リード生成カスタム質問](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

LinkedIn リード生成フォームをカスタマイズし、カスタムリード属性を収集できます。1つのフォームにつき最大3つのカスタム質問を問い合わせ、1行のテキスト入力または複数選択の質問から選択し、Marketoのリードフィールドにマッピングできるようになりました。

## Slackの統合 {#slack-integration}

新しい機能統合の一環として、次の2つのSlackをリリースしました。

* システム通知：現在のSlackのステータスに関するアラートや、すぐに対処する必要がある問題など、Marketoインスタンスの重要なイベントに関するアラート通知を取得します。
* 興味深い瞬間：Marketo Insightがセールスアカウントの既知の個人によってトリガーされた場合、リードの所有者には、Slackで通知できます。 通知には、リード情報と、営業アカウントに関する詳細が含まれます。

## ABM の機能拡張 {#abm-enhancements}

**[連絡先のないアカウントを表示](https://docs.marketo.com/x/fKCt)**

Marketo ABMは、連絡先のないCRMアカウントを同期して表示するようになりました。 先行販売またはマーケティング履歴のない新しいアカウントを含め、後続のリードをアカウントに照合して進捗状況を追跡します。

## ContentAI 分析 {#contentai-analytics}

**[新しい ABM アカウントリストフィルタ](https://docs.marketo.com/x/1BPG)**

ABMアカウント・リスト全体のコンテンツ・パフォーマンスを表示および比較して、既存のコンテンツを最適化します。 ContentAIには次の内容が表示されます。

* 閲覧されたコンテンツの数
* 上位コンバージョンコンテンツ
* マーケティングアクティビティに関するAIを活用した推奨コンテンツ

## ウェブパーソナライゼーションの機能拡張 {#web-personalization-enhancements}

**[ウェブキャンペーン用トークン](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Webキャンペーン内でトークンを使用できるようになりました。 トークンを活用して、パーソナライズされたメッセージとコンテンツを配信し、Webキャンペーンのエンゲージメントを高めます。

![](assets/image2017-11-16-11-3a25-3a7.png)

**[ウェブキャンペーンエディタにおけるデザインスタジオ画像](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Marketo内の複数のチャネルでクリエイティブなアセットと画像を再利用することで、時間を節約できます。

![](assets/image2017-11-16-11-3a26-3a10.png)

## 統合  {#integration}

**[メールプレビュー API](https://developers.marketo.com/rest-api/assets/emails/)**

Marketo以外でEメールをリモートでプレビューできるようになり、Eメールコンテンツのローカライゼーションのプロセスが簡単になり、エラーを減らすことができます。

**[HTML API の置換](https://developers.marketo.com/rest-api/assets/emails/)**

開発者は、電子メールアセットのHTMLコンテンツをリモートで更新でき、単一のシステム内で作業してアセットを管理できます。
