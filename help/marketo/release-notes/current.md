---
description: 最新のリリースノート - Marketo ドキュメント - 製品ドキュメント
title: 最新のリリースノート
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: 46aff8058cb97743bee1bd5ff5ddf0ddbbb663a5
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 9%

---

# リリースノート：2022 年 6 月 {#release-notes-june-22}

以下に、22 年 6 月リリースに含まれるすべての機能を示します。 機能の可用性についてはお使いの Marketo Engage のエディションをご確認ください。

>[!AVAILABILITY]
>
>星（![星](assets/yellow-star.png)）で示す機能は有償オプションです。詳細は Marketo Engage 担当営業にお問い合わせください。

以下の機能のリリースは、 **2022 年 6 月 25 日**（特に指定のない限り）後週に残りの機能が段階的に公開される場合 )

## マーケティングデータ環境 {#marketing-data-environment}

* **カスタムオブジェクトの CreatedAt/UpdatedAt フィールドを公開します**:ユーザーの詳細画面でこれらのフィールドを調べて、さらなるインサイトを得ることができます。

## クロスチャネルオーケストレーション {#cross-channel-orchestration}

* **ダイナミックチャットでのストリームデザイナーの使いやすさの向上**:ドラッグ&amp;ドロップを必要とせずに、ストリームデザイナーのキャンバスから直接カードを追加できます。 また、Dynamic Chat インターフェイスが改善され、個々のカードでのコンテンツの可視性が向上しました。

* **ダイナミックチャット用の高度な予定ルーティングルール**:Dynamic Chat は、ターゲットの予定のルーティング用の追加のオプションを提供します。 Marketo Engageの属性に基づいてルーティングするエージェントの予定を指定し、リードを適切なエージェントにルーティングします。

* **ダイナミックチャットの高度なダイアログレポート**:エンゲージメント指標とコンバージョン指標に関する新しいデータ視覚化機能を使用して、Dynamic Chat キャンペーンのパフォーマンスをより詳細に表示します。

* **ダイナミックチャットの未使用Marketo Engage属性の同期解除**:Dynamic Chat サブスクリプションからMarketo Engage属性を同期解除して、未使用になるので、データを簡単に整理し、必要に応じて代替属性を同期できます。

## エクスペリエンスの自動化 {#experience-automation}

* **グローバルフォームフィールド検証ルールの除外**:グローバルフォーム検証ルールから特定のフォームを除外して、サブスクリプションセンターや他のビジネスクリティカルなワークフローがすべての値を受け入れるようにします。

* **セルフサービスのフローステップ**:スマートキャンペーンで使用するカスタマイズされたフローステップを作成できるので、Marketo Engageとスタックの他の部分との接続性を拡張できます。 Marketo Engageのユーザーとパートナーの両方がこの機能を活用して、トリガー、バッチ、実行可能なキャンペーンでの外部 Web サービスの使用を可能にすることができます。Web フックは、トリガーのキャンペーンでのみ使用できます。

* **Munchkin プロトコル非依存リンクトラッキング**:追跡のサポートを拡張 `tel` および `mailto` Munchkin とのリンクを使用して、拡張された一連のウェブ動作を追跡します。

* **Web フック用の追加の HTTP メソッド**:Web サービスとやり取りするリクエストの種類として、PUT、PATCH、DELETEを指定します。

## Sales Insight {#sales-insight}

![（星印）](assets/yellow-star.png)

* **Salesforce の Sales Insight 権限セット**:管理者は、Sales Insight Salesforce パッケージの一部であるMarketoアプリ権限セットを使用して、プロファイルレベルではなく、ユーザーレベルで限られた一連のユーザーに対して Sales Insight のアクセス権を提供できます。

* **マイMarketoタイルの更新 — Sales Insight アクション**:Marketo管理者（および指定したユーザー）は、My Marketoページにある新しい Sales Insight アクションタイルから、Sales Insight アクションインスタンスにすばやく移動できるようになりました。

## Sales Connect {#sales-connect}

![（星印）](assets/yellow-star.png)

* **Salesforce API 更新**:Salesforce Summer 22 リリースでは、API レガシーバージョン 21 ～ 30 は Salesforce でサポートされなくなります。 このMarketo Engageリリースでは、従来の API バージョンを使用するすべてのセールスコネクトリクエストが更新され、サポート対象のバージョン内に留まります。 Salesforce API の定年プランの詳細は、 [ここ](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target=&quot;_blank&quot;}。

## API の強化 {#api-enhancements}

* **一括プログラムメンバー抽出 API の新しいフィルタリング機能**:抽出したデータセットを絞り込むには、プログラムメンバーシップのステータス、updatedAt、cadence または exhusted コンテンツでフィルタリングします。

* **プログラムメンバー一括抽出 API の改善**:スループットを向上させるには、ジョブの作成中に最大 10 個のプログラムを指定します。

## お知らせ {#announcements}

* **Formsの廃止 — Forms 1.0、リードキャプチャ/保存エンドポイント、非スクリプトバージョンのフォーム**:Forms 1.0 アセットのサポートは、2022 年 10 月までにMarketo Engageから完全に削除されます。 既存のForms 1.0 アセットはすべて機能しなくなります。 Marketo Engageフォームを読み込むには、ランディングページや Web サイトで JavaScript を読み込む必要があります。

**_製品リリースウェビナー_**

2022 年 8 月 24 日 (PT) 午前 9 時/午後 12 時 (ET) に [ライブウェビナー](https://engage.marketo.com/2022_June_August_Release_Webinar_RegistrationPage.html)アドビの製品チームがホストする {target=&quot;_blank&quot;}。最新の製品イノベーションの使用方法を学ぶことができます。
