---
description: 組織ルールによってガバナンス基準を定義する方法と、プログラムの作成、キャンペーンの計画、検証をまたいでMarketo EngageのCX Enterprise Coworkerを導く方法について説明します。
title: 組織ルール
source-git-commit: 148a0ec13abef0658048346f034ff72d9f4012b6
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 1%
---
# 組織ルール {#organizational-rules}

組織ルールは、プログラムの作成、キャンペーンの計画、検証のワークフローをまたいで、Adobe CX Enterprise Coworker for Marketo Engageを活用するための指針となる単一のドキュメントで、マーケティング業務の基準とガバナンス要件を定義します。

## 組織ルールとは？ {#what-are-organizational-rules}

組織ルールは、組織のキャンペーン標準をキャプチャするマークダウンベースの設定ドキュメントです。

* プログラム、メール、スマートキャンペーンの命名規則
* 必要なアセットと構造（フォルダー、トークン、レポート）
* コンプライアンス要件（登録解除リンク、UTM パラメーター、除外フィルター）
* ベストプラクティス（メールデザイン、スマートリスト設定）

すべてのMarketo Engage環境には、デフォルトの組織ルールが含まれています。 組織の特定のガバナンスニーズを反映するためにカスタマイズすることができます。

## 組織ルールを使用する場合 {#where-organizational-rules-are-used}

Marketo EngageのCX Enterprise Coworkerの組織ルールは、次の3つのスキルで構成されています。

| スキル | ルールの適用方法 |
| --- | --- |
| プログラムの構築 | ルールは、プログラム構造、命名、初期設定の作成をガイドします。 CX Enterprise Coworker for Marketo Engageは、プログラムを作成する前に、概要にコンプライアンスの問題があればフラグを立てます。 |
| キャンペーンの計画 | ルールは、Marketo EngageのCX Enterprise Coworkerが、基準に基づいてスマートキャンペーン、フィルター、フローステップをどのように構築するかを示します。 |
| プログラムの検証 | ルールは、アクティベーション前にプログラムを検証する際にCX Enterprise Coworker for Marketo Engageがチェックする内容を定義します。 |

## 組織ルールにアクセスしてカスタマイズする方法 {#how-to-access-and-customize-organizational-rules}

1. マイMarketoで、「**CX Enterprise Coworker Marketo Engage版**」タイルをクリックします。
1. 歯車のアイコンをクリックします。
1. 「**組織ルール**」タブを選択します。
1. デフォルトのルールを確認します（これらは、マーケティング業務のベストプラクティスが事前に入力されています）。
1. 組織のルールに合わせてルールを編集します。

   * 命名規則（プログラム、メール、キャンペーン）
   * 必要なフォルダー構造
   * 必須トークンとフィールド
   * コンプライアンスと除外基準

1. 変更を加えたときにバージョン番号を更新します。
1. 変更を保存します。 Marketo Engage版CX Enterprise Coworkerのすべてのスキルは、カスタマイズされたルールをすぐに使用します。

## 組織ルール構造 {#organizational-rules-structure}

組織ルールは、YAML frontmatterを使用してマークダウンでフォーマットされます。

```markdown
---
name: Your Organization Name - Marketo Campaign Governance
version: 1.0
enabled: true
customized: true
---

# Naming Conventions

## Programs
- Pattern: {{REGION}}_FY{{YEAR}}_{{QUARTER}}_{{TYPE}}_{{DATE}}_{{NAME}}
- Example: AMER_FY25_Q2_WBR_250315_Product_Launch_Webinar
- Region codes: AMER, EMEA, APAC, GLOBAL

## Emails
- Pattern: {{PROGRAM_NAME}}_{{SEQUENCE}}_{{PURPOSE}}
- Example: Product_Launch_01_Invitation

# Program Structure

## Required Local Folders
- 01 Emails
- 02 Smart Campaigns
- 03 Reports

## Required Tokens
- {{my.eventDate}}
- {{my.replyToEmail}}

# Email Compliance

## Required Elements
- Unsubscribe link in footer
- Company name and physical address
- All external links include UTM parameters

## Recommended Elements
- Alt text on all images
- Mobile-responsive design (600px max-width)
```

## 組織ルールのベストプラクティス {#best-practices-for-organizational-rules}

* **初期設定で開始**: カスタマイズする前に、初期設定のルールを確認してください。 マーケティングオペレーションの業界ベストプラクティスを反映しています。
* **ルールに焦点を当てる**：組織にとって重要な要件のみを含めます。 不必要なルールによってノイズが生じ、コンプライアンススコアが不必要に低下します。
* **自動チェックと手動チェックの両方を使用**:

  * 自動チェック：命名規則、必要なフォルダー、トークンの使用状況（CX Enterprise Coworker for Marketo Engageでこれらを検証できます）
  * 手作業によるチェック：電子メールのビジュアルデザイン、ブランドコンプライアンス、キャンペーンロジック（CX Enterprise Coworker for Marketo Engageでは、これらを手作業によるレビュー手順としてフラグ付けします）

* **厳格さと柔軟性のバランス**：厳格すぎるルールは、プログラムの作成が遅くなる可能性があります。 ルールが緩すぎると、重要なコンプライアンスの問題を捉えられません。
* **ルールのバージョン**: ガバナンス基準が更新されていることをチームが把握できるように、大幅な変更を行った場合はバージョン番号を更新します。
* **変更を伝える**：組織ルールを更新する際には、何が変更されたのか、その理由をマーケティング部門に伝えます。

## CX Enterprise Coworker for Marketo Engageで検証できる機能と検証できない機能 {#what-coworker-can-and-cannot-validate}

CX Enterprise Coworker for Marketo Engageでは、次の機能を検証できます（自動チェック）。

* 命名規則がパターンに一致
* 必要なフォルダー構造が存在します
* 必要なトークンが配置されている
* メールには登録解除リンクと必要なフッター要素が含まれています
* 外部リンクにはUTM パラメーターが含まれます
* スマートキャンペーン名は規則に従います

CX Enterprise Coworker for Marketo Engageは検証できません（手作業によるレビューが必要です）。

* スマートリストのフィルターロジック（APIの制限：フィルターを手動で設定する必要があります）
* Smart Campaign フローステップロジック（APIの制限：手動でフローを設定する必要があります）
* メールの視覚的なレンダリングと応答性（視覚的な検査が必要）
* ブランドコンプライアンスとメッセージングのトーン（人間の判断が必要）
* 動的コンテンツセグメンテーションルール（APIの制限）

Marketo Engage用CX Enterprise Coworkerで検証できないエラーが発生した場合は、ワークフローの手動レビューステップとしてフラグが付けられます。

## コンプライアンススコアリング {#compliance-scoring}

プログラムの検証を使用する場合、CX Enterprise Coworker for Marketo Engageは、次の項目に基づいてコンプライアンススコアを計算します。

* **合格したチェック**: Marketo Engage用CX Enterprise Coworkerがコンプライアンスを検証しましたが、問題が見つかりませんでした
* **失敗したチェック**: Marketo Engage用CX Enterprise Coworkerで、組織規則に違反していることが見つかりました
* **手動レビュー手順**：人間による検証が必要な項目（これらはスコアに対してカウントされません）

プログラムのコンプライアンスは100%に達する可能性がありますが、それでも手作業によるレビュー手順が必要です。スコアの計算から除外されます。

## 組織ルールのカスタマイズの例 {#examples-of-organizational-rules-customization}

**例1：厳密な命名規則**

```markdown
## Programs
Pattern: {{COUNTRY}}-{{BUSINESS_UNIT}}-{{CAMPAIGN_TYPE}}-FY{{YEAR}}-{{QUARTER}}-{{DATE}}
```

地域や事業部門をまたいで厳格なガバナンスを確立する必要がある場合に使用します。

**例2：必要な接頭辞を持つ柔軟な命名**

```markdown
## Programs
Pattern: {{PREFIX}}_* (where PREFIX = EMEA, AMER, APAC, GLOBAL)
Example: AMER_Q2_Product_Launch_Webinar_2025
```

地域コードに一貫性を持たせたいが、残りの部分に柔軟性を持たせたい場合に使用します。

**例3：最小限のルール（コンプライアンスに重点を置く）**

```markdown
# Email Compliance - REQUIRED

- Unsubscribe link present
- CAN-SPAM physical address in footer
- Reply-to email configured
```

組織が命名や構造の一貫性よりもコンプライアンスを優先する場合に使用します。

## トラブルシューティング {#troubleshooting}

**Q：組織ルールを更新しましたが、Marketo Engage用CX Enterprise Coworkerは古いルールを引き続き使用しています。**

A：新しいプログラムと検証の変更は、すぐに有効になります。 既存のプログラムを使用している場合は、ブラウザーを更新するか、新しいCX Enterprise Coworker for Marketo Engage ワークフローを開始して、更新されたルールを確認します。

**Q: デフォルトのルールに戻すことはできますか？**

A：はい。 **設定** > **組織ルール**&#x200B;に移動し、**デフォルトにリセット**&#x200B;をクリックします。 カスタムルールは、デフォルトのルールに置き換えられます。

**Q: プログラムは良好に見えますが、コンプライアンススコアは低いです。**

A：失敗しているチェックを確認します。 組織のルールを見直して、現在のワークフローに対して厳格すぎるか、基準を満たすためにプログラムを調整する必要があるかどうかを確認します。
