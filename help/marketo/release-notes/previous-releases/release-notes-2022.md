---
title: 2022
description: 2022 - Marketo Docs – 製品ドキュメント
feature: Release Information
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
  - id: efc9a24a-a6a4-449d-a3e6-44f6c74dfd46
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 992f0ad35d396b1f6ecd30f34ba1d228116fb264
workflow-type: tm+mt
source-wordcount: 4282
ht-degree: 90%

---

# 2022

## 2022年1月 {#january}

2022年1月リリースには、次の機能が含まれています。 機能の可用性についてはお使いの Marketo Engage のエディションをご確認ください。

>[!AVAILABILITY]
>
>星印（![星印](assets/yellow-star.png)）で示す機能は有償オプションです。 詳細は Marketo Engage 担当営業にお問い合わせください。

**_四半期リリース_**

以下の機能のリリースは、**2022年1月21日**&#x200B;に始まり、（特に指定のない限り）次の週から各機能が段階的にロールアウトされます。

## 次世代エクスペリエンス

* **次世代エクスペリエンスのための画面の更新**：次世代のエクスペリエンスで、切替スイッチを介してアクセス可能な、最新のデザインと操作性の強化を備えた新しい画面を追加しました。

   * [!UICONTROL デザインスタジオ]でのランディングページアセットの詳細
   * [!UICONTROL マーケティングアクティビティ]のランディングページアセットの詳細

## [!DNL Microsoft Dynamics] 統合 {#microsoft-dynamics-integration}

* **一般に利用可能な複数選択オプションセットフィールドタイプの同期**：[!DNL Microsoft Dynamics] の複数選択オプションセットフィールドタイプを同期して、スマートリストとスマートキャンペーンで活用し、より詳細なオーディエンスターゲティングを実現します。 トピック／関心のある製品、優先するコミュニケーションモードなどの例があります。 この新しい同期は、[!DNL Microsoft Dynamics] バージョン 9.X（Dynamics 365 Online を含む）で使用できます。

* **[!DNL Microsoft Dynamics 365 Online]** サーバー間認証：セキュリティを強化するため、[!DNL Microsoft Dynamics 365 Online] への非インタラクティブアクセス用に、Azure Active Directory の Marketo Engage 同期ユーザ認証の追加モードとして、サーバー間（S2S）認証をサポートするようになりました。 すべての認証とサインオンが OAuth（クライアント ID とクライアント秘密鍵のみ）に基づくため、多要素認証を使用できます。

>[!NOTE]
>
>S2S モードは、追加のライセンスの使用を保存する Licensed User ではなく、Application User に基づいています。

## 管理 {#administration}

* **[フォーム検証ルール](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**：問題のある、または望ましくないメールドメインが Marketo Engage フォームを送信するのを防ぐ機能を備え、データベースの正常性を維持します。 グローバルフォーム検証ルールパネルを使用すると、管理者はブロックリスト、フォームをブロックする自由消費者ドメインの事前定義済みリストを定義するか、有効にすることができます。

* **[ランディングページヘッダーのセキュリティ](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**：管理者は、ランディングページドメインで Strict Transport Security ヘッダーと X-Frame Options ヘッダーを管理して、強力なセキュリティ要件を実施できます。

**_四半期を通した段階的リリース_**

以下の機能はリリース後約 1～2 か月の間に段階的にリリースされます。

## AEP Marketo Engage 宛先コネクタ - 新規リードを作成 {#aep-marketo-engage-destination-connector}

Adobe Experience Platform（AEP）も使用している Marketo Engage の顧客は、AEP の宛先コネクタを介して新しいリードレコードを AEP から Marketo Engage にプッシュしてデータベースを最大化できます。 オーディエンスセグメントを AEP から Marketo Engage に送信する際、セグメント内のユーザのうち、Marketo Engage データベースにまだ存在しないユーザは[自動的に追加できます](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md)。

## [!DNL Sales Insight] {#sales-insight}

![（星印）](assets/yellow-star.png)

[!DNL Salesforce] CRM 用の **[!DNL Sales Insight]**

* **ベストベット [!UICONTROL の新しいタイプ列]**：販売者は、[!UICONTROL &#x200B; ベストベット &#x200B;] ページで「タイプ」というラベルの付いた新しい列を使用して、リードと取引先責任者を区別するためにより迅速なインサイトを得られます。

* **[!DNL Salesforce]Platform API のアップデート**：[!DNL Salesforce] が [!DNL Salesforce] Platform API バージョン 21.0 ～ 30.0 を廃止したのに対応して、[!DNL Sales Insight] パッケージが最新の API でアップデートされました。

* **アップデートされたブランディング**：すべての [!DNL Sales Insight] ページは、アドビのブランディングに合わせてアップデートされています。

**[!DNL Sales Insight]for[!DNL Microsoft Dynamics]**

* **更新されたアカウントのレイアウト**：販売者は、アカウント内のすべての取引先責任者に関するメールアクティビティ、web アクティビティ、注目のアクティビティ、スコア変更のようなトップアクティビティを総合的に把握できます。

## [!DNL Sales Connect] {#sales-connect}

![（星印）](assets/yellow-star.png)

* **通話結果と理由**：新しく完全にカスタマイズ可能な通話結果と通話理由のオプションを使用して、営業部門のアウトバウンド活動をより詳細に理解および追跡します。 これらの新しいフィールドに加えて、販売者が通話を行う間に、通話理由と結果の選択を強制する新しいガバナンス、および [!DNL Salesforce] にデータを記録するための新しい通話理由と通話結果 [!DNL Salesforce] アクティビティカスタムフィールドが導入されました。 [こちら](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812)をクリックすると、詳細が表示されます。

* **[!DNL Salesforce]アクティビティ詳細のカスタマイズ**：セールスアクティビティが [!DNL Sales Connect] から [!DNL Salesforce] に記録される際に、[!DNL Salesforce] タスク件名フィールドに追加される情報をカスタマイズすることで、[!DNL Salesforce] でより多くのセールスアクティビティとタスクデータを取り込みます。 [こちら](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819)をクリックすると、詳細が表示されます。

## お知らせ {#announcements}

* **Marketo Sky の廃止**：Marketo Sky は 3月に利用できなくなります。これは、当社が次世代ユーザエクスペリエンスの提供にリソースを注力しているためです。 現在 Marketo Sky 専用の機能へのアクセスを維持するため、3 月には、アセットの有効期限とスマートキャンペーンの優先順位の上書きがメインストリームエクスペリエンスに取り入れられます。 [こちら](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33)をクリックすると、詳細が表示されます。

* **フォームエンドポイントの廃止**：leadCapture/save2 エンドポイントに対する、サポートされていないプログラム形式の POST は、Marketo Engage フォームによって拒否されます。 [こちら](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631)をクリックすると、詳細が表示されます。

* **ユーザーを招待ダイアログにログイン**:3月に、既存のオプション機能「ユーザーを招待ダイアログにログイン」が廃止されます。 機能「[!UICONTROL &#x200B; ユーザーを招待ダイアログにログイン &#x200B;]」機能は、今後のAdobe Identity Management System Integrationに必要なユニバーサル ID機能によって上書きされ、すべてのサブスクリプションで2021年8月に有効になりました。 廃止の結果、Marketo Engage の購読では、メールアドレスごとにユーザを 1 名だけ関連付けられるようになります。

**Marketo Engage ドメイン - [!DNL Sales Insight] 設定**：SSL 証明書がプロビジョニングされていない Marketo Engage ドメインおよび https:// の場合、呼び出しは SSL ハンドシェイクエラーで失敗します。 したがって、これらのドメインは廃止される予定です。 その結果、これらのドメインを指す古い設定を持つ [!DNL Sales Insight] ユーザには、リード、取引先責任者、顧客、商談パネル、または Marketo グローバルページでシステムコールアウトエラーが発生する可能性があります。 このエラーが発生した場合、[!DNL Salesforce] で [Marketo Engage 設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)をアップデートすることをお勧めします。 ドキュメントの「[!DNL Marketo Sales Insight] 設定」節でハイライトされている Marketo Engage 資格情報のみを更新する必要があります。

**_製品リリースウェビナー_**

[2022年1月Marketo Engage リリースウェビナー](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)

## 2022年3月 {#march}

2022年3月リリースには、次の機能が含まれています。 利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

>[!AVAILABILITY]
>
>星印（![星印](assets/yellow-star.png)）で示す機能は有償オプションです。 詳細は Marketo Engage 担当営業にお問い合わせください。

**_四半期リリース_**

以下の機能のリリースは、**2022年3月11日**&#x200B;に始まり、（特に指定のない限り）次の週から各機能が段階的にロールアウトされます。

## クロスチャネルオーケストレーション {#cross-channel-orchestration}

* **[!DNL Dynamic Chat]**：積極的で魅力的な、1:1個のパーソナライズされた会話を使用して、リードとアカウントの両方をターゲットにすることで、web サイト上のあらゆる機会を最大化します。 [Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"} を使用すると、Marketo Engage ユーザは、B2B マーケティングおよびセールスのユースケースに対して、統合されたクロスチャネルエクスペリエンスの主要部として、チャットを活用し始めることができます。 チャット内で直接会議を予約する機能、リードルーティング、スターターテンプレート、ドラッグ＆ドロップによる会話の作成などの機能があります。 動的チャットは、すべての Marketo Engage パッケージに含まれ、今年にすべての Marketo Engage ユーザにロールアウトされます。

* **メールボットアクティビティのフィルタリング機能強化**：以前にリリースした[メールボットアクティビティのフィルタリング](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}を機能強化し、ボットとして識別されたアクティビティの記録をオプトインできるようになりました。 ボットが実行したと識別されたアクティビティに基づいて、アクションをフィルタリングしてトリガーを設定できます。

## 次世代エクスペリエンス

* **次世代エクスペリエンスのための画面の更新**：次世代のエクスペリエンスで、切替スイッチを介してアクセス可能な、最新のデザインと操作性の強化を備えた新しい画面を追加しました。

   * [!UICONTROL デザインスタジオ]でのフォームリスト表示（新しい一括アクションを含む）

* **プログラムワークフローインポートのアップデート**：プログラムワークフローのインポートは、デザインと操作性をアップデートして機能強化した、次世代のエクスペリエンスで提供されます。 切替スイッチはなく、自動的に変更されます。

* **次世代エクスペリエンス切替スイッチの管理者制御**：切替スイッチにアクセスできるユーザのタイプを管理者が選択できるように、次世代エクスペリエンスのロールアウトを管理します。

## エクスペリエンスの自動化 {#experience-automation}

* **セルフサービスのフローステップ（ベータ版）**：スマートキャンペーンで使用するカスタマイズされたフローステップを作成する機能により、Marketo Engage とスタックの他の部分との接続性を拡張できます。 Marketo のユーザとパートナーの両方がこの機能を活用して、（トリガーキャンペーンでのみ使用できる web フックとは異なり）バッチ、実行可能なキャンペーンで外部の web サービスを使用できます。

* **アセットの有効期限**：Classic ユーザエクスペリエンスで、指定した日時に自動的に非アクティブ化するようにスケジュールを設定し、時間的制約のあるアセットとキャンペーンの制御を維持します。

* **スマートキャンペーン優先度の上書き**：標準キャンペーン優先順位のトリガーを上書きする機能により、優先度の高いランキングスマートキャンペーンをすぐに実行できます。 また、優先度の高い他のタスクの処理リソースを解放するために、優先度の低いトリガースマートキャンペーンの優先度を低くすることもできます。

## API の強化 {#api-enhancements}

* **メールの開封トラッキングステータスの無効化を返却**：API を介したメールの開封トラッキングステータスの読み取りを許可します。
* **メールから動的コンテンツの件名行を取得**：マーケターが BI ツールで動的な件名行を分析できるようになります。
* **プログラムメンバーカスタムフィールドの CRUD**：マーケターがプログラムメンバーカスタムフィールドをプログラムで作成できるようになります。
* **カスタムオブジェクト一括エクスポート updatedAt フィルター**：マーケターがカスタムオブジェクトをプログラムで同期できるようになります。
* **メールプログラムの優先スタート設定を公開**：マーケターが API を介して優先スタートさせるメールプログラムを設定できるようになります。
* **選択的なプログラムタグ更新**：マーケターは、すべてのタグを同時にプッシュすることなく、選択的なタグの更新をプッシュできます
* **アクティビティ一括抽出 actionResult フィールド**：マーケターがスキップまたは失敗したアクティビティを識別できるようになります。

**_四半期を通した段階的リリース_**

以下の機能はリリース後約 1～2 か月の間に段階的にリリースされます。

## [!DNL Bizible] {#bizible}

![（星印）](assets/yellow-star.png)

* **BI テンプレート**：[!DNL Bizible] では、ビジネスニーズに合わせてカスタマイズされたカスタムレポートの迅速な開発を実現するため、Tableau および Power BI 用のダウンロード可能で基本的なレポートアーティファクトとサンプルレポートを提供するようになります。

## [!DNL Sales Connect] {#sales-connect}

![（星印）](assets/yellow-star.png)

* **メール接続のスロットリング（GA）**：メール接続のスロットリングを使用すると、[!DNL Sales Connect] 管理者は、Gmail または [!DNL Exchange] を配信チャネルとして使用する際のメールの送信率を設定し、配信チャネルプロバイダーに引き渡されるメールの割合が強制的な制限を超えるのを防ぐことができます。

## お知らせ {#announcements}

* **Marketo Sky の廃止**：Marketo Sky は 3月に利用できなくなります。これは、当社が次世代ユーザエクスペリエンスの提供にリソースを注力しているためです。 Marketo Sky 専用の機能へのアクセスを維持するため、アセットの有効期限とスマートキャンペーンの優先順位の上書きが Classic エクスペリエンスに取り入れられます。 [こちら](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33)をクリックすると、詳細が表示されます。

**_製品リリースウェビナー_**

[2022年3月と5月のMarketo Engage リリースウェビナー](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}

## 2022年5月 {#may}

以下に、5月23日リリースに含まれるすべての機能を示します。 利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

>[!AVAILABILITY]
>
>星印（![星印](assets/yellow-star.png)）で示す機能は有償オプションです。 詳細は Marketo Engage 担当営業にお問い合わせください。

**_四半期リリース_**

以下の機能のリリースは、**2022年5月6日**&#x200B;に始まり、（特に指定のない限り）その次の週から残りの機能が段階的にロールアウトされます。

## ネイティブ CRM 統合 {#native-crm-integration}

**[ネイティブ Veeva CRM 統合](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"}（限定的に利用可能）**：ネイティブ統合を介して Veeva CRM と Marketo Engage 間でアクティビティを同期させることで、医療専門家とのエンゲージメントを向上させます。 この統合により、マーケターは、医療専門家向けに、高度にパーソナライズされたシームレスなクロスチャネルエクスペリエンスを作成できます。 参加をご希望の方は、カスタマーサクセスマネージャーにお問い合わせください。

## クロスチャネルオーケストレーション {#cross-channel-orchestration}

**[!DNL Dynamic Chat]** 用チャットボットイベント：ページ滞在時間、サイト滞在時間、ページスクロール率など、web 訪問者のより詳細な行動データを活用して、チャットダイアログを表示するタイミングを定義します。

**[!DNL Dynamic Chat]** の PDF 埋め込み：チャットダイアログに PDF を埋め込むことによって、エンゲージメントを増やし、意味のあるコンテンツを共有します。また、エンゲージメントアクティビティのトラッキングを通じて、コンテンツのパフォーマンスを測定します。

**[!DNL Dynamic Chat]** の拡張言語サポート：[!DNL Dynamic Chat] のユーザインターフェイスが、フランス語、ドイツ語、日本語、ポルトガル語、スペイン語でも使用できるようになりました。 チャットダイアログは、これらの言語でも設定できます。

**[!DNL Dynamic Chat]** の URL を除外：ターゲティング条件から特定の URL を除外する機能と共に、[!DNL Dynamic Chat] が表示される web ページを制御します。

**[メールボットアクティビティのフィルタリング強化](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**：既存の IAB リストの一致識別に加えて、非表示リンクのユーザーエージェントまたは IP と近接性パターンに基づいてボットの動作を識別する機能により、引き続きデータベースの正常性を保護します。 ボットアクティビティの統計を表示して、各タイプで識別されたボットアクティビティの数を把握できます。

**[メールトラッキングリンクの STS ヘッダー](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**：セキュリティのベストプラクティスに従い、セキュリティで保護されたトランスポートセキュリティヘッダーを適用して、トラッキングされるリンクへのトラフィックが常にセキュリティで保護されるようにします。

## 次世代エクスペリエンス

**切り替えスイッチのデフォルト設定は次世代エクスペリエンス**&#x200B;です。切り替えスイッチは、利用可能なすべての画面で新しいエクスペリエンスにデフォルト設定されるので、更新されたデザインとユーザビリティの機能強化をユーザーが簡単に見つけることができます。

**次世代エクスペリエンスのアップデートされた画面**：

次世代のエクスペリエンスで[!UICONTROL Design Studio]内の電子メールテンプレートの詳細ビューを提供し、切り替えスイッチを介してアクセス可能な最新のデザインとユーザビリティの機能強化を提供します。

## エクスペリエンスの自動化 {#experience-automation}

**セルフサービスのフローステップ（継続ベータ版）**：スマートキャンペーンで使用するカスタマイズされたフローステップを作成する機能により、Marketo Engage とスタックの他の部分との接続性を拡張できます。 Marketo Engage のユーザとパートナーの両方がこの機能を活用して、（トリガーキャンペーンでのみ使用できる web フックとは異なり）トリガー、バッチ、実行可能なキャンペーンで外部の web サービスを使用できます。

## API の強化 {#api-enhancements}

* **CRM 対応サブスクリプションの API アクセスの拡張**：CRM 同期が有効になっているサブスクリプションの API アクセスを拡張し、ユーザが Marketo Engage から会社、商談、セールス担当者を取得できるようにします。
* **Formsの「非表示」データタイプのサポート**: APIを介して非表示フォームフィールドを管理する機能を提供します。
* **ルールを使用した isNot フォームの複数の比較値のサポート**：別のフィールドの値が特定のリストの値に含まれていないかどうかに基づいて、フォームフィールドの表示を管理します。
* **選択リストの表示値と送信済み値の設定を個別に許可**：表示値と送信済み値を別々にフィールドに設定します。 例えば、ホテルの名前を表示するが、内部 ID をバックエンドに送信する場合などです。
* **メールの作成または更新時に開封のトラッキングを無効にする設定を許可**：開封のトラッキングを無効にしたメールを作成します。

## お知らせ {#announcements}

**メールの検証と一意性**：4月から、メール検証のロールアウトが開始されます。 その時点で、Marketo Engage ユーザのメールアドレスには、検証と一意性が必須となります（API のみのユーザには適用されません）。 ディレクトリサービスの認証済みユーザは、メールの検証でサブスクリプションが有効になっている場合、自動的にメールを検証します。

「[!UICONTROL &#x200B; ユーザーを招待ダイアログにログイン &#x200B;]」機能を使用するか、複数のユーザーに関連付けられた1つの電子メールを持つサブスクリプションの電子メール検証は、5月のリリースと一致します。 複数のユーザに関連付けられた単一のメールを持つサブスクリプションは、メールの検証で有効になり、競合を解決してユーザごとに一意のメールを使用するよう求められます。 「ユーザーを招待ダイアログにログイン」機能が有効になっている場合、この機能を介して招待されたユーザーには一意のメールアドレスが必要になります。 API のみのユーザがこの機能を使用して招待された場合、メールアドレスを一意にする必要はありません。

**フォルダー動作の変更をアーカイブ**：このリリースで、アーカイブフォルダーに新しいアセットを作成する機能は、ツリーのコンテキストメニューから使用できなくなりました。 新しいアセットを作成するためのメニューオプションは、すべてのアセットで非表示になります。 詳しくは、[こちらを参照](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}してください。

**_製品リリースウェビナー_**

[2022年3月と5月のMarketo Engage リリースウェビナー](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}

## 2022年6月 {#june}

以下に、2022年6月リリースに含まれるすべての機能を示します。 利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

>[!AVAILABILITY]
>
>星印（![星印](assets/yellow-star.png)）で示す機能は有償オプションです。 詳しくは、Marketo Engage 担当営業にお問い合わせください。

以下の機能のリリースは、**2022年6月24日**（PT）に始まり、（特に指定のない限り）その次の週から残りの機能が段階的にロールアウトされます。

## マーケティングデータ環境 {#marketing-data-environment}

* **カスタムオブジェクトの CreatedAt／UpdatedAt フィールドの公開**：人物の詳細画面でこれらのフィールドを調べて、さらなるインサイトを得ることができます。

## クロスチャネルオーケストレーション {#cross-channel-orchestration}

* **[!DNL Dynamic Chat]** のストリームデザイナーの使いやすさの向上：ドラッグ＆ドロップを必要とせずに、ストリームデザイナーのキャンバスから直接カードを追加できます。 また、[!DNL Dynamic Chat] インターフェイスを改良し、個々のカードでのコンテンツの可視性が向上しました。

* **[!DNL Dynamic Chat]** の高度な予定ルーティングルール：[!DNL Dynamic Chat] は、ターゲットの予定ルーティングに対してさらに多くのオプションを提供します。 Marketo Engage の属性に基づいてルーティングするエージェントの予定を指定し、リードを適切なエージェントにルーティングします。

* **[!DNL Dynamic Chat]** の高度なダイアログレポート：エンゲージメント指標とコンバージョン指標に関する新しいデータビジュアライゼーションを使用して、[!DNL Dynamic Chat] のキャンペーン効果をより詳しく表示します。

* **[!DNL Dynamic Chat]** で使用されない Marketo Engage 属性の同期解除：[!DNL Dynamic Chat] サブスクリプションから未使用の Marketo Engage 属性の同期を解除することで、データを簡単に整理でき、必要に応じて代替の属性を同期できます。

## 次世代のエクスペリエンス

**新しい切替スイッチ表示**：次世代のエクスペリエンスで、以下の表示を利用できるようになりました。

* [メールの詳細表示](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [メールリスト表示](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## エクスペリエンスの自動化 {#experience-automation}

* **グローバルフォームフィールド検証ルールの除外**：グローバルフォーム検証ルールから特定のフォームを除外して、サブスクリプションセンターや他のビジネスクリティカルなワークフローがすべての値を受け入れるようにします。

* **セルフサービスのフローステップ**：スマートキャンペーンで使用するカスタマイズされたフローステップを作成する機能により、Marketo Engage とスタックの他の部分との接続性を拡張できます。 Marketo Engage のユーザとパートナーの両方がこの機能を活用して、トリガーキャンペーンでのみ使用できる web フックとは異なり、トリガー、バッチ、実行可能なキャンペーンで外部の web サービスを使用できます。

* **Munchkin プロトコル非依存リンクトラッキング**：Munchkin による `tel` と `mailto` のリンクトラッキングのサポートを拡張して、展開された一連の web 動作をトラックします。

* **Webhook 用の追加の HTTP メソッド**：Web サービスとやり取りするリクエストの種類として、PUT、PATCH、DELETE を指定します。

## [!DNL Sales Insight] {#sales-insight}

![（星印）](assets/yellow-star.png)

* **[!DNL Sales Insight]&#x200B;[!DNL Salesforce]** での権限セット：管理者は、[!DNL Sales Insight] [!DNL Salesforce] パッケージの一部である Marketo アプリ権限セットを使用して、プロファイルレベルではなく、ユーザレベルで限られた一連のユーザに対して [!DNL Sales Insight] のアクセス権を提供できます。

* **My Marketo タイルのアップデート - [!DNL Sales Insight]アクション**：Marketo 管理者（および指定したユーザ）は、マイ Marketo ページにある新しい [!DNL Sales Insight] アクションタイルから、[!DNL Sales Insight] アクションインスタンスにすばやく移動できるようになりました。

## [!DNL Sales Connect] {#sales-connect}

![（星印）](assets/yellow-star.png)

* **[!DNL Salesforce]API のアップデート**：[!DNL Salesforce] 2022 年夏のリリースで、[!DNL Salesforce] は API のレガシーバージョン 21～30 のサポートを終了します。 この Marketo Engage リリースにより、API のレガシーバージョンを使用する [!DNL Sales Connect] リクエストがすべてアップデートされ、サポート対象バージョン内に含まれるようになります。 [!DNL Salesforce] API 廃止プランについて詳しくは、[こちら](https://help.salesforce.com/s/articleView?language=en_US&type=1&id=000354473){target="_blank"}をクリックしてください。

## API の強化 {#api-enhancements}

* **Bulk Program Member Extract API の新しいフィルタリング機能**：プログラムメンバーシップのステータス、updatedAt、ケイデンス、消費済みコンテンツでフィルタリングして、抽出したデータセットを絞り込みます。

* **Bulk Program Member Extract API の向上**：ジョブの作成中に最大 10 個のプログラムを指定してスループットを向上させます。

## お知らせ {#announcements}

* **Forms の廃止 - Forms 1.0、リードキャプチャ／保存エンドポイント、非スクリプトバージョンのフォーム**：Forms 1.0 アセットのサポートは、2022年10月までに Marketo Engage から完全に削除されます。 既存の Forms 1.0 アセットはすべて機能を停止します。 Marketo Engage フォームは、ランディングページや web サイトの読み込みに JavaScript が必要です。

**_製品リリースウェビナー_**

[2022年6月と8月のMarketo Engage リリースウェビナー](https://engage.marketo.com/jp/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}

## 2022年8月 {#august}

以下に、2022年8月リリースに含まれるすべての機能を示します。 利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

>[!AVAILABILITY]
>
>星印（![星印](assets/yellow-star.png)）で示す機能は有償オプションです。 詳しくは、Marketo Engage 担当営業にお問い合わせください。

次の機能は、**2022年8月26日（PT）**&#x200B;に段階的にロールアウトを開始しました。

## クロスチャネルオーケストレーション {#cross-channel-orchestration}

* [!DNL Dynamic Chat] に対してすべての公開済みダイアログを一度に有効／無効にする**：ボタンを押しながら、設定ページからすべての公開済みダイアログを一度にグローバルに有効／無効にします。

* **[!DNL Dynamic Chat]** 用カスタムアバター：カスタムチャットボットアバターをアップロードして、ブランドにパーソナライズできるようにします。

* **[!DNL Dynamic Chat]** 用チャットトランスクリプト：すべての会話のチャットトランスクリプトを表示して、それぞれの web 訪問者が興味を持っているものについて、より深いインサイトを入手します。

## 次世代のエクスペリエンス

* **アドビブランディング**：新しい Adobe Experience Cloud ブランディングで、エディターおよび個人詳細ページのルックアンドフィールをアップデートしました。

* **移動ダイアログでの保存先フォルダーのフォルダー階層の表示**：各フォルダーのフォルダー階層を表示すると、アセットの移動が容易になり、誤ったフォルダーに入れられる可能性が低減されます。

* **[次世代エクスペリエンスのための画面の更新](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md){target="_blank"}**：次世代のエクスペリエンスで、切替スイッチを介してアクセス可能な、最新のデザインと操作性の強化を備えた新しい画面を追加しました。

   * スニペット詳細
   * 「画像とファイル」詳細

>[!NOTE]
>
>例外は、マーケティングアクティビティのプログラム内のフォルダーにアセットを移動することです。 プログラム内のフォルダーは重複した名前を持つことができないので、この移動アクションではフォルダー階層が表示されません。

## エクスペリエンスの自動化 {#experience-automation}

* **[セルフサービス型フローステップ - プログラム読み込み機能強化](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/flow-step-service.md){target="_blank"}**：カスタムフローステップを使用したプログラム読み込みのサポートが改善されました。これにより、同じサービスプロバイダーの複数のインスタンスを使用して、サービスプロバイダーと互換性のあるフローステップを持つプログラムを読み込めるようになりました。

* **[!DNL Munchkin]- リンクトラッキングの拡張**：Munchkin による `tel` リンクと `mailto` リンクのトラッキングのサポートを拡張し、より幅広い web 行動をトラッキングできるようになりました。

* **Web フックカスタムヘッダーの表示**：Web フックカスタムヘッダーが、[!UICONTROL 管理者]／「[!UICONTROL Web フック]」タブに表示され、可視性が向上しました。

* **CAPTCHA**：[reCAPTCHA v3 を使用](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"}して、フォーム送信の有効性を評価し、受信フォームトラフィックをスコアリングします。 疑わしいボットトラフィックを自動的に除外、強制隔離または削除するマーケティングワークフローを作成します。

* **フォームの承認権限**：他の[!UICONTROL デザインスタジオ]のアセットと連動して、フォームの変更を承認できるデザイナーを制御する新しい権限が追加されました。 これにより、承認権限を持つデザイナーがレビューを行わない限り、他のデザイナーがフォームに変更をプッシュすることができなくなります。

* **匿名結合後に常にキャンペーンリプレイを実行**：匿名リードの結合はキャンペーンリプレイの前に実行されるので、匿名キャンペーンリプレイが実行された場合でも、カスタムフィールドフィルターは確実に機能します。

## マーケティングデータ環境 {#marketing-data-environment}

* **カスタムオブジェクト「[!UICONTROL 使用者]」フィールド**&#x200B;のUI切り捨てを修正：「使用中」のカスタムオブジェクトフィールドを識別しやすくなりました。これにより、必要に応じてカスタムオブジェクトからフィールドを削除できます。

## API の強化 {#api-enhancements}

* **Bulk Program Member Extract API の新しいフィルタリング機能**：プログラムメンバーシップのステータス、updatedAt、ケイデンス、消費済みコンテンツでフィルタリングして、抽出したデータセットを絞り込みます。

## [!DNL Sales Insight] {#sales-insight}

![（星印）](assets/yellow-star.png)

* **[[!DNL Sales Insight]  [!DNL Dynamic Chat]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}** との統合：[!DNL Sales Insight] パネルの [!DNL Dynamic Chat] からアクティビティを表示し、この新しいデータポイントを見込み客活動に活用します。

## お知らせ {#announcements}

**_製品リリースウェビナー_**

[2022年6月と8月のMarketo Engage リリースウェビナー](https://engage.marketo.com/jp/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}

## 2022年10月 {#october}

以下に、2022年10月リリースに含まれるすべての機能を示します。 利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

>[!AVAILABILITY]
>
>星印（![星印](assets/yellow-star.png)）で示す機能は有償オプションです。 詳しくは、Marketo Engage 担当営業にお問い合わせください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに該当し、リリースは **2022年10月14日**（PT）から開始し、その次の週から残りの機能が段階的にロールアウトされます。 リリースの機能と日付は変更される場合があります。 各機能のステータスについては、以下を確認してください。

### マーケティングデータ環境 {#marketing-data-environment}

</br>

* **プログラムメンバーのカスタムフィールド同期**：プログラムメンバー用にキャプチャされた拡張可能なフィールド（食べ物、セッション、トラックなどのイベント登録時の参加者の環境設定など）を双方向で同期する機能 Salesforceのキャンペーンメンバーフィールドで定義されています。

<table>
  <tr>
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr>
   <td>リリース</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md">プログラムメンバーカスタムフィールドの同期</a></td>
  </tr>
  </tbody>
</table>

* **Adobe Privacy Service の統合**：Privacy Service と調和し、Experience Cloud 製品全体のデータプライバシー規制へのコンプライアンスを自動化します。 現在、このサービスは、Adobe Identity Management システムにオンボーディングした Marketo Engage のお客様のみが利用できます。

<table>
  <tr>
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr>
   <td>リリース</td>
   <td><a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md">Adobe Identity Management</a></td>
  </tr>
  </tbody>
</table>

### 次世代のエクスペリエンス

</br>

* **次世代エクスペリエンスのための画面の更新**：次世代のエクスペリエンスで、切替スイッチを介してアクセス可能な、最新のデザインと操作性の強化を備えた新しい画面を追加しました。

   * ランディングページテンプレートの詳細
   * メールテンプレートリスト

<table>
  <tr>
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr>
   <td>リリース</td>
   <td><a href="/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md">切替スイッチ</a></td>
  </tr>
  </tbody>
</table>

* **メールテンプレートの詳細の「使用者」タブの拡張**：新しいエクスペリエンスでは、アセットのステータス、最終変更日、最終変更者など、メールテンプレートを使用しているアセットに関する追加情報が表示されます。 また、アセットで使用されるリストの検索、並べ替え、フィルタリングを行うこともできます。

<table>
  <tr>
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr>
   <td>リリース</td>
   <td>該当なし</td>
  </tr>
  </tbody>
</table>

* **レポートアセットフィルターのモーダル**：レポート設定モーダルの新しいデザインで、設定メニューで新しいアセットツリーと、作成日および変更日のフィルターを表示します。

<table>
  <tr>
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr>
   <td>リリース</td>
   <td>該当なし</td>
  </tr>
  </tbody>
</table>

### API の強化 {#api-enhancements}

</br>

* **リードの一括読み込み：セールス担当者との関連付け**：パリティ付きのリード REST API で一括読み込みプロセス中にリードをセールス担当者に関連付け、複雑さを軽減し、必要な API 呼び出し数を減らすことができます。

<table>
  <tr>
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr>
   <td>リリース</td>
   <td><a href="https://developer.adobe.com/marketo-apis/api/mapi/#tag/Bulk-Import-Leads">リードの一括読み込み</a></td>
  </tr>
  </tbody>
</table>

### セールスインサイト {#sales-insight}

</br>

![（星印）](assets/yellow-star.png)

* **セールスインサイトと Dynamic Chat の統合**：インサイトダッシュボードに、スマートグリッドの動的チャットアクティビティと、週別の概要および詳細カードが含まれるようになりました。

<table>
  <tr>
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr>
   <td>リリース</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md">動的チャットの統合</a></td>
  </tr>
  </tbody>
</table>

## アジャイルリリースの機能

以下の機能は、アジャイル形式に従い、標準リリース日前後の様々な日付にリリースされます。 各機能のステータスについては、以下を確認してください。

* **動的チャットのダイアログストリームの自動配置**：混み合ったダイアログキャンバスが、「自動配置」ボタンを押すことで、すべての項目がきれいで読みやすい形式に整理され、改善されます。

<table>
  <tr>
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr>
   <td>リリース</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-icons">ストリームデザイナーのアイコン</a></td>
  </tr>
  </tbody>
</table>

* **動的チャットのミーティングリンク**：訪問者に送信されるすべてのカレンダー招待に、Google と Outlook の Teams または Meet のリンクを自動的に含めるオプションです。

<table>
  <tr>
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr>
   <td>リリース</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md">カレンダー</a></td>
  </tr>
  </tbody>
</table>

* **動的チャットの追加のデータタイプをサポート**：3 つの新しいデータタイプ（ブーリアン、整数、浮動少数）を使用すると、スコアに基づくターゲティングや、訪問者に「はい／いいえ」回答形式で質問するなど、動的チャットの既存の Marketo Engage フィールドをより活用できます。

<table>
  <tr>
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr>
   <td>リリース</td>
   <td>該当なし</td>
  </tr>
  </tbody>
</table>

## お知らせ {#announcements}

* **Forms 1.0**：Forms 1.0 の廃止は 10月のリリースで完了します。 Forms 1.0 のアセットは Marketo Engage にデータを送信できなくなり、試行するとエラーが返されます。

* **スクリプトなし Forms**：ブラウザーで JavaScript が無効になっている場合、Forms は機能しなくなります。 フォームの送信には、JavaScript を有効にする必要があります。

