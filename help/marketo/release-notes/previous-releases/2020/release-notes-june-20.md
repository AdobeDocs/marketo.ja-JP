---
unique-page-id: 37357276
description: リリースノート - 2020 年 6 月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2020 年 6 月
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
feature: Release Information
TQID: https://experienceleague.adobe.com/HqmRqpmJ9HipbkC2SWTM7RaxYgp04IAbz9cOiDsuGiY
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a8c137b3-8aa5-433e-bdc9-0a216c2a11c1
  - id: ffdd6159-0e10-4a57-8021-94e93bab8183
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: beb7a3c1-66ab-4786-b879-7621375b3c40
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 1099
ht-degree: 89%

---

# リリースノート：2020 年 6 月 {#release-notes-june}

2020 年 6 月リリースには、次の機能が含まれています。 お客様のご契約により、制限やオプションの契約が必要なものがあります。詳細は担当の営業にお問い合わせください。

>[!AVAILABILITY]
>
>星印（![](assets/yellow-star.png)）がついている機能は有償オプションになります。 詳細は Marketo Engage 担当営業にお問い合わせください。

**_四半期リリース_**：以下の機能は **2020 年 6 月 5 日**&#x200B;にリリースされます。

## Marketo Engage のコア機能 {#core-marketo-engage}

* **[予測オーディエンス &#x200B;](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=ja#predictive-audiences)** ![&#x200B; （星） &#x200B;](assets/yellow-star.png):Adobe AIを搭載した新しいスマートリストとスマートキャンペーンフィルターを使用すると、メール、イベント、ウェビナーマーケティングプログラム用にAIを活用したオーディエンスセグメントを作成できます。 AI を使用して、リードがイベントに登録したり参加したり、登録解除したりする可能性に基づいてオーディエンスをセグメント化できます。 過去のプログラムに基づいて類似したオーディエンスを構築し、以前の成功を効率的にレプリケートします。 予測目標追跡を使用してコンバージョン目標を達成し、イベントプログラムのオーディエンスセグメントを絞り込む方法に関するレコメンデーションを得ます。
* **バッチメールの高速化** ![（星）](assets/yellow-star.png)：1 時間に最大 300 万件のバッチメールを送信できる、アドビのメールマーケティング機能の強化。 バッチキャンペーンとメールレポート処理を再設計し、メールプログラムとバッチメールキャンペーンのパフォーマンスを向上させました。 これにより、送信のリードタイムが短くなり、完了時間が改善します。 メール送信は通常どおりに簡単に設定できます。 この機能強化は、Delivery Services Launch Pack、メール配信ツール、複数の専用 IP アドレスも含まれる製品アドオンとして使用できます。
* **[Adobe Experience Cloud（AEC）とのオーディエンスの統合](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**：新しい Adobe Experience Cloud（AEC）統合では、Marketo Engage の既知のリードの静的リストを複数の AEC アプリケーションと同期して、既存のプログラムの強化、新しい使用例のロック解除、マルチチャネルキャンペーンの調整をおこなうことができます。 この統合には、Adobe Analytics、Adobe Target、Adobe Experience Manager、Adobe Audience Manager、Adobe Advertising Cloud が含まれます。
* **[プログラムメンバーカスタムフィールド](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**：プログラムメンバーに関するカスタムフィールドをキャプチャおよび利用します。 Marketo Engageフォームでこれらの新しいフィールドを使用し、プログラムのメンバーリストで表示し、スマートリストのフィルターとトリガーで活用し、新しいスマートキャンペーンのフローアクションに含めることで、オートメーションを強化し、より詳細なパーソナライズを実現します。 UI および API を使用した読み込みと書き出しもできます。 カスタムデータオブジェクトおよびフィールド機能の強化。
* **プログラムメンバーの説明**：REST API を使用してプログラムメンバーカスタムフィールドデータの読み込みと書き出しを行えるように、プログラムメンバーメタデータを取得します。 API の機能強化。
* **[&#x200B; [!DNL Microsoft Dynamics]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)** でタスクを作成：Marketo Engage でキャプチャされた顧客行動に基づく新しいフローアクションを使用して、[!DNL Microsoft Dynamics] 内で Sales のタスクを作成します。 ネイティブの [!DNL Microsoft Dynamics] CRM 統合の強化。
* **リストアセット API エンドポイントで使用されるフォームを取得**：フォームに依存するアセットのリストを取得します。 API の機能強化。
* **API を使用したメールのプリヘッダーの設定**：メールのプリヘッダーフィールドの自動翻訳とローカライゼーションを有効にします。 API の機能強化。
* **画像とファイルのキャッシュ**：60 秒のキャッシュから Marketo Engage とファイルアセットを提供することで、画像サーバーの安定性を向上させています。

## アカウントベースドマーケティング {#account-based-marketing}

![（星印）](assets/yellow-star.png)

* **新しい顧客検出が一般に利用可能**

   * 新しい顧客検出は、AI を利用した理想的な顧客プロファイルモデルに基づいて、ABM 戦略の新しいターゲット顧客を検出できる、顧客プロファイル機能強化です。 提案される新しいアカウントと、AI ベースの適合および目的データの指標を表示、選択、および読み込みます。

<br> 

**_四半期を通した段階的リリース_**

以下の機能はリリース後約 1～2 か月の間に段階的にリリースされます。

## [!DNL Bizible] {#bizible}

![（星印）](assets/yellow-star.png)

* **Marketo Engage プログラムの統合**：Marketo Engage から直接プログラムデータを抽出し、[!DNL Bizible] の属性ジャーニーに沿ってタッチポイントを作成して、メールやエンゲージメントプログラムに適切なクレジットを付与します。 Marketo Engage 統合の強化。
* **Marketo Engage アクティビティの統合（Beta）**：Marketo Engage アクティビティデータを [!DNL Bizible] に直接取り込み、カスタマージャーニーとすべてのアトリビューションモデルをまたいだタッチポイントを作成します。 例としては、リードスコアの変更、注目のアクション、メールのクリック、その他のカスタムアクティビティなどがあります。 Marketo Engage 統合の強化。
* **[!DNL Bizible]B2B 顧客属性統合（Beta）**：Adobe Analytics との Adobe Experience Cloud 統合で、選択した Bizible データを直接 Adobe Analytics に取り込み、より詳細な分析を行うことができます。 例としては、企業名別のアカウントベースのサイトトラフィックとコンテンツ分析、アカウント属性別、CRM 商談別、[!DNL Bizible] の属性収益とファネルステージで定義された高価値の個人などがあります。
* **[!DNL Bizible]Discover フィルターと機能強化**：ダッシュボード全体でチャネル、サブチャネル、キャンペーン、セグメントフィルターを使用してデータを分析します。 より詳細な属性を使用して、データの可視性を強化します。 これは、Discover ボードの機能強化です。
* **[!DNL Microsoft Dynamics]** のアクティビティ同期：[!DNL Microsoft Dynamics] CRM アクティビティをタッチポイントジャーニーに取り込み、リードや連絡先に関連付けられた呼び出し、予定、タスクなどのイベントを追跡することで、セールスインタラクションを関連付けます。 [!DNL Microsoft Dynamics] CRM 統合の強化。

## [!DNL Sales Insight] {#sales-insight}

![（星印）](assets/yellow-star.png)

* **[Salesforce CRM 用インサイトダッシュボード](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**：[!DNL Sales Insight] の機能を新しい視覚的な新しいマーケティングイベントやキャンペーンの可視性で再設計し、販売者がニーズや興味に基づいて顧客や見込み客に対してより関連性の高いレコメンデーションを提供できるようにしています。 また、販売者は、タイムライン内で連絡先とアカウントアクティビティの両方を表示でき、追加のアクティビティの詳細に簡単にアクセスできます。 パッケージのアップグレード方法の詳細については[こちら](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md)をご覧ください。

<br> 

## お知らせ {#announcements}

* **ITP 2.1 以降 RTP のアップデート**：[!DNL Safari] の cookie ポリシーが変更されたので、RTP cookie が同じドメインで複数のセッションをまたいでユーザを追跡する機能は、ITP によって、訪問者が使用しているブラウザーとブラウザーのバージョンに基づいて 1 日または 7 日に制限されます。 これを考慮して、HTTP 応答を介して Set-Cookie ヘッダーで RTP の cookie を設定できるようにする新しい Web サービスを実装しています。 詳しくは[こちら](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603)をご覧ください。

* **バッチキャンペーンインフラストラクチャの変更**：バッチキャンペーンサービスは、今年中にアップグレードします。 これはシームレスな更新で、進行中のバッチキャンペーンに影響を与えず、動作の変更にもつながりません。 アクションは必要ありません。 こちらの [Nation post](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374) で詳細をご覧ください。

## 廃止予定機能 {#deprecations}

* **[Munchkin アソシエイト リード &#x200B;](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: バージョン 159 リリースの[!DNL Munchkin] JSから始まり、アソシエイト リード メソッドが呼び出されると、ブラウザーのコンソールに非推奨警告が記録されます。この機能は将来のリリースで削除されます。完全な非推奨化スケジュールは後日お知らせします。

**_製品リリースウェビナー_**：2019年6月リリースイノベーションのウェビナーの[録画をこちらでご覧ください](https://engage.marketo.com/June-Release-2020-On-Demand.html)。
