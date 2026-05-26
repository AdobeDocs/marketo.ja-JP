---
description: プログラムのQA、リードのインポート、データの正規化など、マーケティングタスクを自動化するために設計されたMarketoのAI エージェント群をご覧ください。
title: Marketo AIの概要
badge: ベータ版
exl-id: b89750cc-aa70-402c-9d0b-9a3e6a12a423
source-git-commit: 854fee409fb55c8f611ee85225bea6ab77036dff
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 2%

---

# Marketo AIの概要 {#overview}

MarketoのAIは、時間はかかりますが、重要なマーケティング機能を自動化するために設計されたエージェントを提供します。

>[!AVAILABILITY]
>
>この機能は限定的に利用できます。 アクセスをリクエストするには、[このフォーム ](https://forms.cloud.microsoft/Pages/ResponsePage.aspx?id=Wht7-jR7h0OUrtLBeN7O4Y-uSf63sAxCmWyqMJg8eMFUMVZSVExSNDA3T0I4SEcwRDFSVTBGWU01Uy4u&origin=QRCode){target="_blank"}に入力してください。 サブスクリプションのMunchkin IDの準備が整っていることを確認します。

>[!PREREQUISITES]
>
>この機能を使用するには、まず[Core Gen-AI条件と補足条件](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}に同意する必要があります。 詳しくは、アカウントマネージャーにお問い合わせください。

>[!IMPORTANT]
>
>この機能がサブスクリプションに対して有効になった後、必要なユーザーにアクセス権を付与するために、いくつかの[ セットアップ手順](/help/marketo/product-docs/marketo-ai/settings-setup.md){target="_blank"}を実行する必要があります。

## アクセス方法 {#access}

マイMarketo画面で、**AIでビルド** タイルをクリックします。

![](assets/overview-1.png)

プロンプトフィールドで、**開始**&#x200B;をクリックします（または独自のクエリを入力します）。

![](assets/overview-2.png)

## エージェント {#agents}

センターコンソールには、様々なタスクを支援する一連のエージェントが追加されています。 各エージェントは、特定のタスクを完了するために自然言語を通じてインタラクションを行う、専用のAI アシスタントです。

### プログラム QA {#program-qa}

プログラムのQAでは、Marketoのベストプラクティスに照らし合わせて設定が自動的にチェックされ、ローンチ前に問題が表面化されます。 [ プログラム QA エージェント ](/help/marketo/product-docs/marketo-ai/agents/program-qa.md){target="_blank"}の詳細をご覧ください。

### リードの読み込み {#import-leads}

フィールドマッピング機能を利用すれば、リードリストをMarketo Engageデータベースにインポートして重複を排除できます。 [ リードの読み込みエージェント ](/help/marketo/product-docs/marketo-ai/agents/import-leads.md){target="_blank"}について詳しく説明します。

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
