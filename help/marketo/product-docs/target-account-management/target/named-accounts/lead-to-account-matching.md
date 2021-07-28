---
unique-page-id: 11381156
description: アカウントの照合のお知らせ — Marketoドキュメント — 製品ドキュメント
title: アカウントの照合へのリード
exl-id: 676ae500-7691-492d-abec-0cac708216b7
source-git-commit: 98388f1ed941b321449e6e8badac0153dc2245ba
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 2%

---

# アカウントの照合へのリード {#lead-to-account-matching}

「一致」は、Marketoの「リードツーアカウント」の照合を使用して、適切な名前のアカウントに導きます。

>[!NOTE]
>
>**リードツーアカウントのマ** ッチングは、Marketo Targetのアカウント管理の組み込み機能です。あいまいなロジックを使用して、ほぼリアルタイムで適切な名前のアカウントにリードを自動的に一致させます。 これらの名前付きアカウントは、CRMアカウントまたはMarketoの会社です。

## 概要 {#overview}

Marketoのリードツーアカウントの照合は、次の4つの手順に従います。

**手順1 -** リードレコードに関する次のような重要な情報を使用して、照合プロセスを開始します。

* 電子メールドメイン（acme.comなど）
* IPアドレスから推測された会社名
* 会社名 — CRMアカウント名またはリード会社名属性（フォームの入力から取得したものなど）

**手順2 -** 様々なリード属性に基づいて見つけた会社名を正規化します（例：Acme Inc.およびAcme Corpは、自動的にAcmeに正規化されます）。この手順では、Marketoで名前付きアカウントが1つで表示され、1つの名前付きアカウント内のすべてのリードを確認できます。

**手順3 — 一致したリ** ードを2つのバケットに分割します。強い試合と弱い試合。

* 名前の付いたアカウントに弱い一致のリードが表示され、手動で解決できます。

**ステップ4 -** 我々は、強いマッチと弱いマッチを持つ提案企業のリストを提示する。提案された会社の1つに基づいて名前付きアカウントを作成する場合、一致するルールを作成し、適切な名前のアカウントに進む新しいリード（例えば、フォームに記入したリード）を自動的に関連付けます。 これにより、リードの一致や収益の獲得に関して心配する必要がなくなります。

MarketoのLead-to-Account MatchingはMarketo Target Account Managementの組み込み機能なので、Adobe Targetのアカウントとのマッチングは、ほぼリアルタイムでおこなわれます(例えば、リードがMarketoフォームに記入した瞬間に、適切なアカウントと関連付けます)。 このイベントを使用して、アラートをトリガーし、指定されたアカウントから新しくリードが届くことをアカウントの所有者に通知できます。

>[!NOTE]
>
>SalesforceのLeanDataを使用してリードツーアカウントの照合をおこなう場合、Marketoは、Marketoインスタンスに一致するものを同期する統合機能を備えています。 この機能を有効にするには、[Marketoサポート](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。以下のLeanDataの設定方法をご覧ください。

## リードからアカウントへの照合にLeanDataを使用 {#using-leandata-for-lead-to-account-matching}

[Marketoサポート](https://nation.marketo.com/t5/Support/ct-p/Support)がお使いのアカウントでLeanDataを有効にしたら、以下の手順に従って設定します。

1. Salesforceで、左側のナビゲーションで「**Setup Home**」をクリックします。

1. 左側のナビゲーションの「管理」で、「**ユーザー**」、「**プロファイル**」の順にクリックします。

1. **Marketo Sync**&#x200B;プロファイルを探して選択します。

1. 下の「フィールドレベルのセキュリティ」セクションまでスクロールし、リードオブジェクトを見つけます。 **表示**&#x200B;を選択します。

1. フィールド名「Reporting Matched Account」に対して、「**Read Access**」列のチェックボックスがオンになっていることを確認します。

1. Marketoで、**Admin**&#x200B;セクションに移動します。

   ![](assets/lead-to-account-matching-1.png)

1. 「**フィールド管理**」を選択します。

   ![](assets/lead-to-account-matching-2.png)

1. 「一致するアカウントをレポート」を検索して、フィールドがあることを確認します。

   ![](assets/lead-to-account-matching-3.png)

>[!MORELIKETHIS]
[アカウントの検出](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md)>
>
