---
unique-page-id: 12983280
description: リリースノート — 17年秋 —Marketoドキュメント — 製品ドキュメント
title: リリースノート — 17年秋
exl-id: 329022e6-f388-4ff9-9724-62aeed76c0b9
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 11%

---

# リリースノート：秋&#39;17 {#release-notes-fall}

2017年秋のリリースには、次の機能が含まれています。 Marketo版で利用可能な機能を確認してください。

タイトルリンクをクリックすると、各機能に関する表示の詳細記事が表示されます。 注意：このリリースに含まれる一部の機能には、関連記事がありません。 トピックに複数のサブ見出しが含まれる場合は、そこにリンクが配置されます。

## システムの信頼性 {#system-reliability}

Marketoの基盤インフラをさらに改善しました優れた配列決定、ミスマッチの減少、マンチキンの安定性の向上などです

## SFDC 同期パフォーマンス {#sfdc-sync-performance}

MarketoとSalesforceの豊富で高速な同期を活用。 アカウントまたはリードで一括更新を必要とするデータの変更は、バックログを避けるために並列キューに分割できます。 また、イベントとタスクの同期が最大50%高速化されました。

## 分析パフォーマンスの向上 {#analytics-performance-improvements}

最近のインフラストラクチャの強化オファーにより、Marketoのレポートおよび分析ツール内でアップタイムと安定性が向上し、アドホックレポートをより迅速に作成できるようになりました。

## [受信者タイムゾーン](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

この新機能により、ローカルタイムゾーンに従って電子メールを保持し、配信できるようになりました。 電子メールおよびエンゲージメントのプログラムは、受信者のタイムゾーンで配信されるように設定でき、複数のプログラムを作成する必要がなくなります。1回送信すると、Marketoはローカルの正しい時刻まで電子メールを自動的に保持します。 電子メール指標を上昇させ、ローカルの慣行を観察し、グローバルに単一のプログラムを使用して時間を節約します。

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>電子メールおよびエンゲージメントプログラムで受信者のタイムゾーンをまだ有効にできない場合は、パニックに陥らないでください。 この機能は、すべてのお客様に対して徐々に有効になっています。

## [セグメント別サンプルメールのレビュー](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

Marketoには、レビュー用にサンプル電子メールを送信する際に、セグメントを選択する新しいオプションが追加されました。 リードが属するセグメントを手動で判断する必要がなくなり、動的なコンテンツを含む電子メールを様々なセグメントに簡単に送信できるようになりました。

## [LinkedIn リード生成カスタム質問](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

LinkedIn リード生成フォームをカスタマイズし、カスタムリード属性を収集できます。1つのフォームにつき最大3つのカスタム質問を尋ねたり、1行のテキスト入力または複数選択の質問から選択したり、Marketoのリードフィールドにマッピングしたりできるようになりました。

## [Slack統合](/help/marketo/product-docs/administration/additional-integrations/add-slack-as-a-launchpoint-service.md) {#slack-integration}

新しいSlack統合の一環として、次の2つの機能をリリースしました。

* システム通知：現在のキャンペーンのステータスや、直ちに注意を必要とする問題に関する警告など、Marketoインスタンスの重要なイベントに関するSlack通知を取得します。
* 興味深い瞬間：Marketoインサイトが営業アカウントから既知の個人によってトリガーされた場合、リードの所有者にはSlack経由で通知できます。 通知には、リード情報と営業アカウントに関する詳細が含まれます。

## ABM の機能拡張 {#abm-enhancements}

**[連絡先のないアカウントを表示](https://docs.marketo.com/x/fKCt)**

MarketoABMは、連絡先のないCRMアカウントを同期して表示するようになりました。 事前の販売またはマーケティング履歴のない新しいアカウントを含め、後続のリードをアカウントに照合して進行状況を追跡します。

## ContentAI 分析 {#contentai-analytics}

**[新しい ABM アカウントリストフィルタ](https://docs.marketo.com/x/1BPG)**

ABMアカウントリスト全体でコンテンツの表示と比較を行い、既存のコンテンツを最適化します。 ContentAIで表示される内容：

* 閲覧されたコンテンツのトップ
* トップコンバージョンコンテンツ
* マーケティングアクティビティ向けのAIベースの推奨コンテンツ

## ウェブパーソナライゼーションの機能拡張 {#web-personalization-enhancements}

**[ウェブキャンペーン用トークン](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Webキャンペーンー内でトークンを使用できるようになりました。 トークンを利用して、パーソナライズされたメッセージやコンテンツを配信し、Webキャンペーンーへの関与を増やします。

![](assets/image2017-11-16-11-3a25-3a7.png)

**[ウェブキャンペーンエディタにおけるデザインスタジオ画像](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Marketo内の複数のチャネルでクリエイティブなアセットや画像を再利用し、時間を節約できます。

![](assets/image2017-11-16-11-3a26-3a10.png)

## 統合  {#integration}

**[メールプレビュー API](https://developers.marketo.com/rest-api/assets/emails/)**

電子メールをMarketo外でリモートプレビューできるようになり、電子メールコンテンツローカライゼーションのプロセスが簡単になり、エラーを減らすことができます。

**[HTML API の置換](https://developers.marketo.com/rest-api/assets/emails/)**

開発者は、電子メールアセットのHTMLコンテンツをリモートで更新でき、単一のシステム内でアセットを管理できるようになります。
