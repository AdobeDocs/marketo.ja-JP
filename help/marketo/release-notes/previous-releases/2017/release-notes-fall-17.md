---
unique-page-id: 12983280
description: リリースノート - 2017 年秋 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2017 年秋
exl-id: 329022e6-f388-4ff9-9724-62aeed76c0b9
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 100%

---

# リリースノート：2017 年秋 {#release-notes-fall}

17 年秋リリースには、次の機能が含まれています。機能の可用性についてはお使いの Marketo のエディションをご確認ください。

各機能の詳細な記事を表示するには、タイトルリンクをクリックしてください。注意：このリリースに含まれる機能の一部には、関連記事がありません。トピックに複数のサブ見出しが含まれる場合、リンクはそこに配置されます。

## システムの信頼性 {#system-reliability}

Marketo のコアインフラストラクチャをさらに改善し、シーケンシングの改善、ミスマッチの削減、Munchkin の安定性の向上を行いました。

## SFDC 同期パフォーマンス {#sfdc-sync-performance}

Marketo と Salesforce の豊富で高速な同期を活用できます。顧客やリードで一括更新が必要なデータ変更は、バックログを避けるために、並列キューに分割できます。イベントとタスクの同期速度が最大で 50% 向上しています。

## 分析パフォーマンスの向上 {#analytics-performance-improvements}

最近のインフラストラクチャの改善により、Marketo のレポートと分析ツール内の稼動時間と安定性が向上し、臨時のレポートをより迅速に作成できるようになりました。

## [受信者タイムゾーン](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

この新機能を使用すると、ローカルタイムゾーンに応じてメールを保留して配信できるようになります。メールおよびエンゲージメントプログラムは、受信者のタイムゾーンで配信するように設定できるので、複数のプログラムを作成する必要がなくなります。一度送信すると、メールは自動的にローカルで正しい時間まで保持されます。グローバルに 1 つのプログラムを使用して、メール指標を改善し、ローカルプラクティスを観察し、時間を節約します。

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>メールやエンゲージメントプログラムで受信者タイムゾーンを有効にできない場合は、パニックを起こす必要はありません。この機能は、すべてのお客様に対して徐々に有効化されています。

## [セグメント別サンプルメールのレビュー](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

Marketo には、レビュー用にサンプルメールを送信する際にセグメントを選択する新しいオプションが追加されました。リードが属するセグメントを手動で決定する必要がなくなり、動的コンテンツを含むメールを様々なセグメントに簡単に送信できるようになりました。

## [LinkedIn リード生成カスタム質問](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

LinkedIn リード生成フォームをカスタマイズし、カスタムリード属性を収集できます。1 つのフォームにつき最大 3 つのカスタム質問をして、1 行のテキスト入力または複数選択の質問から選択、Marketo リードフィールドにマッピングできるようになりました。

## Slack 統合 {#slack-integration}

新しい Slack 統合の一環として、次の 2 つの機能をリリースしました。

* システム通知：現在のキャンペーンステータスや早急な対応が必要な問題に関するアラートなど、Marketo インスタンスの重要なイベントに関する Slack 通知を受け取ります。
* 注目のアクション：Marketo Insight がセールスアカウントの既知の個人によってトリガーされた場合、リードの所有者は Slack 経由で通知を受け取ることができます。通知には、リード情報とセールスアカウントに関する詳細が含まれます。

## ABM の機能拡張 {#abm-enhancements}

**[連絡先のないアカウントを表示](https://docs.marketo.com/x/fKCt)**

Marketo ABM が連絡先のない CRM アカウントを同期し、表示するようになりました。以前の販売またはマーケティング履歴のない新規アカウントを含め、後続のリードをアカウントに一致させて進捗を追跡します。

## ContentAI 分析 {#contentai-analytics}

**[新しい ABM アカウントリストフィルタ](https://docs.marketo.com/x/1BPG)**

ABM アカウントリスト全体でコンテンツのパフォーマンスを表示および比較して、既存のコンテンツを最適化します。ContentAI には次の情報が表示されます。

* 閲覧されたコンテンツの数
* 上位の変換済みコンテンツ
* AI を利用したマーケティングアクティビティ用の推奨コンテンツ

## ウェブパーソナライズの機能拡張 {#web-personalization-enhancements}

**[ウェブキャンペーン用トークン](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Web キャンペーンでトークンを使用できるようになりました。トークンを活用してパーソナライズされたメッセージやコンテンツを配信し、web キャンペーンでのエンゲージメントを高めます。

![](assets/image2017-11-16-11-3a25-3a7.png)

**[ウェブキャンペーンエディタにおけるデザインスタジオ画像](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Marketo 内の複数のチャネルでクリエイティブアセットと画像を再利用することで、時間を節約できます。

![](assets/image2017-11-16-11-3a26-3a10.png)

## 統合  {#integration}

**[メールプレビュー API](https://developers.marketo.com/rest-api/assets/emails/)**

メールを Marketo 外でリモートでプレビューできるようになり、メールコンテンツのローカライゼーションのプロセスが簡単になり、エラーを減らすことができます。

**[HTML API の置換](https://developers.marketo.com/rest-api/assets/emails/)**

デベロッパーは、メール HTML のアセットコンテンツをリモートで更新でき、1 つのシステム内で作業してアセットを管理できます。
