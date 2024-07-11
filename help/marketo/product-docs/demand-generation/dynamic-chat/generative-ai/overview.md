---
description: ジェネレーティブ AI の概要 – Marketo ドキュメント – 製品ドキュメント
title: 生成 AI の概要
feature: Dynamic Chat
exl-id: 2ec6409b-f2c8-42a4-94e0-5d2cd331a0a6
source-git-commit: 338f7ab16b3eea1a5d9777ca5283a1b1629376e6
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 10%

---

# 生成 AI の概要 {#generative-ai-overview}

Adobe Dynamic Chatのジェネレーティブ AI を活用した機能により、営業担当者の生産性を最適化し、Web サイトの訪問者の意図に関するインサイトを得て、訪問者の質問に安全な方法で対応できます。

## 権限 {#permissions}

生成 AI を使用するには、目的のユーザーに適切な権限を付与してください [権限](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md).

![](assets/generative-ai-overview-1.png)

## 生成応答カード {#generation-response-card}

訪問者が会話の特定の時点に達したときのメッセージを作成します。必要な主要業績評価指標を達成するために、1 回の操作で尋ねることができる質問をいくつか設定します。 最大 5 つのフォローアップ質問を追加し、訪問者の質問に対する応答がない場合はフォールバックメッセージを含めます。

![](assets/generative-ai-overview-2.png)

## 会話の概要 {#conversation-summary}

通常、訪問者の会話のコンテキスト全体を取得するには、チャットトランスクリプト全体をスクロールする必要があります。 会話の概要では、リアルタイムで概要が生成され、訪問者が興味を示したトピックも含まれます。 これは、複数の訪問者とのチャットを切り替える際に、会話のコンテキストをすばやく把握する必要があるチャットエージェントで特に役立ちます。 エージェントのインボックスチャット画面に表示されるほか、完了した会話概要は、Marketo Engageデータベース内の訪問者のユーザーレコードのアクティビティログにも表示されます。

![](assets/generative-ai-overview-3.png)

![](assets/generative-ai-overview-4.png)

>[!NOTE]
>
>会話の概要は、ライブチャットと自動チャットの両方について生成されます。

## 質問の生成 {#question-generation}

[インバウンドエクスペリエンスの昇格](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/question-generation.md) と、販売、マーケティング、製品の知識でトレーニングされたインターフェイスを使用した、訪問者向けの AI 支援の会話。

![](assets/generative-ai-overview-5.png)

## 回答ライブラリ {#response-library}

[カスタマイズされたコレクションの生成](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md) の質問と回答（すべての事前承認）をジェネレーティブ AI チャットキャンペーン内で使用できます。

![](assets/generative-ai-overview-6.png)

## アクティビティログ {#activity-log}

[すべてのタスクのリストを表示](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/activity-log.md) 名前、所有者、タイプ、編集者、編集者の日時など、それに伴う詳細。

![](assets/generative-ai-overview-7.png)

## 未回答の質問 {#unanswered-questions}

[追加の事前承認済み応答の作成](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/unanswered-questions.md) 以前の会話から回答のない質問のリポジトリに基づく AI を使用している応答ライブラリの場合。

![](assets/generative-ai-overview-8.png)

## 議論されたトピック {#discussed-topics}

ディスカッショントピックは、スマートリストトリガーとフィルターで制約として使用でき、Dynamic Chatインサイトをさらに詳しく掘り下げることができます。

![](assets/generative-ai-overview-9.png)

>[!IMPORTANT]
>
>生成 AI を使用する場合は、を遵守する必要があります [Adobe Experience Cloud ジェネレーティブ AI ユーザーガイドライン](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) そのため、生成 AI を組み込んだAdobe Experience Cloud機能が、安全かつ責任ある方法で使用されていることを確認できます。

## よくある質問 {#faq}

**ジェネレーティブ AI はすべてのDynamic Chat ユーザーが利用できますか？**

ジェネレーティブ AI は、Dynamic Chatプライムのサブスクライバーのみが使用できます。 詳しくは、アドビのアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

**生成できる質問と回答の量に制限はありますか？**

あります。この時点では、ライフタイム制限は 1000 です。

**生成 AI では、どのような言語が利用できますか？**

現在、生成 AI では英語のみがサポートされています。
