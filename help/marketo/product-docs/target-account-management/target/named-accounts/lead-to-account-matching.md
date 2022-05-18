---
unique-page-id: 11381156
description: リードと顧客の照合 - Marketo ドキュメント - 製品ドキュメント
title: リードと顧客の照合
exl-id: 676ae500-7691-492d-abec-0cac708216b7
source-git-commit: 98388f1ed941b321449e6e8badac0153dc2245ba
workflow-type: ht
source-wordcount: '474'
ht-degree: 100%

---

# リードと顧客の照合 {#lead-to-account-matching}

Marketo のリードと顧客の照合を使用して、適切なリードを適切な重点顧客に照合します。

>[!NOTE]
>
>**リードと顧客の照合**&#x200B;は、Marketo ターゲット顧客管理の組み込み機能です。ファジィ論理を使用して、ほぼリアルタイムで適切な重点顧客にリードを自動的に一致させます。これらの重点顧客は、CRM アカウントまたは Marketo の会社です。

## 概要 {#overview}

Marketo のリードと顧客の照合は、次の 4 つの手順に従います。

**手順 1：**&#x200B;照合プロセスは、次のようなリードレコードの主要情報を使用して開始されます。

* メールドメイン（例：acme.com）
* 推測される会社名（IP アドレスから）
* 会社名 — CRM 顧客名またはリード会社名属性（フォームの入力からの場合など）

**手順 2：** 様々なリード属性に基づいて見つけた会社名を標準化します（例：Acme Inc.や Acme Corp は、自動的に Acme に正規化されます）。この手順では、Marketo に重点顧客の単一の表現が存在し、1 つの特定顧客内のすべてのリードを確認できます。

**手順 3**：一致したリードを 2 つのバケット（強い一致と弱い一致）に分割しました。

* 一致のないリードが重点顧客に表示され、手動で解決できます。

**手順 4**：強い一致と弱い一致を持つ提案企業のリストを提示します。提案された会社の 1 つに基づいて重点顧客を作成する場合、一致するルールを作成して、新規リード（例：フォームに入力されたリード）を適切な重点顧客に自動的に関連付けます。これにより、リードの照合の心配を減らし、収益の獲得についての心配を減らすことができます。

Marketo のリードと顧客の照合は Marketo ターゲット顧客管理の組み込み機能なので、ほぼリアルタイムでおこなわれます（例えば、リードが Marketo フォームに入力した瞬間に、適切な重点顧客と関連付けます）。このイベントを使用して、アラートをトリガーし、顧客の所有者に対して、重点顧客からの新規リードの通知をおこなうことができます。

>[!NOTE]
>
>Salesforce の LeanData を使用してリードと顧客の照合をおこなう場合、Marketo は、Marketo インスタンスとの一致を同期する統合を備えています。この機能を有効にするには、[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)に問い合わせてください。以下で LeanData の設定方法を説明します。

## リードと顧客の照合に LeanData を使用 {#using-leandata-for-lead-to-account-matching}

[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)がお使いのアカウントで LeanData を有効にした後、以下の手順に従って設定します。

1. Salesforce の左側のナビゲーションで、**セットアップホーム**&#x200B;をクリックします。

1. 左側のナビゲーションにある管理の下で&#x200B;**ユーザー**／**プロファイル**&#x200B;をクリックします。

1. **Marketo 同期**&#x200B;プロファイルを見つけて選択します。

1. 下のフィールドレベルのセキュリティセクションまでスクロールし、リードオブジェクトを見つけます。**ビュー**&#x200B;を選択します。

1. フィールド名が「Reporting Matched Account」である場合は、**読み取りアクセス**&#x200B;列のチェックボックスが選択されていることを確認してください。

1. Marketo で、**管理**&#x200B;セクションに移動します。

   ![](assets/lead-to-account-matching-1.png)

1. 「**フィールド管理**」を選択します。

   ![](assets/lead-to-account-matching-2.png)

1. 「Reporting Matched Account」を検索して、フィールドが存在することを確認します。

   ![](assets/lead-to-account-matching-3.png)

>[!MORELIKETHIS]
>
>[アカウントの検出](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md)
