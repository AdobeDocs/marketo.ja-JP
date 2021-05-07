---
unique-page-id: 37357276
description: リリースノート — 20年6月21日 —Marketoドキュメント — 製品ドキュメント
title: リリースノート — 2010年6月
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
translation-type: tm+mt
source-git-commit: d44f5e6f3fb24a25678e4d15ee4c6361b658556b
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 0%

---

# リリースノート：6月20日{#release-notes-june}

6月21日リリースには次の機能が含まれています。 Marketo版で利用可能な機能を確認してください。

>[!AVAILABILITY]
>
>星印(![](assets/yellow-star.png))で示される機能は有料のアドオンです。 詳しくは、Marketo Engageの担当者にお問い合わせください。

**_四半期別_** リリース次の機能が2020年6月5日にリリースさ **れます**。

## コア Marketo エンゲージ {#core-marketo-engage}

* **[予測オーディエンス](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)** ![（星形）](assets/yellow-star.png):Adobe Senseiが提供する新しいスマートリストおよびスマートキャンペーンフィルターを使用すると、電子メール、イベント、ウェビナーマーケティングプログラム向けに、AIで提供されるオーディエンスセグメントを作成できます。AIを使用すると、リードがイベントに登録したり、イベントに参加したり、登録を取り消したりする可能性に基づいてオーディエンスをセグメント化できます。 過去の成功を効率的に再現するために、過去のプログラムに基づいて類似オーディエンスを構築。 予測目標追跡を使用してコンバージョン目標を達成し、イベントプログラムのためのオーディエンスセグメントを絞り込む方法に関する推奨事項を得ます。
* **Batch Email Boost** ![（星形）](assets/yellow-star.png):1時間に最大300万個のバッチ電子メールを送信できるEメールマーケティング機能の強化。バッチキャンペーンおよび電子メールレポート処理を再設計し、電子メールプログラムとバッチ電子メールキャンペーンのパフォーマンスを向上しました。 これにより、送信するリードタイムが短くなり、完了時間も短縮されます。 通常どおりに電子メールの送信を設定します。複雑さは増しません。 この機能強化は、配信サービス起動パック、電子メール配信ツール、複数の専用IPアドレスなどの製品アドオンとして利用できます。
* **[Adobe Experience Cloudとのオーディエンス統合(AEC)](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**:新しいAdobe Experience Cloud(AEC)統合により、Marketo Engageからの既知のリードの静的なリストを複数のAECアプリケーションと同期して、既存のプログラムを強化し、新しい使用例をロック解除し、複数チャネルのキャンペーンを調整できます。この統合には、Adobe Analytics、Adobe Target、Adobe Experience Manager、Adobe Audience Manager、Adobe Advertising Cloudが含まれます。
* **[プログラムメンバのカスタムフィールド](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**:プログラムメンバに関するカスタムフィールドの取得と利用。これらの新しいフィールドをMarketo Engageフォームで使用し、プログラムのメンバーリストに表示し、スマートリストフィルターとトリガーで活用し、新しいスマートキャンペーンフローアクションに含めて、自動化とより詳細なパーソナライゼーションを強化します。 これらは、UIやAPIを使用して読み込んだり書き出したりすることもできます。 カスタムデータオブジェクトおよびフィールド機能の強化。
* **プログラムメンバーの説明**:プログラムメンバーのメタデータを取得し、REST APIを使用してプログラムメンバーのカスタムフィールドデータの読み込みと書き出しを行うことができます。APIの機能強化。
* **[Microsoft Dynamics](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**&#x200B;でタスクを作成：Marketo Engageでキャプチャされた顧客の行動に基づいて、新しいフローアクションを使用して、Microsoft Dynamics内の販売のタスクを作成します。ネイティブのMicrosoft Dynamics CRM統合の強化。
* **リストアセットAPIエンドポイントで使用されるフォームの取得**:フォームに依存するアセットのリストを取得します。APIの機能強化。
* **APIを介した電子メールプリヘッダーの設定**:電子メールプリヘッダーフィールドの自動翻訳およびローカライゼーションを有効にします。APIの機能強化。
* **イメージとファイルのキャッシュ**:60秒のキャッシュからMarketo Engageとファイルのアセットを提供することで、画像サーバの安定性を向上させています。

## アカウントベースドマーケティング {#account-based-marketing}

![（星形）](assets/yellow-star.png)

* **新しいアカウントの検出は一般的に利用可能**

   * 新規アカウント発見は、AIを利用した理想的な顧客プロファイルモデルに基づいて、ABM戦略の新規ターゲットアカウントを発見できるようにする、アカウントプロファイル機能の強化です。 推奨される新しいアカウントと、AIベースの適合および意図データインジケーターを表示、選択および読み込みます。

<br> 

**_四半期全体でリリース_**

次の機能は、四半期に属さないサイクルで提供され、今後数か月間にわたってリリースされます。

## Bizible {#bizible}

![（星形）](assets/yellow-star.png)

* **Marketo Engageプログラムの統合**:プログラムデータをMarketo Engageから直接取り込み、Bizibleのアトリビューションジャーニーに沿ってタッチポイントを作成して、電子メールやエンゲージメントプログラムのクレジットを適切に配分します。Marketo Engage統合の強化。
* **Marketo Engageアクティビティ統合（ベータ版）**:Marketo EngageアクティビティデータをBizibleに直接取り込んで、顧客ジャーニーとすべてのアトリビューションモデルにわたるタッチポイントを作成します。例としては、リードスコアの変更、興味深い瞬間、電子メールのクリック、任意のカスタムアクティビティなどがあります。 Marketo Engage統合の強化。
* **Bizible B2B顧客属性統合（ベータ版）**:これはAdobe AnalyticsとのAdobe Experience Cloud統合で、Bizibleのデータを選択して直接Adobe Analyticsに持ち込み、より詳細な分析を実現します。例としては、会社名別のアカウントベースのサイトトラフィックやコンテンツ分析、アカウント属性別のCRMオポチュニティ、Bizible属性付きの売上高やファネルステージで定義される高価値の個人などがあります。
* **Bizbile Discoverのフィルターと機能強化**:ダッシュボード間のチャネル、サブチャネル、キャンペーン、セグメントのフィルターでデータを分析します。ドリルダウン属性を増やして、データの視認性を高めます。 これは、Discoverボードの機能強化です。
* **Microsoft Dynamics**&#x200B;用アクティビティ同期：Microsoft Dynamics CRMアクティビティをタッチポイントジャーニーに取り込み、リードや連絡先に関連付けられた呼び出し、予定、タスクなどのイベントを追跡することで、販売インタラクションを関連付けます。Microsoft Dynamics CRM統合の機能強化。

## Sales Insight {#sales-insight}

![（星形）](assets/yellow-star.png)

* **[Salesforce CRMのインサイトダッシュボード](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**:Sales Insightの機能を新たに考え直し、今後のマーケティングイベントやキャンペーンの注目度を新たに取り入れて、販売者のニーズや関心に基づいて、顧客や見込み客に対してより関連性の高いレコメンデーションを提供します。販売者は、タイムライン内の連絡先とアカウントのアクティビティの両方を表示して、追加のアクティビティの詳細に簡単にアクセスすることもできます。 パッケージのアップグレード方法の詳細は、[こちら](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/configuration-for-existing-customers.md)を参照してください。

<br> 

## お知らせ {#announcements}

* **ITP 2.1+ RTPの更新**:SafariのCookieポリシーが変更されたため、同じドメインのセッション間でユーザーを追跡するRTP Cookieの機能は、訪問者が使用するブラウザーとブラウザーのバージョンに基づいて、ITPによって1日または7日に制限されます。この点を考慮して、HTTP応答を介してSet-CookieヘッダにRTP cookieを設定できるようにする新しいWebサービスを導入します。 詳細は、[](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603)を参照してください。

* **バッチキャンペーンインフラストラクチャの変更**:バッチキャンペーンサービスは、今年中にアップグレードします。これはシームレスな更新で、進行中のバッチキャンペーンに影響を与えず、動作の変更には影響しません。 操作は必要ありません。 詳細については、この[国の投稿](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374)を参照してください。

## 廃止{#deprecations}

* **[Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**:Munchkin JSのバージョン159リリース以降、Associate Leadメソッドが呼び出されると、非推奨の警告がブラウザーコンソールに記録され、今後のリリースでこの機能が削除されることを示します。 完全な廃止スケジュールは、後日発表されます。

**_製品リリース_** [のウェビナー：6月20日の製品リリース・イノベーションに関するウェビナーの](https://engage.marketo.com/June-Release-2020-On-Demand.html) 記録を視聴できます。
