---
title: '2020'
description: 2020 - Marketo Docs – 製品ドキュメント
feature: Release Information
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
    internal-label: Design Studio
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
    internal-label: Reporting
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
    internal-label: Personalization
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
    internal-label: Resources
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
subfeature_v2:
  - id: a8c137b3-8aa5-433e-bdc9-0a216c2a11c1
    internal-label: Custom activities
  - id: d1956f52-ecfd-4e01-8941-47af238acb0d
    internal-label: Help center
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
    internal-label: Microsoft Dynamics
  - id: ea4e3ff5-e7b9-4b4c-a5a0-dc27cc3f4275
    internal-label: Custom objects
  - id: f5e85a9b-a883-40d0-8759-f3651efb32e9
    internal-label: Field management
  - id: f7d2c504-7d5f-4a94-b77e-7fce7ef46c22
    internal-label: Audit trail
  - id: fd4ca7b1-bd80-47f4-ad1a-846912e45cc5
    internal-label: Target Account Management
  - id: ffdd6159-0e10-4a57-8021-94e93bab8183
    internal-label: Event programs
  - id: af97ce94-35fa-4fa9-b85a-46b752ac4028
    internal-label: Release information
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: beb7a3c1-66ab-4786-b879-7621375b3c40
    internal-label: Email marketing
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
    internal-label: Governance
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
    internal-label: Optimization
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '4154'
ht-degree: 94%
---
# 2020

## 2020年1月 {#january}

2020 年 1 月リリースには以下の新機能が含まれています。 機能の利用可否については、お使いの Marketo エディションを確認してください。

>[!AVAILABILITY]
>
>星印（![（星印）](assets/yellow-star.png)）がついている機能は有償オプションになります。 詳細は Marketo Engage 担当営業にお問い合わせください。

**_四半期リリース_**

以下の機能は **2020 年 1 月 17 日**（PT）にリリースされます。

## コア Marketo Engage Adobe アプリケーション {#core-marketo-engage-adobe-application}

* [Adobe Experience Manager Asset Selector](/help/marketo/product-docs/adobe-experience-cloud-integrations/importing-assets-with-adobe-experience-manager.md)：Marketo Engage で直接使用できる AEM アセットでブランドに合ったアセットにすばやくアクセスできます。 メモ：この機能は、Marketo Sky と従来の両方のエクスペリエンスで使用できますが、管理機能は Classic エクスペリエンスで使用できます。 AEM Assets のお客様であり、バージョン 6.5 以降を利用している必要があります。

>[!NOTE]
>
>現在、AEM アセットセレクターは Firefox でのみ完全にサポートされています。 Safariではサポートされておらず、最新バージョンのChrome（v）では動作しない場合があります。 80）、SameSite Cookie設定に応じて。

* **[!DNL Microsoft Dynamics]- リードをリアルタイムで CRM に同期**：Marketo Engage と [!DNL Microsoft Dynamics] の間でのリードと取引先責任者のリアルタイム同期。 「リードを Microsoft に同期」フローアクションを使用して、リードまたは取引先責任者を作成し、[!DNL Microsoft Dynamics] ですぐに確認できます。
* **[!DNL LinkedIn]リードジェネレーションフォームの追加フィールドマッピング**：[!DNL LinkedIn] リードジェネレーションフォームからリードデータをキャプチャして、セールスとマーケティングの両方のタッチポイントに、より関連性の高いエクスペリエンスを作成できます。 非表示のフィールド、同意フィールド、およびテストリードフィールドを Marketo Engage に取り込みます。
* **メールテンプレート依存関係 API**：メールテンプレートに依存するアセットのリストを取得して、変更の可能性の範囲と、テンプレートに対するアドレスの依存関係を把握し、テンプレートの変更と削除を迅速におこなうことができます。
* **マルチインスタンス管理の機能強化**：サブスクリプションのスクロール可能なアルファベット順のドロップダウンメニューを使用して、必要なインスタンスにすばやく移動します。

## アカウントベースドマーケティング

![（星印）](assets/yellow-star.png)

* [新しいアカウントの検出（ベータ版）](https://docs.marketo.com/x/WQA6Ag) ![（星）](assets/yellow-star.png)：アカウントプロファイルを使用して、AI を利用した理想的な顧客プロファイルモデルに基づいて、ABM 戦略の新しいターゲットアカウントを検出します。 ABM ターゲティング用の Marketo Engage リードおよびアカウントデータベース内にまだ存在しない、推奨される新しいアカウントと、AI ベースの適合および目的データ指標を表示、選択、インポートします。 資格のあるアカウントプロファイリングのお客様には、すぐに利用可能です。

<br> 

**_四半期を通した段階的リリース_**

以下の機能は四半期ごとのサイクルには含まれず、今後数か月にわたって順次リリースされます。

## [!DNL Bizible]

![（星印）](assets/yellow-star.png)

* **Marketo Engage リード統合**：セールスとマーケティングに、[!DNL Bizible] と Marketo Engage をまたいだリードの統合ビューを提供します。 このアップデートにより、Marketo Engage を追加のリードデータソースとして使用できるようになったので、リードが CRM と同期してリードジェネレーションに関するレポートを作成するのを待つ必要がなくなりました。
* **Discover の機能強化**：[!DNL Bizible] の Discover ボードの機能をさらに活用しましょう。お客様からのフィードバックに基づいて、タイルや属性からトランザクションレコードをドリルダウン、重要なレコード数と対応するコストパーメトリクスを追加、複数のダッシュボードのダッシュボードフィルターを追加／削除などの機能強化が行われました。 また、ログイン時にデフォルトのダッシュボードに直接移動します。

## [!DNL Marketo Sky] {#marketo-sky}

* [画像編集](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/marketo-image-editor.html?lang=en#design-studio)：Marketo Engage を終了せずに、アドビの編集機能にアクセスできます。 この新しい機能により、[!UICONTROL Design Studio] で直接画像の拡張、切り抜き、画像へのテキストの追加などを簡単に実行できます。

## [!DNL Sales Insight]

* **[!DNL Salesforce Lightning]一括アクション**：[!DNL Salesforce Lightning] を使用して、最大 200 名の取引先責任者／リードをキャンペーンに追加し、Marketo Engage メールを一括で送信する機能でセールス効率を高め、購入者のエンゲージメントを維持します。
* **[!DNL Salesforce1]** のモバイルサポート：[!DNL Salesforce1] アプリで、注目のアクションや web アクティビティ、メールなど、すべての [!DNL Sales Insight] 機能に対するモバイルアクセスを外出先で利用できるようになりました。
* **UI の強化**：インターフェイスを更新して、読みやすさを強化し、[!DNL Marketo Sky] エクスペリエンスと一貫性のあるデザインにしました。

## [!DNL Sales Connect]

* **グリッドコンポーネント**：新しいグリッドカスタマイズ機能で [!DNL Sales Connect] インスタンスを最適化します。 表示する列の選択、列の検索、すべての列の選択／選択解除、各ページに表示するデータの行数の指定をおこないます。
* **[コンテンツのロックダウン](/help/marketo/product-docs/marketo-sales-connect/admin/content-lockdown.md)**：管理者以外のユーザがテンプレートやキャンペーンを作成および編集できるかどうかを制御する、購読全体の設定によるブランドの調整を最大化します。

>[!NOTE]
>
>* **TLS 1.0 および 1.1 の廃止**：アドビのリリース構造との統合に向けて、TLS 1.0 および TLS 1.1 の廃止を 2020 年 1 月 13 日に移動しています。 詳細は[こちら](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq)をご覧ください。
>
>* **ITP 2.1+ [!DNL Munchkin] のアップデート**：[!DNL Safari] の cookie ポリシーが変更されたので、[!DNL Munchkin] が同じドメインで複数のセッションをまたいでユーザを追跡する機能は、ITP によって、訪問者が使用しているブラウザーとブラウザーのバージョンに基づいて 1 日または 7 日に制限されます。 これを考慮して、新しい web サービスを実装し、HTTP 応答を介して Set-Cookie ヘッダーで Munchkin の Cookie を設定できるようにしています。 この新しいサービスの実装方法の詳細については、[こちら](https://nation.marketo.com/docs/DOC-7351)を参照してください。

**_製品リリースウェビナー_** [3月3日午前11:00PT / 2:00PM ETに参加して、製品チームが主催するライブウェビナーを開催し、このリリースに含まれる機能について詳しく説明します。](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html)

## 2020年2月 {#february}

2020 年 2 月リリースには以下の新機能が含まれています。 お客様のご契約により、制限やオプションの契約が必要なものがあります。詳細は担当の営業にお問い合わせください。

>[!AVAILABILITY]
>
>星印（![（星印）](assets/yellow-star.png)）がついている機能は有償オプションになります。 詳細は Marketo Engage 担当営業にお問い合わせください。

**_四半期リリース_**&#x200B;以下の機能は **2020 年 2 月 21 日**（PT）にリリースされます。

## Marketo Engage のコア機能

* **[!DNL Microsoft Dynamics]「Microsoft 上の所有者の変更」フローアクション**：Marketo Engage から直接リード／取引先責任者を変更する機能により、[!DNL Microsoft Dynamics] CRM データの管理を維持します。 これは、Marketo のネイティブ CRM 連携機能を強化したものです。
* **ユーザー管理用 API**：外部の ID 管理や組織管理システムを介して、ユーザーや役割の管理を自動化します。 これは、API 機能を強化したものです。
* **カスタムオブジェクトスキーマ API**：Marketo Engage のインスタンス間でカスタムオブジェクトスキーマを自動的に管理およびプロビジョニングすることで、営業およびマーケティングツール間でデータモデルの一貫性を保つことができます。 この API を使用すると、サンドボックスやセンターオブエクセレンスでカスタムオブジェクトを定義してテストし、必要な数だけインスタンスにプロビジョニングすることができます。 これは、API 呼び出し機能を強化したものです。 この拡張機能へのアクセス方法については、Marketo Engage の担当者にお問い合わせください。
* **ランディングページリダイレクトルール API**：ランディングページのリダイレクトルールの管理を自動化します。 これは、API 呼び出し機能を強化したものです。
* **フォームディスクリプターキャッシュ**：フォームをリソースとしてキャッシュすることで、埋め込みフォームの負荷時間を短縮し、アプリケーション全体の安定性を高めています。 埋め込みフォームへの承認は、web 上に反映されるまでに最大 4 分かかる場合があります。 これはランディングページと Forms の機能を強化したものです。

<br> 

**_四半期を通した段階的リリース_**

以下の機能は四半期ごとのサイクルには含まれず、今後数か月にわたって順次リリースされます。

## [!DNL Bizible]

![（星印）](assets/yellow-star.png)

* **アカウントベースのセグメント化**：アカウントの属性に基づいて、Discover ボード用のセグメントやフィルターを作成する機能により、アカウントレベルでのアトリビューションを分析します。 これらのセグメントを使用して、アカウントベースドマーケティングのパフォーマンスを掘り下げることができます。
* **フィルターの保存**：ユーザー独自のダッシュボードに特化したフィルターを保存して、ダッシュボードを迅速かつ一貫して分析できます。
* **PDF へのエクスポート**：Bizible ダッシュボードを PDF としてエクスポートすることで、貴重なインサイトを組織全体で共有します。

## [!DNL Sales Connect]

* **作成ウィンドウのアップデート**：[!DNL Sales Connect] でテンプレートを選択してメールを送信するプロセスを効率化しました。 Web クライアントと Salesforce の作成ウィンドウを、テンプレートカテゴリの保存、メールのスケジュール、メールの一括送信、表示およびクリックの追跡機能付きのメール送信など、販売者のためのワンストップショップとしてご利用いただけます。
* **コマンドセンターのアップデート**：[!DNL Sales Connect] のコマンドセンターを再構築し、[!DNL Sales Connect] から開始されたすべてのメール、コール、タスクを販売者が把握できるようにしました。 また、メールのエンゲージメントや配信可能性などの情報もすべてコマンドセンターから確認できます。

<br> 

## お知らせ

* **Marketo Engage Success Center**：2020 年 2 月に Marketo Success Center をローンチします。 Success Center は製品内のヘルプセンターで、製品ドキュメントやコミュニティの検索、ハウツーガイドの起動、Marketo University や同業ユーザーのベストプラクティスビデオなどのコンテンツへのアクセスなどを、Marketo Engage インスタンスから直接行うことができます。 **注**：この機能は ANZ 地域でベータ版として開始され、北米では四半期後半に展開される予定です。

## 廃止予定機能

* **Asset API「_method」パラメーター**：2020 年 9 月以降、Asset API エンドポイントは、URI 長制限を回避するための POST ボディ内のクエリパラメーターを渡す方法として「_method」パラメーターを受け付けなくなります。 このパラメーターを必要とするリクエストに対応するため、Asset API の URI 制限が 6 KB から 65 KB に引き上げられ、長いリクエスト URI を送信できるようになります。
* **Internet Explorer サポートの廃止**：2020 年 7 月 31 日（PT）の 7 月リリースから、Marketo Engage のユーザーインターフェイスは Internet Explorer でのサポートが終了します。

**_製品リリースウェビナー_** [3月3日午前11:00PT / 2:00PM ETに参加して、製品チームが主催するライブウェビナーを開催し、このリリースに含まれる機能について詳しく説明します。](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html)

## 2020年6月 {#june}

2020 年 6 月リリースには、次の機能が含まれています。 お客様のご契約により、制限やオプションの契約が必要なものがあります。詳細は担当の営業にお問い合わせください。

>[!AVAILABILITY]
>
>星印（![](assets/yellow-star.png)）がついている機能は有償オプションになります。 詳細は Marketo Engage 担当営業にお問い合わせください。

**_四半期リリース_**：以下の機能は **2020 年 6 月 5 日**&#x200B;にリリースされます。

## Marketo Engage のコア機能

* **[予測オーディエンス ](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)** ![ （星） ](assets/yellow-star.png):Adobe AIを搭載した新しいスマートリストとスマートキャンペーンフィルターを使用すると、メール、イベント、ウェビナーマーケティングプログラム用にAIを活用したオーディエンスセグメントを作成できます。 AI を使用して、リードがイベントに登録したり参加したり、登録解除したりする可能性に基づいてオーディエンスをセグメント化できます。 過去のプログラムに基づいて類似したオーディエンスを作成し、以前の成功を効率的に再現します。 予測目標追跡を使用してコンバージョン目標を達成し、イベントプログラムのオーディエンスセグメントを絞り込む方法に関するレコメンデーションを得ます。
* **バッチメールの高速化** ![（星）](assets/yellow-star.png)：1 時間に最大 300 万件のバッチメールを送信できる、アドビのメールマーケティング機能の強化。 バッチキャンペーンとメールレポート処理を再設計し、メールプログラムとバッチメールキャンペーンのパフォーマンスを向上させました。 これにより、送信のリードタイムが短くなり、完了時間が改善します。 メール送信は通常どおりに設定するだけで、追加の複雑さはありません。 この機能強化は、Delivery Services Launch Pack、メール配信ツール、複数の専用 IP アドレスを含む製品アドオンとして利用できます。
* **[Adobe Experience Cloud（AEC）とのオーディエンスの統合](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**：新しい Adobe Experience Cloud（AEC）統合では、Marketo Engage の既知のリードの静的リストを複数の AEC アプリケーションと同期して、既存のプログラムの強化、新しい使用例のロック解除、マルチチャネルキャンペーンの調整をおこなうことができます。 この統合には、Adobe Analytics、Adobe Target、Adobe Experience Manager、Adobe Audience Manager、Adobe Advertising Cloud が含まれます。
* **[プログラムメンバーカスタムフィールド](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**：プログラムメンバーに関するカスタムフィールドをキャプチャおよび利用します。 Marketo Engageフォームでこれらの新しいフィールドを使用し、プログラムのメンバーリストで表示し、スマートリストのフィルターとトリガーで活用し、新しいスマートキャンペーンのフローアクションに含めることで、オートメーションを強化し、より詳細なパーソナライズを実現します。 UI および API を使用した読み込みと書き出しもできます。 カスタムデータオブジェクトおよびフィールド機能の強化。
* **プログラムメンバーの説明**：REST API を使用してプログラムメンバーカスタムフィールドデータの読み込みと書き出しを行えるように、プログラムメンバーメタデータを取得します。 API の機能強化。
* **[ [!DNL Microsoft Dynamics]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)** でタスクを作成：Marketo Engage でキャプチャされた顧客行動に基づく新しいフローアクションを使用して、[!DNL Microsoft Dynamics] 内で Sales のタスクを作成します。 ネイティブの [!DNL Microsoft Dynamics] CRM 統合の強化。
* **リストアセット API エンドポイントで使用されるフォームを取得**：フォームに依存するアセットのリストを取得します。 API の機能強化。
* **API を使用したメールのプリヘッダーの設定**：メールのプリヘッダーフィールドの自動翻訳とローカライゼーションを有効にします。 API の機能強化。
* **画像とファイルのキャッシュ**：60 秒のキャッシュから Marketo Engage とファイルアセットを提供することで、画像サーバーの安定性を向上させています。

## アカウントベースドマーケティング

![（星印）](assets/yellow-star.png)

* **新しい顧客検出が一般に利用可能**

  * 新しいアカウント検出は、AI を活用した理想的な顧客プロファイルモデルに基づいて、ABM 戦略向けのまったく新しいターゲットアカウントを検出できる、アカウントプロファイリング機能の強化です。 提案される新しいアカウントと、それらの AI を活用した適合度およびインテントデータの指標を表示、選択、および読み込みます。

<br> 

**_四半期を通した段階的リリース_**

以下の機能は四半期ごとのサイクルには含まれず、今後数か月にわたって順次リリースされます。

## [!DNL Bizible]

![（星印）](assets/yellow-star.png)

* **Marketo Engage プログラムの統合**：Marketo Engage から直接プログラムデータを抽出し、[!DNL Bizible] の属性ジャーニーに沿ってタッチポイントを作成して、メールやエンゲージメントプログラムに適切なクレジットを付与します。 Marketo Engage 統合の強化。
* **Marketo Engage アクティビティの統合（Beta）**：Marketo Engage アクティビティデータを [!DNL Bizible] に直接取り込み、カスタマージャーニーとすべてのアトリビューションモデルをまたいだタッチポイントを作成します。 例としては、リードスコアの変更、インタレストモーメント、メールのクリック、その他のカスタムアクティビティなどがあります。 Marketo Engage 統合の強化。
* **[!DNL Bizible]B2B 顧客属性統合（Beta）**：Adobe Analytics との Adobe Experience Cloud 統合で、選択した Bizible データを直接 Adobe Analytics に取り込み、より詳細な分析を行うことができます。 例としては、企業名別のアカウントベースのサイトトラフィックとコンテンツ分析、アカウント属性別、CRM 商談別、[!DNL Bizible] の属性収益とファネルステージで定義された高価値の個人などがあります。
* **[!DNL Bizible]Discover フィルターと機能強化**：ダッシュボード全体でチャネル、サブチャネル、キャンペーン、セグメントフィルターを使用してデータを分析します。 より詳細な属性を使用して、データの可視性を強化します。 これは、Discover ボードの機能強化です。
* **[!DNL Microsoft Dynamics]** のアクティビティ同期：[!DNL Microsoft Dynamics] CRM アクティビティをタッチポイントジャーニーに取り込み、リードや連絡先に関連付けられた呼び出し、予定、タスクなどのイベントを追跡することで、セールスインタラクションを関連付けます。 [!DNL Microsoft Dynamics] CRM 統合の強化。

## [!DNL Sales Insight]

![（星印）](assets/yellow-star.png)

* **[Salesforce CRM 用インサイトダッシュボード](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**：[!DNL Sales Insight] の機能を新しい視覚的な新しいマーケティングイベントやキャンペーンの可視性で再設計し、販売者がニーズや興味に基づいて顧客や見込み客に対してより関連性の高いレコメンデーションを提供できるようにしています。 また、販売者は、タイムライン内で連絡先とアカウントアクティビティの両方を表示でき、追加のアクティビティの詳細に簡単にアクセスできます。 パッケージのアップグレード方法の詳細については[こちら](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md)をご覧ください。

<br> 

## お知らせ

* **ITP 2.1 以降 RTP のアップデート**：[!DNL Safari] の cookie ポリシーが変更されたので、RTP cookie が同じドメインで複数のセッションをまたいでユーザを追跡する機能は、ITP によって、訪問者が使用しているブラウザーとブラウザーのバージョンに基づいて 1 日または 7 日に制限されます。 これを考慮して、HTTP 応答を介して Set-Cookie ヘッダーで RTP の cookie を設定できるようにする新しい Web サービスを実装しています。 詳しくは[こちら](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603)をご覧ください。

* **バッチキャンペーンインフラストラクチャの変更**：バッチキャンペーンサービスは、今年中にアップグレードします。 これはシームレスな更新で、進行中のバッチキャンペーンに影響を与えず、動作の変更にもつながりません。 アクションは必要ありません。 こちらの [Nation post](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374) で詳細をご覧ください。

## 廃止予定機能

* **[Munchkin 関連リード](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**：[!DNL Munchkin] JS のバージョン 159 以降では、Associate Lead メソッドが呼び出されると、廃止の警告がブラウザーコンソールに記録され、将来のリリースでこの機能が削除されることを示します。  完全な廃止スケジュールは、後日発表されます。

**_製品リリースウェビナー_**：2019年6月リリースイノベーションのウェビナーの[録画をこちらでご覧ください](https://engage.marketo.com/June-Release-2020-On-Demand.html)。

## 2020年7月 {#july}

2020 年 7 月リリースには以下の新機能が含まれています。 お客様のご契約により、制限やオプションの契約が必要なものがあります。詳細は担当の営業にお問い合わせください。

>[!AVAILABILITY]
>
>ご契約状況によっては、星印（![（星）](assets/yellow-star.png)）がついている機能は有償オプションの追加購入が必要となる場合があります。 詳細は Marketo Engage 担当営業にお問い合わせください。

**_四半期リリース_**&#x200B;以下の機能は **2020 年 7 月 31 日**（PT）にリリースされます。

## 管理

* **[「使用者」書き出し（フィールド管理](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**）：管理者は、選択したフィールドのすべての「使用者」アセットリンクをCSV ファイルに書き出せるようになりました。 この機能強化は、管理者と非管理者の両方が未使用のフィールドをクリーンアップするのに役立ちます。 さらに、アセットを新しいブラウザータブまたはウィンドウで開けるようになりました。

## アカウントベースドマーケティング

![（星印）](assets/yellow-star.png)

* **アカウントプロファイリング UI のアップデート**：アカウントプロファイリングでのターゲットアカウントリストの作成を簡素化し、すべてのステップを 1 つの画面で行うことができます。

<br> 

**_四半期を通した段階的リリース_**

以下の機能は四半期ごとのサイクルには含まれず、今後数か月にわたって順次リリースされます。

* **Forms サービス**：より強力なフォームのフィールド構文検証と、ランディングページ用の新しい Secured Domains の機能で一般的なボットパターンをブロックする機能を導入します。 ボットパターンをブロックすることでスパムフォームの送信を減らし、データベースの品質を向上させることができます。

>[!NOTE]
>
>拡張フォームフィールド構文の検証の完全なロールアウトは、2021 年 1 月のリリース後まで延期されました。

* **Asset API URI サイズ上限の引き上げ**：「_method」パラメーターの削除に先立ち、URI のサイズ制限を 8 KB から 65 KB に引き上げます。 長いクエリ文字列を実行する際に、このサイズ制限を増やすことでデータの受け渡しがより容易になります。 「_method」パラメーターの削除は、今後のセキュリティアップグレードの一環として行われます。

## [!DNL Sales Insight]

![（星印）](assets/yellow-star.png)

*  [!DNL Salesforce]  CRM 統合非ネイティブのお客様に対する **[[!DNL Sales Insight] の有効化](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)（Beta）**：[!DNL Salesforce] CRM 統合非ネイティブの Marketo Engage のお客様も、[!DNL Sales Insight] を使用することで、セールス部門が最もエンゲージメントの高いリードや商談を把握、優先順位付け、的確な対応を行えるようになります。これにより、スマートな販売と取引の迅速化を実現できます。

## [!DNL Sales Connect]

![（星）](assets/yellow-star.png)

* **[販売呼び出しに対する双方の同意の強化：](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)**&#x200B;管理者は、通話録音の設定をより細かく管理できるようになりました。 双方の同意に関する法律に準拠していることを確認し、[通話録音を有効](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md)にします。 通話が録音されていることを知らせる通知を自動化し、通話の前に再生されるオーディオクリップを有効化します。

<br> 

## 告知情報＆廃止予定機能

* **Asset API「_method」パラメーターの削除**：2020 年 9 月以降、Asset API エンドポイントは、URI 長制限を回避するための POST ボディ内のクエリパラメーターを渡す方法として「_method」パラメーターを受け付けなくなります。 このパラメーターを必要とするリクエストに対応するため、Asset API の URI 制限が 8 KB から 65 KB に引き上げられます。
* **[[!DNL Munchkin] Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**：このリリースの Munchkin JavaScript Client のバージョン 159 から、[!DNL Munchkin] Associate Lead メソッドのサポート廃止が開始されます。 メソッドを呼び出すと、今後のリリースでメソッドが削除されることを示す警告が表示されます。 削除すると、メソッドは機能しなくなり、使用しようとしても失敗します。 Marketo Engage のお客様で、最近この方法を利用した場合、利用内容が個別に通知されます。
* **Internet Explorer のサポート**：既にお知らせした通り、Marketo Engage の Internet Explorer 11 のサポートは **2020 年 7 月 31 日**（PT）で終了しました。 引き続き [!DNL Google Chrome]、[!DNL Mozilla Firefox]、[!DNL  Apple Safari]、[!DNL Microsoft Edge] をサポートしていきます。
* **Sky デフォルトエクスペリエンス**：今回のリリースでは、今後行われるメインユーザーエクスペリエンスのアップデートに備えて、管理者やユーザーが [!DNL Marketo Sky] をデフォルトエクスペリエンスとして設定するオプションが削除されます。 今年後半に予定されているメインエクスペリエンスのアップデートの詳細は、7 月以降に公開される予定です。 [!DNL Marketo Sky] をデフォルトのエクスペリエンスとして設定したユーザや、[!DNL Marketo Sky] へのアクセス権を付与されたユーザは、引き続き、マイ Marketo ホームページのタイルから [!DNL Marketo Sky] にアクセスできます。
* **EdgeHTML（Chromium 以外）[!DNL Microsoft Edge] のサポート**：Marketo Engage は、2020 年末に Microsoft Edge の EdgeHTML バージョンのサポートを終了します。 2021年1月1日（PT）からは、Microsoft Edge の Chromium 最新版のみをサポートします。

## 2020年10月 {#october}

2020 年 10 月リリースには以下の新機能が含まれています。 お客様のご契約により、制限やオプションの契約が必要なものがあります。詳細は担当の営業にお問い合わせください。

>[!AVAILABILITY]
>
>星印（![](assets/yellow-star.png)）がついている機能は有償オプションになります。 詳細は Marketo Engage 担当営業にお問い合わせください。

**_四半期リリース_**&#x200B;以下の機能は **2020 年 10 月 16 日（PT）**&#x200B;にリリースされます。

## ターゲットアカウント管理 {#target-account-management}

![（星印）](assets/yellow-star.png)

* **アカウントスマートリスト（ベータ版）**：新しいアカウントスマートリスト機能で ABM 戦略を強化できます。 必要なアカウント属性および人物属性を持つアカウントを動的に識別してクロスチャネルキャンペーンを実行し、タイムリーなアラートをセールス部門に送信することで、案件をより迅速にクローズできます。 注：この機能は、[次世代ユーザーエクスペリエンス](https://nation.marketo.com/t5/Employee-Blogs/The-Next-Generation-Marketo-Engage-Experience/ba-p/304205)が有効になっている環境のお客様で、ターゲットアカウント管理オプションをご契約のお客様にのみご利用いただけます。

## メールマーケティング {#email-marketing}

* **バッチメール高速化**![（星印）](assets/yellow-star.png)：バッチメール配信において、1 時間あたり最大 500 万通までスループットを向上させ、より多くのメールを送信できるようになります。 この拡張されたメール配信オプションをご利用いただくと、複数のバッチメール配信キャンペーン間で待機する必要がなくなり、スケジュールした時間通りにメールを配信することが可能になります。

## ウェブサイトマーケティング {#website-marketing}

* **フォームの埋め込みコードの自動化**：Marketo の外部でホストされている安全なランディングページに埋め込まれた Marketo Engage フォームで、より多くのリードを獲得しましょう。 フォームの埋め込みコードは、ランディングページのドメイン名を含むように自動的に更新されるので、web 開発者の手作業が不要になります。 コードリンク内のカスタムドメインは、ウェブサイトのナビゲーション体験とフォームの利用率を向上させます。

## Experience Cloud 連携 {#experience-cloud-integration}

* **Adobe Experience Cloud から Marketo Engage への継続的なオーディエンス同期**：Adobe Analytics、Adobe Audience Manager またはアドビのリアルタイム CDP のファーストパーティインテントデータに基づいて、Marketo Engage でリードをターゲティングできます。 継続的な同期によって Marketo Engage の静的リストを自動的に更新し、エンゲージメントプログラムやメールプログラムにリードを追加し、リードの準備ができたらセールス部門にアラートを送信します。

## CRM 連携 {#crm-integration}

* **[!DNL Salesforce]** CRM との同期：新しい 2 つの [!DNL Salesforce] 同期ダッシュボードとエラーダッシュボードを使用すると、同期エラーと障害の特定が容易になります。 新規レコードの更新、削除、失敗、同期プロセスの完了を監視します。 レポートは、日付、操作タイプ、またはオブジェクトタイプでフィルタリングできます。

* **[!DNL Microsoft Dynamics 365]統合**：リードおよび取引先責任者の [!DNL Microsoft Dynamics 365] キャンペーンへの登録を自動化します。 新しいスマートキャンペーンフローアクションを使用すると、Marketo Engage のリードと取引先責任者を [!DNL MS Dynamics] キャンペーンに簡単に追加したり削除したりすることができます。 マーケティングからセールスへのリードの受け渡しをシームレスに行い、より迅速に取引をクローズできます。

## 有料メディアへのターゲティング {#paid-media-targeting}

* **[!DNL Facebook]リード広告との連携**：[!DNL Facebook] リード広告用の LaunchPoint サービスを通じて、[!DNL Facebook] フォームのトラッキングパラメーターを取得できるようになりました。 これらの非表示フィールドを Marketo のフィールドにマッピングできるようになり、マーケターは貴重なキャンペーントラッキングデータを保存し、それに基づいて行動できるようになりました。

## 管理

* **役割と権限のエクスポート**：役割と権限をスプレッドシートにエクスポートして、組織内のチーム間で簡単に共有できます。 ロールと権限の監査を簡単かつ迅速に実行できます。

* **監査記録の強化**：新しい監査記録の項目により、マーケティングチームによるメールやランディングページへの変更をより詳細に可視化できます。 メール本文の各モジュールへの変更を記録し、リッチテキスト要素の編集、ステータスの変更、フォームや画像の追加や削除を追跡します。

* **フィールド管理**：全フィールドをエクスポートすることなく、フィールドレコード上の新しいメタデータ入力機能を使用して API フィールド名を簡単に検索できます。 組織に合った方法で LaunchPoint のアプリケーションとの統合を作成したり、データベースに接続したり、オープン API を使用したりすることができます。

* **新しいメタデータエクスポートオプション**：選択したカスタムオブジェクトのメタデータをスプレッドシートにエクスポートして簡単に共有できます。 さらに、リード、企業、標準およびカスタムアクティビティ、タグ、チャネルなどのサブスクリプションオブジェクトのメタデータを、任意にまたはすべてエクスポートできます。 データは管理者が抽出し、分析や設計の目的でエンジニアリングチームと迅速に共有できます。

* **商談カスタムフィールド**：Marketo Engage 内で商談カスタムフィールドを表示できるようになり、商談レコードに関するより深いインサイトを得ることができます。 [!DNL Salesforce] CRM、[!DNL Microsoft Dynamics 365] CRM、Sales ネイティブ連携、または他の API 連携から商談カスタムフィールドのデータを表示します。 商談の詳細とパイプラインを完全に可視化することで、セールス部門と連携してエンゲージメントを調整し、コンバージョン率を高め、案件をより迅速に成約させることができます。

## 四半期を通した段階的リリース {#releasing-throughout-the-quarter}

以下の機能はリリース後約 1 ～ 2 か月の間に段階的にリリースされます。

## [!DNL Sales Insight]

![（星印）](assets/yellow-star.png)

* **API の最適化と新しいガバナンス設定オプション**：API 最適化の強化とガバナンス機能の追加により、[!DNL Sales Insight] のユーザーエクスペリエンスを向上させます。 設定を使用すると、管理者はキャンペーンやイベントをセールスインサイトダッシュボードにどのようにロードするかを定義できます。 柔軟なカレンダーアクティビティ表示オプションにより、API の使用量が削減され、全体的なエクスペリエンスが向上します。

## 告知情報＆廃止予定機能

* **Marketo Engage の新しい外観**：折れ線グラフ、棒グラフ、列グラフ、円グラフを新しく刷新し、マーケティングアクティビティとすべてのレポート機能、およびマーケティングアクティビティに表示されるデータを含む Marketo Engage 全体でアップデートされた可視化の方法を提供します。 今回のアップデートは、Adobe Flash が 2020年12月31日（PT）にサポート終了を迎えることを受けての対応です。

* **ユーザーの役割と権限の更新**：今後のリリースでは、役割と権限の管理を簡素化するために、詳細なリストインポート権限は非推奨となります。 マーケティングアクティビティとリードデータベースの既存のリストインポート権限は、それぞれのアプリ領域で必要なリストインポートオプションを有効にします。

* **フィールド管理**：インフラのセキュリティを高めるために、Marketo Engage のカスタムフィールドタイプへの同期変更の制限が導入されました。 複数のフィールドタイプに変更を加える際には、最初のフィールドの変更を完了させてから次のフィールドに移動する必要があります。 この新しいプロセスにより、より安定した環境を確保し、変更タイプの運用失敗リスクを最小限に抑えることができます。

* **Asset API URI サイズ上限の引き上げ**：「_method」パラメーターの削除に先立ち、URI のサイズ制限を 8 KB から 65 KB に引き上げます。 これにより、長いクエリ文字列をご利用のお客様は、より簡単にデータを渡すことができるようになります。 「_method」パラメーターの削除は、今後のセキュリティアップグレードの一環として行われます。

## 製品リリースウェビナー {#product-release-webinar}

[ここから](https://engage.marketo.com/Oct_20_Release_OnDemand.html)製品リリースウェビナーの録画を視聴する。

