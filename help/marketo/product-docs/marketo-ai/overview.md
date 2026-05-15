---
description: プログラムのQA、リードのインポート、データの正規化など、マーケティングタスクを自動化するために設計されたMarketo EngageのAI エージェント群をご覧ください。
title: Marketo Engage AIの概要
badge: ベータ版
exl-id: b89750cc-aa70-402c-9d0b-9a3e6a12a423
source-git-commit: f552c0b0219aede39e0742466ab2473e8e924e55
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 2%

---

# Marketo Engage AIの概要 {#overview}

Marketo EngageのAIは、時間はかかりますが、重要なマーケティング機能を自動化するために設計されたエージェントを提供します。

>[!PREREQUISITES]
>
>この機能を使用するには、まず[Core Gen-AI条件と補足条件](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}に同意する必要があります。 詳しくは、Adobe アカウントチーム（アカウントマネージャー）にお問い合わせください。

>[!NOTE]
>
>この機能はクローズド版であり、現在数か月にわたって段階的に展開されています。 My Marketo画面に&#x200B;_AIでビルド_ タイルが表示されたら、サブスクリプションが有効になったときにわかります。

>[!IMPORTANT]
>
>この機能がサブスクリプションに対して有効になった後、必要なユーザーにアクセス権を付与するために、いくつかの[&#x200B; セットアップ手順](/help/marketo/product-docs/marketo-ai/settings-setup.md)を実行する必要があります。

## アクセス方法 {#access}

マイMarketo画面で、**AIでビルド** タイルをクリックします。

![](assets/overview-1.png)

プロンプトフィールドで、**開始**&#x200B;をクリックします（または独自のクエリを入力します）。

![](assets/overview-2.png)

## エージェント {#agents}

センターコンソールには、様々なタスクを支援する一連のエージェントが追加されています。 各エージェントは、特定のタスクを完了するために自然言語を通じてインタラクションを行う、専用のAI アシスタントです。

### プログラム QA {#program-qa}

プログラムのQAでは、Marketoのベストプラクティスに照らし合わせて設定が自動的にチェックされ、ローンチ前に問題が表面化されます。 [&#x200B; プログラム QA エージェント &#x200B;](/help/marketo/product-docs/marketo-ai/agents/program-qa.md){target="_blank"}の詳細をご覧ください。

### リードの読み込み {#import-leads}

フィールドマッピング機能を利用すれば、リードリストをMarketo Engageデータベースにインポートして重複を排除できます。 [&#x200B; リードの読み込みエージェント &#x200B;](/help/marketo/product-docs/marketo-ai/agents/import-leads.md){target="_blank"}について詳しく説明します。

## 近日リリース予定 {#coming-soon}

最も反復的で時間のかかる作業を処理するために設計された追加のエージェントが、近日リリースされる予定です。

* リードがMQLを実行しなかった理由や、ライフサイクルを先に進めた理由を診断します。
* キャンペーン概要から、包括的なMarketo Engageプログラムを直接生成できます。
* その他。

<!--

### Investigate Lead (Coming soon) {#investigate-lead}

Discover why someone didn't MQL, qualify for a program, or progress through the lifecycle.

### Plan Program (Coming soon) {#plan-program}

Create a program setup document for others to use from a campaign brief.

### Create Program (Coming soon) {#create-program}

Generate an entire Marketo Engage program using a campaign brief, complete with email, landing page, and Smart Campaign.

### Normalize data (Coming soon) {#normalize-data}

Standardize fields such as company name, job title, country, and more.

### Callable agents (Coming soon) {#callable-agents}

These agents run as webhooks in Marketo Engage Smart Campaigns for real-time data processing.

-->
