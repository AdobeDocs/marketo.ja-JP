---
description: リリースノート - 2021 年 1 月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2021 年 1 月
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 76%

---

# リリースノート：2021 年 1 月 {#release-notes-jan-21}

2021 年 1 月リリースには以下の新機能が含まれています。お客様のご契約により、制限やオプションの契約が必要なものがあります。詳細は担当の営業にお問い合わせください。

>[!AVAILABILITY]
>
>星印（![（星印）](assets/yellow-star.png)）がついている機能は有償オプションになります。詳細は Marketo Engage 担当営業にお問い合わせください。

**_四半期リリース_**

以下の機能は **2021 年 1 月 15 日**（PT）にリリースされます。

## 次世代ユーザエクスペリエンス {#next-generation-user-experience}

* ワークスペースのサポート：Marketo Engage の次世代ユーザエクスペリエンスにより、Adobe Experience Cloud のルックアンドフィールと、生産性を高めるイノベーションを組み合わせることで、マーケティング実行者は迅速かつスマートに作業を行うことができます。最新のリリースでは、ワークスペース間でフォルダーを共有する機能を含む、ワークスペースとパーティションの完全なサポートが追加されます。右側のキャンバスに切り替えスイッチが表示され、コンテキストを失うことなく、機能ごとに古いエクスペリエンスと新しいエクスペリエンスをシームレスに切り替えることができます。詳しくは、Marketing Nation の次世代エクスペリエンス FAQ を[ご覧ください](https://nation.marketo.com/t5/The-modern-ux/modern-ux-FAQ/ba-p/307124)。

## マルチチャネルのパーソナライゼーション {#multi-channel-personalization}

* **[Adobe Experience Cloud オーディエンス同期フェーズ 3](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**：既存の Adobe Experience Cloud（AEC）オーディエンス同期機能で、Marketo Engage からリアルタイム顧客データプラットフォームや Adobe Experience Platform アクティベーションなどの Adobe Experience Platform（AEP）製品を含む、その他の AEC アプリケーションへの継続的な双方向 B2B オーディエンス同期がサポートされるようになりました。リードがオーディエンスセグメントに追加されたり削除されたりすると、Marketo Engage は、接続された AEC アプリ間で更新されたオーディエンスを自動的に同期します。AEC 技術スタック全体で、アドビのマルチチャネルオーケストレーション、リターゲティング、オーディエンス抑制、パーソナライゼーションおよびレポートのユースケースを活用するために使用します。
* **[Google、 [!DNL Facebook]、および [!DNL LinkedIn]](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)** に対する継続的なオーディエンス同期：静的なリストで有効化した場合に、ユーザーの操作を必要とせずに、リストメンバーシップの変更に合わせて Ad Network を更新する、Ad Network による継続的な自動同期が可能です。
* **[プログラムメンバーカスタムフィールドのトークン](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)**：トークンフレームワークをサポートするために、プログラムメンバーカスタムフィールド機能が拡張されました。マーケターは、プログラムメンバーカスタムフィールドトークンを電子メール、ランディングページ、SMS メッセージ、プッシュ通知、web フックに挿入できます。キャンペーンフローアクションの新しいトークンを使用して、データ値の変更、タスクや注目のアクションを作成します。

## ランディングページと Forms {#landing-pages-and-forms}

* **フォーム API**：リード情報を取り込むか、Marketo 以外のフォームからデータを取り込みながらナーチャリングキャンペーンをトリガーします。Marketo 以外のフォームは、REST API を使用して Marketo Engage と連携できます。新しい API では、関連するすべての機能を使用して、Marketo Engage フォームの送信を模倣できます。
* **ランディングページ API**：新しいランディングページプレビュー API を使用して、連携されたアプリケーションでの編集と翻訳のワークフローを合理化します。サードパーティベンダーは、Marketo Engage にログインすることなく、ランディングページの完全にパーソナライズされたプレビューをレンダリングできるようになりました。ランディングページプレビュー API を使用すると、サードパーティの連携アプリケーションで、エンドツーエンドの編集およびローカライゼーションワークフローが可能になります。

## メールマーケティング {#email-marketing}

* **[カスタムオブジェクトの取得制限の増加](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)**：メールベロシティスクリプティングの開発者は、セルフサービスの上書きを通じて、カスタムオブジェクトの数を 100 に素早く増やせます。マーケターは、多数の第 1 レベルおよび第 2 レベルのカスタムオブジェクトにアクセスすることで、スマートキャンペーンの効果を高めることができます。

## [!DNL Salesforce] CRM 統合 {#salesforce-crm-integration}

* [[!DNL Salesforce] CRM 認証 ](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md):Marketo Engageと CRM の間で操作を同期するために、OAuth 2.0 プロトコル [!DNL Salesforce] 使用できます。 新規契約者の場合、このオプションはデフォルトで有効になっています。現在の契約者は、Marketo サポートに問い合わせて、この機能をリクエストできます。
* [[!DNL Salesforce] CRM 同期ダッシュボード ](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md)：管理者はダッシュボードから CRM 同期 [!DNL Salesforce] ステータスをすばやく確認できます。 パフォーマンスレポートの同期期間が 2 時間から 5 日に増えました。
* **メタデータのエクスポート**：商談オブジェクトの属性、名前付きアカウント、プログラムメンバーの標準フィールドおよびカスタムフィールドをサポートするように拡張されました。

## 管理 {#administration}

* **マイアカウントページの更新**：マイアカウントページで必要なサブスクリプション情報を確認します。任意のレベルのアクセス権を持つユーザーは、サブスクリプション名、データセンター識別子、[!DNL Munchkin] ID を表示できます。

**_四半期を通した段階的リリース_**

以下の機能はリリース後約 1～2 か月の間に段階的にリリースされます。

## [!DNL Sales Insight] {#sales-insight}

![（星印）](assets/yellow-star.png)

* **[強化されたテストメールワークフロー（[!DNL Salesforce] CRM）](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**：強化された [!DNL Sales Insight] テストメールワークフローにより、セールスチームの効率を向上させます。 販売者は、最大 200 人の受信者にメールを一括送信する前に、選択したメールアドレスにテスト用メールを送信できます。
* **[メールステータス（[!DNL Salesforce] CRM）に関するインサイト](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**：無効なメール ID または登録解除されたメールアドレスにメールを送信しようとする際、メール送信前に警告メッセージが表示されます。  メール配信ステータスは、[!DNL Sales Insight] の「メール」タブで確認できます。
* **[ アカウント ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) および [ 商談 ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) パネル（[!DNL Salesforce] CRM）からの一括メール送信**：新しい一括アクション機能を使用して、販売者のワークフローの効率を向上させ、アカウントまたは商談の連絡先リスト全体に関与させます。 個々の取引先責任者を扱う代わりに、「アカウント」または「商談」タブの新しいドロップダウンオプションを使用して、Marketo Engage キャンペーンにメールを送信したり、取引先責任者を追加したりできます。リードがホットになったときに通知を受けるために、アカウントの取引先責任者をウォッチリストに追加します。
* **[[!DNL Sales Insight] Non-Native [!DNL Salesforce] CRM 統合の場合](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)**：カスタムのSalesforce CRM 統合による GA 版のサブスクリプションでは、[!DNL Sales Insight] パッケージをインストールして、セールスチームが最も有望なリードやオポチュニティを優先順位付けしてやり取りできるようにします。
* **[ベストプラクティスの強化](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)**：「ベストベット」タブからホットリードに素早く連絡するには、リードをメールで送信するか、Marketo Engage キャンペーンに追加します。リードを Marketo Engage で表示するか、ウォッチリストに追加します。[!UICONTROL &#x200B; ベストベット &#x200B;] タブの一括アクションと並べ替えオプションにより、時間を節約し、セールスチームの効率を向上させることができます。

## [!DNL Sales Connect] {#sales-connect}

![（星印）](assets/yellow-star.png)

* **E メール接続スロットル（BETA）**:[!DNL Sales Connect] 向けの E メール接続スロットルにより、E メールの配信品質を向上させ、1 対 1 のセールスコミュニケーションを拡大します。 アドビの新しいスロットルテクノロジーは、メール送信のタイミングを自動的に管理し、[!DNL Exchange] および Gmail ユーザーにシームレスなエクスペリエンスを作成します。 サードパーティのメール一括送信アプリケーションの使用が減少する、または不要になります。
* **メール接続バウンストラッキング**：新しいメールバウンスレポートを使用して、リードの品質とメールテンプレートのパフォーマンスに対するインサイトを獲得します。[!DNL Exchange] および Gmail ユーザーは、ライブフィード、メールフォルダー、テンプレート分析およびキャンペーン分析にロールアップされるバウンス通知の受信を選択できます。
* **プロファイルページの設定**：新しいプロファイルページで、簡単にユーザの環境設定を管理できます。パスワードの変更、位置情報と言語の設定の編集、連携ステータスの確認を 1 箇所で行います。
* **テンプレートの管理**：新しいドラッグ＆ドロップ機能でセールスのメールテンプレートをカテゴリ別に整理し、関連するテンプレートに素早くアクセスして検索時間を短縮できます。
* **[!DNL Sales Connect]User Experience Updates**：列のサイズ変更 [!DNL Sales Connect] 並べ替えによるグリッドレイアウトのカスタマイズ。 表示環境設定が自動的に保存されます。

**_告知情報＆廃止予定機能_**

* すべてのユーザは、**2021年1月15日より前**&#x200B;に、Sales Insight の最新バージョンにアップグレードする必要があります。アップグレードを完了していない場合は、アプリケーションにログインする際に、アップグレードを完了するよう求められます。[このガイド](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md)の手順に従ってください。更新版には、識別されたセキュリティ脆弱性に対するパッチが含まれています。このパッチは、2016 年 4 月 6 日にリリースされました。注意：**バージョン 1.4363 以降**&#x200B;は、アップグレードを実行する必要はありません。
* Form 1.0 サービスの廃止は、**2021 年 5 月**&#x200B;のリリースで有効になります。Forms 1.0 サービスは完全に廃止されるので、残りの Forms 1.0 アセットが引き続き使用されている場合は機能が失われます。また、プログラム形式の POST や leadCapture/save および leadCapture/save2 エンドポイントへの送信など、サポートされていない方法で行われたフォーム送信は拒否されます。詳細と修正については、[Marketing Nation の投稿](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631)を参照してください。
* 2021 年、Marketo Engage は、ランディングページ、フォーム、画像、ファイルアセットの URL 構造を変更する予定です。既存の Marketo Engage のサブスクリプションについては、2021 年 4 月 1 日（PT）に段階的なロールアウトを開始します。ロールアウトのタイムラインについて詳しくは、2021 年 3 月にリリース予定です。影響を受ける各アセットタイプの変更方法について詳しくは、[Marketing Nation の投稿](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632)を参照してください。

**_製品リリースウェビナー_**

これらの機能および機能強化の詳細を確認するには、[今すぐ登録](https://engage.marketo.com/January_21_Release_Webinar_Registration.html)して、1 月 21 日の午後 1 時（PT）／午後 4 時（ET）に開催される製品チームとのライブウェビナーに参加して、イノベーションに対する理解を深めてください。
