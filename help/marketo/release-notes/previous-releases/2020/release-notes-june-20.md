---
unique-page-id: 37357276
description: リリースノート - 2020 年 6 月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2020 年 6 月
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 100%

---

# リリースノート：2020 年 6 月 {#release-notes-june}

2020 年 6 月リリースには、次の機能が含まれています。お客様のご契約により、制限やオプションの契約が必要なものがあります。詳細は担当の営業にお問い合わせください。

>[!AVAILABILITY]
>
>星印（![](assets/yellow-star.png)）がついている機能は有償オプションになります。詳細は Marketo Engage 担当営業にお問い合わせください。

**_四半期リリース_**：以下の機能は **2020 年 6 月 5 日**&#x200B;にリリースされます。

## Marketo Engage コア機能 {#core-marketo-engage}

* **[予測オーディエンス](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)**![（星）](assets/yellow-star.png)：Adobe Sensei が提供する新しいスマートリストおよびスマートキャンペーンフィルターを使用すると、メール、イベント、ウェビナーマーケティングプログラム用の AI を利用したオーディエンスセグメントを作成できます。AI を使用して、リードがイベントに登録したり参加したり、登録解除したりする可能性に基づいてオーディエンスをセグメント化できます。過去のプログラムに基づいて類似したオーディエンスを構築し、以前の成功を効率的にレプリケートします。予測目標追跡を使用してコンバージョン目標を達成し、イベントプログラムのオーディエンスセグメントを絞り込む方法に関する提案を得ます。
* **バッチメールの高速化** ![（星）](assets/yellow-star.png)：1 時間に最大 300 万件のバッチメールを送信できる、アドビのメールマーケティング機能の強化。バッチキャンペーンとメールレポート処理を再設計し、メールプログラムとバッチメールキャンペーンのパフォーマンスを向上させました。これにより、送信のリードタイムが短くなり、完了時間が改善します。メール送信は通常どおりに簡単に設定できます。この機能強化は、Delivery Services Launch Pack、メール配信ツール、複数の専用 IP アドレスも含まれる製品アドオンとして使用できます。
* **[Adobe Experience Cloud（AEC）とのオーディエンスの統合](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**：新しい Adobe Experience Cloud（AEC）統合では、Marketo Engage の既知のリードの静的リストを複数の AEC アプリケーションと同期して、既存のプログラムの強化、新しい使用例のロック解除、マルチチャネルキャンペーンの調整をおこなうことができます。この統合には、Adobe Analytics、Adobe Target、Adobe Experience Manager、Adobe Audience Manager、Adobe Advertising Cloud が含まれます。
* **[プログラムメンバーカスタムフィールド](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**：プログラムメンバーに関するカスタムフィールドをキャプチャおよび利用します。Marketo Engage フォームでこれらの新しいフィールドを使用し、プログラムのメンバーリストに表示し、スマートリストフィルターとトリガーで活用し、新しいスマートキャンペーンフローアクションに含めて、より詳細なパーソナライゼーションを実現します。UI および API を使用した読み込みと書き出しもできます。カスタムデータオブジェクトおよびフィールド機能の強化。
* **プログラムメンバーの説明**：REST API を使用してプログラムメンバーカスタムフィールドデータの読み込みと書き出しを行えるように、プログラムメンバーメタデータを取得します。API の機能強化。
* **[Microsoft Dynamics でタスクを作成](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**：Marketo Engage でキャプチャされた顧客行動に基づく新しいフローアクションを使用して、Microsoft Dynamics 内で Sales のタスクを作成します。ネイティブの Microsoft Dynamics CRM 統合の強化。
* **リストアセット API エンドポイントで使用されるフォームを取得**：フォームに依存するアセットのリストを取得します。API の機能強化。
* **API を使用したメールのプリヘッダーの設定**：メールのプリヘッダーフィールドの自動翻訳とローカライゼーションを有効にします。API の機能強化。
* **画像とファイルのキャッシュ**：60 秒のキャッシュから Marketo Engage とファイルアセットを提供することで、画像サーバーの安定性を向上させています。

## アカウントベースドマーケティング {#account-based-marketing}

![（星印）](assets/yellow-star.png)

* **新しい顧客検出が一般に利用可能**

   * 新しい顧客検出は、AI を利用した理想的な顧客プロファイルモデルに基づいて、ABM 戦略の新しいターゲット顧客を検出できる、顧客プロファイル機能強化です。提案される新しいアカウントと、AI ベースの適合および目的データの指標を表示、選択、および読み込みます。

<br> 

**_四半期を通した段階的リリース_**

以下の機能はリリース後約 1～2 か月の間に段階的にリリースされます。

## Bizible {#bizible}

![（星印）](assets/yellow-star.png)

* **Marketo Engage プログラムの統合**：Marketo Engage から直接プログラムデータを抽出し、Bizible の属性ジャーニーに沿ってタッチポイントを作成して、メールやエンゲージメントプログラムに適切なクレジットを付与します。Marketo Engage 統合の強化。
* **Marketo Engage アクティビティの統合（ベータ版）**：Marketo Engage アクティビティデータを Bizible に直接取り込み、カスタマージャーニーとすべてのアトリビューションモデルにわたるタッチポイントを作成します。例としては、リードスコアの変更、注目のアクション、メールのクリック、その他のカスタムアクティビティなどがあります。Marketo Engage 統合の強化。
* **Bizible B2B 顧客属性統合（ベータ版）**：これは、Adobe Analytics との Adobe Experience Cloud 統合で、選択した Bizible データを直接 Adobe Analytics に取り込み、より詳細な分析をおこなうことができます。例としては、企業名別のアカウントベースのサイトトラフィックとコンテンツ分析、アカウント属性別、CRM 商談別、Bizible の属性収益とファネルステージで定義された高価値の個人などがあります。
* **Bizible Discover フィルターと機能強化**：ダッシュボード全体でチャネル、サブチャネル、キャンペーン、セグメントフィルターを使用してデータを分析します。より詳細な属性を使用して、データの可視性を強化します。これは、Discover ボードの機能強化です。
* **Microsoft Dynamics のアクティビティ同期**：Microsoft Dynamics CRM アクティビティをタッチポイントジャーニーに取り込み、リードや連絡先に関連付けられた呼び出し、予定、タスクなどのイベントを追跡することで、セールスインタラクションを関連付けます。Microsoft Dynamics CRM 統合の強化。

## Sales Insight {#sales-insight}

![（星印）](assets/yellow-star.png)

* **[Salesforce CRM 用インサイトダッシュボード](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**：Sales Insight の機能を新しい視覚的な新しいマーケティングイベントやキャンペーンの可視性で再設計し、販売者がニーズや興味に基づいて顧客や見込み客に対してより関連性の高い提案を提供できるようにしています。また、販売者は、タイムライン内で連絡先とアカウントアクティビティの両方を表示でき、追加のアクティビティの詳細に簡単にアクセスできます。パッケージのアップグレード方法の詳細については[こちら](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md)をご覧ください。

<br> 

## お知らせ {#announcements}

* **ITP 2.1 以降 RTP の更新**：Safari の cookie ポリシーが変更されたので、RTP cookie が同じドメインで複数のセッションをまたいでユーザーを追跡する機能は、ITP によって、訪問者が使用しているブラウザーとブラウザーのバージョンに基づいて 1 日または 7 日に制限されます。これを考慮して、HTTP 応答を介して Set-Cookie ヘッダーで RTP の cookie を設定できるようにする新しい Web サービスを実装しています。詳しくは[こちら](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603)をご覧ください。

* **バッチキャンペーンインフラストラクチャの変更**：バッチキャンペーンサービスは、今年中にアップグレードします。これはシームレスな更新で、進行中のバッチキャンペーンに影響を与えず、動作の変更にもつながりません。アクションは必要ありません。こちらの [Nation post](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374) で詳細をご覧ください。

## 廃止予定機能 {#deprecations}

* **[Munchkin 関連リード](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**：Munchkin JS のバージョン 159 以降では、Associate Lead メソッドが呼び出されると、廃止の警告がブラウザコンソールに記録され、将来のリリースでこの機能が削除されることを示します。完全な廃止スケジュールは、後日発表されます。

**_製品リリースウェビナー[_**](https://engage.marketo.com/June-Release-2020-On-Demand.html)：2019 年 6 月リリースイノベーションのウェビナーの録画をこちらでご覧ください。
