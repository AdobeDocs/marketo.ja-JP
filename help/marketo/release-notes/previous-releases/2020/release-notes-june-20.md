---
unique-page-id: 37357276
description: リリースノート — 20年6月21日 — Marketoドキュメント — 製品ドキュメント
title: リリースノート — 20年6月
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 5%

---

# リリースノート：20年6月 {#release-notes-june}

20年6月リリースには、次の機能が含まれています。 お客様のご契約により、制限やオプションの契約が必要なものがあります。詳細は担当の営業にお問い合わせください。

>[!AVAILABILITY]
>
>星印（![](assets/yellow-star.png)）がついている機能は有償オプションになります。詳細は Marketo Engage 担当営業にお問い合わせください。

**_四半期_** リリース次の機能は2020年6 **月5日にリリースされます**。

## Marketo Engage コア機能 {#core-marketo-engage}

* **[Predictive Audiences](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)** ![（星）](assets/yellow-star.png):Adobe Senseiを利用した新しいスマートリストフィルターとスマートキャンペーンフィルターを使用すると、Eメール、イベントおよびウェビナーマーケティングプログラム用に、AIを利用したオーディエンスセグメントを作成できます。AIを使用して、イベントに登録、イベントへの参加、購読解除の見込み客数に基づいてオーディエンスをセグメント化します。 過去のプログラムに基づいて類似したオーディエンスを構築し、以前の成功を効率的にレプリケートします。 予測目標追跡を使用してコンバージョン目標を達成し、イベントプログラムのオーディエンスセグメントを絞り込む方法に関するレコメンデーションを得ます。
* **バッチ電子メールブースト** ![（星）](assets/yellow-star.png):1時間に最大300万件のバッチ電子メールを送信できる電子メールマーケティング機能の強化。EメールプログラムとEメールキャンペーンの一括処理を強化するために、バッチキャンペーンとEメールレポート処理のアーキテクチャを変更しました。 これにより、送信のリードタイムが短くなり、完了時間が短縮されます。 通常どおりにEメールを設定し、複雑さは増しません。 この強化は、Delivery Services Launch Pack、電子メール配信ツール、複数の専用IPアドレスも含まれる製品アドオンとして使用できます。
* **[Adobe Experience Cloud(AEC)とのオーディエンスの統合](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**:新しいAdobe Experience Cloud(AEC)統合により、Marketo Engageの既知のリードの静的なリストを複数のAECアプリケーションと同期して、既存のプログラムの強化、新しい使用例のロック解除、マルチチャネルキャンペーンのオーケストレーションをおこなうことができます。この統合には、Adobe Analytics、Adobe Target、Adobe Experience Manager、Adobe Audience Manager、Adobe Advertising Cloudが含まれます。
* **[プログラムメンバーのカスタムフィールド](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**:プログラムメンバーに関するカスタムフィールドを取得し、利用します。Marketo Engageフォームでこれらの新しいフィールドを使用し、プログラムのメンバーリストに表示し、スマートリストフィルターとトリガーで活用し、新しいスマートキャンペーンフローアクションに含めて、自動化を強化し、より詳細なパーソナライゼーションを実現します。 これらは、UIおよびAPIを使用して読み込みおよび書き出しすることもできます。 カスタムデータオブジェクトおよびフィールド機能の強化。
* **プログラム・メンバーの説明**:REST APIを使用してプログラムメンバーカスタムフィールドデータを読み込みおよび書き出す機能を提供し、プログラムメンバーメタデータを取得します。APIの機能強化。
* **[Microsoft Dynamicsでのタスクの作成](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**:Microsoft Dynamics内でSales用のタスクを作成し、Marketo Engageでキャプチャされた顧客行動に基づいて、新しいフローアクションを使用します。ネイティブのMicrosoft Dynamics CRM統合の強化。
* **リストアセットAPIエンドポイントで使用するフォームの取得**:フォームに依存するアセットのリストを取得します。APIの機能強化。
* **APIを使用した電子メールのプリヘッダーの設定**:Eメールのプリヘッダーフィールドの自動翻訳とローカライゼーションを有効にします。APIの機能強化。
* **画像とファイルのキャッシュ**:60秒のキャッシュからMarketo Engageとファイルのアセットを提供することで、画像サーバの安定性を向上させています。

## アカウントベースドマーケティング {#account-based-marketing}

![（星）](assets/yellow-star.png)

* **新しいアカウントの検出は一般に利用可能**

   * 新しいアカウント検出は、AIを利用した理想的な顧客プロファイルモデルに基づいて、ABM戦略の新しいターゲットアカウントを検出できるアカウントプロファイル機能の強化です。 推奨される新しいアカウントと、AIベースの適合および目的データの指標を表示、選択、およびインポートします。

<br> 

**_四半期を通した段階的リリース_**

以下の機能はリリース後約 1 ～ 2 か月の間に段階的にリリースされます。

## Bizible {#bizible}

![（星印）](assets/yellow-star.png)

* **Marketo Engageプログラムの統合**:プログラムデータをMarketo Engageから直接取り込み、Bizibleのアトリビューションジャーニーに沿ったタッチポイントを作成して、Eメールやエンゲージメントプログラムに適切なクレジットを与えます。アドビのMarketo Engage統合の強化。
* **Marketo Engageアクティビティの統合（ベータ版）**:Marketo EngageアクティビティデータをBizibleに直接取り込み、カスタマージャーニーとすべてのアトリビューションモデルをまたいだタッチポイントを作成します。例としては、リードスコアの変更、興味深い瞬間、Eメールのクリック、その他のカスタムアクティビティなどがあります。 アドビのMarketo Engage統合の強化。
* **Bizible B2B顧客属性の統合（ベータ版）**:Adobe AnalyticsとのAdobe Experience Cloud統合で、選択したBizibleデータをAdobe Analyticsに直接取り込み、より詳細な分析をおこなうことができます。例としては、会社名別のアカウントベースのサイトトラフィックおよびコンテンツ分析、アカウント属性別、CRMオポチュニティ別、Bizibleの属性による売上高およびファネルステージで定義された高価値の個人などがあります。
* **Bizbile Discoverのフィルターと機能強化**:ダッシュボード全体でチャネル、サブチャネル、キャンペーン、セグメントフィルターを使用してデータを分析します。より詳細な属性により、データの可視性を強化。 これは、Discoverボードの機能強化です。
* **Microsoft Dynamicsのアクティビティ同期**:Microsoft Dynamics CRMアクティビティをタッチポイントのジャーニーに取り込み、リードや連絡先に関連付けられた呼び出し、予定、タスクなどのイベントを追跡することで、販売のインタラクションを分析します。Microsoft Dynamics CRM統合の強化。

## Sales Insight {#sales-insight}

![（星印）](assets/yellow-star.png)

* **[Salesforce CRM用のインサイトダッシュボード](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**:販売者がニーズや関心に基づいて顧客や見込み客に対してより関連性の高いレコメンデーションを提供できるように、今後のマーケティングイベントやキャンペーンを新たに可視化して、販売インサイト機能を再設計しています。販売者は、タイムライン内で連絡先とアカウントのアクティビティの両方を表示し、追加のアクティビティの詳細に簡単にアクセスすることもできます。 パッケージ[のアップグレード方法の詳細は、こちら](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md)をご覧ください。

<br> 

## お知らせ {#announcements}

* **ITP 2.1以降のRTPの更新**:SafariのCookieポリシーが変更されたので、RTP Cookieで同じドメイン上のセッションをまたいでユーザーを追跡する機能は、訪問者が使用しているブラウザーとブラウザーのバージョンに基づいて、ITPで1日または7日に制限されます。これを考慮して、HTTP応答を介してSet-CookieヘッダーでRTP Cookieを設定できるようにする新しいWebサービスを実装します。 詳細は[こちら](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603)を参照してください。

* **Campaignインフラストラクチャの一括変更**:アドビでは、今年中にバッチキャンペーンサービスをアップグレードしています。これはシームレスな更新で、進行中のバッチキャンペーンには影響せず、動作の変更にはつながりません。 アクションは不要です。 詳しくは、この[Nation post](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374)を参照してください。

## 廃止予定機能 {#deprecations}

* **[マンチキンのアソシエイトリード](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**:バージョン159のMunchkin JSリリースから、 Associate Leadメソッドを呼び出すと、廃止の警告がブラウザーコンソールに記録され、将来のリリースでこの機能が削除されることを示します。 完全な廃止スケジュールは、後日発表されます。

**_製品リリー_** [スウェビナーWebセミナ](https://engage.marketo.com/June-Release-2020-On-Demand.html) ー「20年6月の製品リリースイノベーション」ウェビナーの録画を視聴します。
