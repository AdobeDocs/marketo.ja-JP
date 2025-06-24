---
description: リリースノート - 2022年6月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2022年6月
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 62%

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

* **[!DNL Dynamic Chat]** ーザーによるストリームDesignerの使いやすさの向上：ドラッグ&amp;ドロップを必要とせずに、ストリームDesignerキャンバスからカードを直接追加します。 また、[!DNL Dynamic Chat] インターフェイスも改善され、個々のカードのコンテンツの可視性が向上しました。

* **[!DNL Dynamic Chat]** の高度な予定ルーティングルール：[!DNL Dynamic Chat] では、ターゲット設定された予定ルーティングに関するより多くのオプションを提供しています。 Marketo Engage の属性に基づいてルーティングするエージェントの予定を指定し、リードを適切なエージェントにルーティングします。

* **[!DNL Dynamic Chat]** の高度なダイアログレポート：エンゲージメントとコンバージョン指標に関するすべての新しいデータビジュアライゼーションを使用して、[!DNL Dynamic Chat] キャンペーンのパフォーマンスをより詳細に表示します。

* **[!DNL Dynamic Chat]** の未使用のMarketo Engage属性の同期を解除：未使用になる [!DNL Dynamic Chat] サブスクリプションからMarketo Engage属性の同期を解除します。これにより、データのクリーン性が向上し、必要に応じて代替属性を同期することができます。

## 次世代のエクスペリエンス

**新しい切替スイッチ表示**：次世代のエクスペリエンスで、以下の表示を利用できるようになりました。

* [ メールの詳細表示 ](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [ メールリスト表示 ](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## エクスペリエンスの自動化 {#experience-automation}

* **グローバルフォームフィールド検証ルールの除外**：グローバルフォーム検証ルールから特定のフォームを除外して、サブスクリプションセンターや他のビジネスクリティカルなワークフローがすべての値を受け入れるようにします。

* **セルフサービスのフローステップ**：スマートキャンペーンで使用するカスタマイズされたフローステップを作成する機能により、Marketo Engage とスタックの他の部分との接続性を拡張できます。Marketo Engage のユーザとパートナーの両方がこの機能を活用して、トリガーキャンペーンでのみ使用できる web フックとは異なり、トリガー、バッチ、実行可能なキャンペーンで外部の web サービスを使用できます。

* **Munchkin プロトコル非依存リンクトラッキング**：Munchkin による `tel` と `mailto` のリンクトラッキングのサポートを拡張して、展開された一連の web 動作をトラックします。

* **Webhook 用の追加の HTTP メソッド**：Web サービスとやり取りするリクエストの種類として、PUT、PATCH、DELETE を指定します。

## [!DNL Sales Insight] {#sales-insight}

![（星印）](assets/yellow-star.png)

* [!DNL Salesforce]&#x200B;**の**&#x200B;[!DNL Sales Insight] 権限セット：管理者は、[!DNL Sales Insight] [!DNL Salesforce] パッケージの一部であるMarketo アプリ権限セットを使用して、プロファイルレベルではなくユーザーレベルで、限られたユーザーセットに [!DNL Sales Insight] しいアクセス権を付与できます。

* **マイMarketo タイルの更新 – [!DNL Sales Insight] アクション**: Marketo管理者（および管理者が指名したユーザー）は、マイMarketo ページの新しい [!DNL Sales Insight] アクションタイルを使用して、[!DNL Sales Insight] Actions インスタンスにすばやく移動できるようになりました。

## [!DNL Sales Connect] {#sales-connect}

![（星印）](assets/yellow-star.png)

* **[!DNL Salesforce]API アップデート**:[!DNL Salesforce] Summer &#39;22 リリースでは、API レガシーバージョン 21 ～ 30 は [!DNL Salesforce] でサポートされなくなります。 このMarketo Engage リリースでは、従来の API バージョンを使用しているすべての [!DNL Sales Connect] リクエストが、サポートされているバージョンの範囲内に収まるように更新されました。 API 廃止プランについて詳 [!DNL Salesforce] くは、[ こちら ](https://help.salesforce.com/s/articleView?language=en_US&type=1&id=000354473){target="_blank"} をクリックしてください。

## API の強化 {#api-enhancements}

* **Bulk Program Member Extract API の新しいフィルタリング機能**：プログラムメンバーシップのステータス、updatedAt、ケイデンス、消費済みコンテンツでフィルタリングして、抽出したデータセットを絞り込みます。

* **Bulk Program Member Extract API の向上**：ジョブの作成中に最大 10 個のプログラムを指定してスループットを向上させます。

## お知らせ {#announcements}

* **Forms の廃止 - Forms 1.0、リードキャプチャ／保存エンドポイント、非スクリプトバージョンのフォーム**：Forms 1.0 アセットのサポートは、2022年10月までに Marketo Engage から完全に削除されます。既存の Forms 1.0 アセットはすべて機能を停止します。Marketo Engage フォームは、ランディングページや web サイトの読み込みに JavaScript が必要です。

**_製品リリースウェビナー_**

[2022 年 6 月および 8 月のMarketo Engage リリースウェビナー ](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
