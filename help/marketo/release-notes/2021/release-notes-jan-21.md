---
description: リリースノート — 2021年1月 —Marketoドキュメント — 製品ドキュメント
title: リリースノート — 2021年1月
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
translation-type: tm+mt
source-git-commit: 7566581555eb95564b9f69884190dd987e123dbe
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 0%

---

# リリースノート：Jan 2021 {#release-notes-jan-21}

1月22日リリースには、次の機能が含まれています。 Marketo版で利用可能な機能を確認してください。

>[!AVAILABILITY]
>
>星印(![(star)](assets/star-yellow.svg))で示される特徴は有料のアドオンです。 詳しくは、Marketo Engageの担当者にお問い合わせください。

**_四半期別リリース_**

次の機能は、**2021年1月15日**&#x200B;にリリースされます。

## 次世代ユーザーエクスペリエンス{#next-generation-user-experience}

* ワークスペースのサポート：Marketo Engageの次世代ユーザーエクスペリエンスにより、Adobe Experience Cloudのルック&amp;フィールが生産性の革新と統合され、マーケティング担当者の作業が迅速かつ効率的になります。 最新リリースでは、ワークスペースとパーティションの完全なサポートが追加され、ワークスペース間でフォルダーを共有する機能も追加されています。 右側のキャンバスに切り替えスイッチがオファーされ、コンテキストを失うことなく、機能ごとに古いエクスペリエンスと新しいエクスペリエンスをシームレスにトランジションできます。 [Marketing Nationの次世代のエクスペリエンスFAQから](https://nation.marketo.com/t5/The-Next-Generation-Experience/Next-Generation-Experience-FAQ/ba-p/307124) さらに詳しく説明します。

## マルチチャネルパーソナライゼーション{#multi-channel-personalization}

* **[Adobe Experience Cloudオーディエンス同期フェーズ3](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**:既存のAdobe Experience Cloud(AEC)オーディエンス同期機能は、Marketo EngageからAdobe Experience Platform(AEP)製品(リアルタイム顧客データプラットフォーム、Adobe Experience Platformアクティベーションなど)製品への、連続的で双方向のB2Bオーディエンス同期をサポートするようになりました。リードがオーディエンスセグメントに追加および削除されると、Marketo Engageは、接続されたAECアプリ間で更新されたオーディエンスを自動的に同期します。 AECテクニカルスタック全体で、Adobeのマルチチャネルオーケストレーション、リターゲティング、オーディエンス抑制、パーソナライゼーション、レポートの使用例を活用するために使用します。
* **[Google、Facebook、LinkedInとの継続的なオーディエンス同期](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)**:広告ネットワークとの継続的な自動同期は、静的なリストで有効にでき、ユーザーの介入を必要とせずに、リストのメンバーシップの変更に応じて広告ネットワークを更新できます。
* **[プログラムメンバーのカスタムフィールド](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)**:プログラムメンバーのカスタムフィールド機能を拡張し、トークンフレームワークをサポートしました。マーケターは、電子メール、ランディングページ、SMSメッセージ、プッシュ通知、Webフックに、プログラムメンバーのカスタムフィールドトークンを挿入できます。 キャンペーンフローのアクションで新しいトークンを使用して、データ値の変更、タスクの作成、または興味深い瞬間を行います。

## ランディングページとForms{#landing-pages-and-forms}

* **フォームAPI**:Marketo以外のフォームからデータを取り込みながら、リードキャンペーンまたはトリガーの育成情報を取り込みます。Marketo以外のフォームは、REST APIを通じてMarketo Engageと統合できます。 新しいAPIでは、Marketo Engageフォームの送信と、関連するすべての機能を模倣できます。
* **ランディングページAPI**:新しいランディングページプレビューAPIを搭載した統合アプリケーションで、編集や翻訳のワークフローを効率化。サードパーティベンダーは、Marketo Engageにログインすることなく、完全にパーソナライズされたプレビューのランディングページをレンダリングできるようになりました。  ランディングページプレビューAPIを使用すると、サードパーティの統合アプリケーションでエンドツーエンドの編集およびローカライゼーションワークフローを行うことができます。

## メールマーケティング {#email-marketing}

* **[Custom Objects Retrieval Limits Increased](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)**:電子メール速度スクリプティングの開発者は、セルフサービスのオーバーライドを使用して、カスタムオブジェクトの数をすぐに100に増やすことができます。マーケターは、第1レベルおよび第2レベルのカスタムオブジェクトに多数アクセスすることで、スマートキャンペーンの効果を高めることができます。

## Salesforce CRM の統合 {#salesforce-crm-integration}

* [Salesforce CRM認証](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md):OAuth 2.0プロトコルは、Marketo EngageとSalesforce CRMの間の操作を同期するために使用できます。新規サブスクライバーの場合、このオプションはデフォルトで有効になっています。 現在のサブスクリプションをご利用の場合は、Marketoサポートにご連絡ください。
* [Salesforce CRM同期ダッシュボード](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md):管理者は、ダッシュボードからSalesforce CRMの同期ステータスをすばやく確認できます。同期パフォーマンスレポートの期間が2時間から5日に延長されました。
* **メタデータの書き出し**:名前付きアカウント、プログラムメンバーの標準フィールドおよびカスタムフィールドなど、オポチュニティオブジェクト属性をサポートするように強化されました。

## 管理 {#administration}

* **マイアカウントページを更新しました**:マイアカウントページで重要な購読情報を確認します。任意のレベルのアクセス権を持つユーザは、購読名、データセンターID、およびMunchkin IDを表示できます。

**_四半期全体でリリース_**

次の機能は、四半期に属さないサイクルで提供され、今後数か月間にわたってリリースされます。

## Sales Insight {#sales-insight}

![（星形）](assets/star-yellow.svg)

* **[テスト用電子メールワークフローの強化(Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**:Sales Insightのテスト用電子メールワークフローが強化され、セールスチームの効率が向上します。販売者は、選択した電子メールアドレスにテスト用の電子メールを送信してから、最大200人の受信者にバルクメールを送信できます。
* **[電子メールステータス(Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**:ユーザーは、電子メールを送信する前に、無効な電子メールIDまたは登録解除された電子メールアドレスに電子メールを送信しようとすると、警告メッセージを表示します。 電子メール配信のステータスは、Sales Insightの「電子メール」タブで確認できます。
* **AccountandOpportunityPanelsから [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) の一括電子メールの送信(Salesforce CRM) [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout)**:新しいバルクアクション機能を使用して、販売者のワークフローの効率性を向上させ、アカウント全体またはオポチュニティ連絡先リストに関与します。個々の連絡先で作業する代わりに、アカウントまたは商談タブの新しいドロップダウンオプションを使用して、Marketo Engageキャンペーンに電子メールを送信したり、連絡先を追加したりします。 ア追加カウントはウォッチリストに連絡し、リードがホットになったときに通知を受けます。
* **[ネイティブ以外のSalesforce CRM統合向けSales Insight](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)**:カスタムSalesforce CRM統合を利用したGA購読は、Sales Insightパッケージをインストールし、販売チームが最も有望なリードやオポチュニティに優先順位をつけ、やり取りするのを支援します。
* **[ベストベストの強化](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)**:Marketo Engageキャンペーンに電子メールまたは追加して、「ベストベット」タブのホットリードにすばやく連絡します。Marketo Engageのリードを表示するか、ウォッチリストに追加します。 「ベストベット」タブのバルクアクションと並べ替えオプションにより、時間を節約し、セールスチームの効率を向上できます。

## セールスコネクト {#sales-connect}

![（星形）](assets/star-yellow.svg)

* **電子メール接続の制限（ベータ版）**:Eメールの配信品質を向上させ、Sales Connectの電子メール接続スロットリングを使用して1:1の販売コミュニケーションを拡大します。アドビの新しいスロットリングテクノロジーは、電子メールの送信タイミングを自動的に管理し、ExchangeおよびGmailユーザーにシームレスなエクスペリエンスを提供します。 サードパーティの一括電子メール送信アプリケーションの使用を減らすか、減らします。
* **電子メール接続のバウンストラッキング**:新しい電子メールバウンスレポートを使用して、リードの質と電子メールテンプレートのパフォーマンスに関するインサイトを得ます。ExchangeおよびGmailのユーザーは、ライブフィード、電子メールフォルダー、テンプレート分析およびキャンペーン分析にロールアップされるバウンス通知の受信を選択できます。
* **プロファイルページ設定**:新しいプロファイルページで、簡単にユーザー環境設定を管理できます。パスワードの変更、位置情報および言語設定の編集、統合のステータスの確認を1か所で行います。
* **テンプレートの管理**:新しいドラッグ&amp;ドロップ機能により、販売用電子メールテンプレートをカテゴリに整理し、関連するテンプレートにすばやくアクセスでき、検索時間を短縮できます。
* **Sales Connect User Experience Updates**:列のサイズ変更と並べ替えを行って、Sales Connectのグリッドレイアウトをカスタマイズします。表示設定が自動的に保存されます。

**_お知らせと廃止_**

* すべてのユーザーは、2021年1月15日&#x200B;**までにSales Insightの最新バージョン**&#x200B;にアップグレードする必要があります。 アップグレードが完了していない場合は、アプリケーションにログインした後にアップグレードを完了するように求められます。 このガイド](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md)の[の指示に従ってください。 アップデートバージョンには、識別されたセキュリティ脆弱性に対するパッチが含まれます。 このパッチは、元々2016年4月6日にリリースされました。 注意：**バージョン1.4363以降**&#x200B;は、アップグレードを実行する必要はありません。
* Form 1.0サービスの廃止は、**2021年5月**&#x200B;リリースで有効になります。 Forms1.0サービスは完全に廃止され、残りのForms1.0アセットが引き続き使用中である場合は機能が失われます。 また、leadCapture/saveやleadCapture/save2エンドポイントに対するプログラム的なフォームPOSTなど、サポートされていないメソッドを通じて行われるフォーム送信は拒否されます。 詳細と修正方法については、[Marketing Nationの投稿](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631)を参照してください。
* 2021年には、Marketo Engageは、ランディングページ、フォーム、画像、ファイルアセットのURL構造を変更します。 既存のMarketo Engage購読については、2021年4月1日から段階的な展開を開始します。 公開日程の詳細は、2021年3月に発表予定です。 影響を受ける各アセットタイプの変更方法について詳しくは、[Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632)の投稿を参照してください。

**_製品リリースに関するウェビナー_**

これらの機能および拡張機能の詳細をご覧になりますか？ 1月21日午後1時（太平洋標準時間午後4時）には、ぜひ[今すぐ登録](https://engage.marketo.com/January_21_Release_Webinar_Registration.html)してください。当社の製品チームとのライブウェビナーで、これらの革新についてより深く掘り下げることができます。
