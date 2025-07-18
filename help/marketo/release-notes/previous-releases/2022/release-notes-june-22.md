---
description: リリースノート - 2022年6月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2022年6月
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: ht
source-wordcount: '600'
ht-degree: 100%

---

# リリースノート：2022年6月 {#release-notes-june-22}

以下に、2022年6月リリースに含まれるすべての機能を示します。利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

>[!AVAILABILITY]
>
>星（![星](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

以下の機能のリリースは、**2022年6月24日**（PT）に始まり、（特に指定のない限り）その次の週から残りの機能が段階的にロールアウトされます。

## マーケティングデータ環境 {#marketing-data-environment}

* **カスタムオブジェクトの CreatedAt／UpdatedAt フィールドの公開**：人物の詳細画面でこれらのフィールドを調べて、さらなるインサイトを得ることができます。

## クロスチャネルオーケストレーション {#cross-channel-orchestration}

* **[!DNL Dynamic Chat]** のストリームデザイナーの使いやすさの向上：ドラッグ＆ドロップを必要とせずに、ストリームデザイナーのキャンバスから直接カードを追加できます。また、[!DNL Dynamic Chat] インターフェイスを改良し、個々のカードでのコンテンツの可視性が向上しました。

* **[!DNL Dynamic Chat]** の高度な予定ルーティングルール：[!DNL Dynamic Chat] は、ターゲットの予定ルーティングに対してさらに多くのオプションを提供します。Marketo Engage の属性に基づいてルーティングするエージェントの予定を指定し、リードを適切なエージェントにルーティングします。

* **[!DNL Dynamic Chat]** の高度なダイアログレポート：エンゲージメント指標とコンバージョン指標に関する新しいデータビジュアライゼーションを使用して、[!DNL Dynamic Chat] のキャンペーン効果をより詳しく表示します。

* **[!DNL Dynamic Chat]** で使用されない Marketo Engage 属性の同期解除：[!DNL Dynamic Chat] サブスクリプションから未使用の Marketo Engage 属性の同期を解除することで、データを簡単に整理でき、必要に応じて代替の属性を同期できます。

## 次世代のエクスペリエンス

**新しい切替スイッチ表示**：次世代のエクスペリエンスで、以下の表示を利用できるようになりました。

* [メールの詳細表示](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [メールのリスト表示](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## エクスペリエンスの自動化 {#experience-automation}

* **グローバルフォームフィールド検証ルールの除外**：グローバルフォーム検証ルールから特定のフォームを除外して、サブスクリプションセンターや他のビジネスクリティカルなワークフローがすべての値を受け入れるようにします。

* **セルフサービスのフローステップ**：スマートキャンペーンで使用するカスタマイズされたフローステップを作成する機能により、Marketo Engage とスタックの他の部分との接続性を拡張できます。Marketo Engage のユーザとパートナーの両方がこの機能を活用して、トリガーキャンペーンでのみ使用できる web フックとは異なり、トリガー、バッチ、実行可能なキャンペーンで外部の web サービスを使用できます。

* **Munchkin プロトコル非依存リンクトラッキング**：Munchkin による `tel` と `mailto` のリンクトラッキングのサポートを拡張して、展開された一連の web 動作をトラックします。

* **Webhook 用の追加の HTTP メソッド**：Web サービスとやり取りするリクエストの種類として、PUT、PATCH、DELETE を指定します。

## [!DNL Sales Insight] {#sales-insight}

![（星印）](assets/yellow-star.png)

* **[!DNL Sales Insight][!DNL Salesforce]** での権限セット：管理者は、[!DNL Sales Insight] [!DNL Salesforce] パッケージの一部である Marketo アプリ権限セットを使用して、プロファイルレベルではなく、ユーザレベルで限られた一連のユーザに対して [!DNL Sales Insight] のアクセス権を提供できます。

* **My Marketo タイルのアップデート - [!DNL Sales Insight]アクション**：Marketo 管理者（および指定したユーザ）は、マイ Marketo ページにある新しい [!DNL Sales Insight] アクションタイルから、[!DNL Sales Insight] アクションインスタンスにすばやく移動できるようになりました。

## [!DNL Sales Connect] {#sales-connect}

![（星印）](assets/yellow-star.png)

* **[!DNL Salesforce]API のアップデート**：[!DNL Salesforce] 2022 年夏のリリースで、[!DNL Salesforce] は API のレガシーバージョン 21～30 のサポートを終了します。この Marketo Engage リリースにより、API のレガシーバージョンを使用する [!DNL Sales Connect] リクエストがすべてアップデートされ、サポート対象バージョン内に含まれるようになります。[!DNL Salesforce] API 廃止プランについて詳しくは、[こちら](https://help.salesforce.com/s/articleView?language=en_US&type=1&id=000354473){target="_blank"}をクリックしてください。

## API の強化 {#api-enhancements}

* **Bulk Program Member Extract API の新しいフィルタリング機能**：プログラムメンバーシップのステータス、updatedAt、ケイデンス、消費済みコンテンツでフィルタリングして、抽出したデータセットを絞り込みます。

* **Bulk Program Member Extract API の向上**：ジョブの作成中に最大 10 個のプログラムを指定してスループットを向上させます。

## お知らせ {#announcements}

* **Forms の廃止 - Forms 1.0、リードキャプチャ／保存エンドポイント、非スクリプトバージョンのフォーム**：Forms 1.0 アセットのサポートは、2022年10月までに Marketo Engage から完全に削除されます。既存の Forms 1.0 アセットはすべて機能を停止します。Marketo Engage フォームは、ランディングページや web サイトの読み込みに JavaScript が必要です。

**_製品リリースウェビナー_**

[2022年6月および8月の Marketo Engage リリースウェビナー](https://engage.marketo.com/jp/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
