---
unique-page-id: 37355534
description: リリースノート - 2020 年 1 月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2020 年 1 月
exl-id: 7b011c1a-1161-42f8-8bd0-4ee273928b59
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: ht
source-wordcount: '796'
ht-degree: 100%

---

# リリースノート：2020 年 1 月 {#release-notes-jan}

2020 年 1 月リリースには以下の新機能が含まれています。お客様のご契約により、制限やオプションの契約が必要なものがあります。詳細は担当の営業にお問い合わせください。

>[!AVAILABILITY]
>
>星印（![（星印）](assets/yellow-star.png)）がついている機能は有償オプションになります。詳細は Marketo Engage 担当営業にお問い合わせください。

**_四半期リリース_**

以下の機能は **2020 年 1 月 17 日**（PT）にリリースされます。

## コア Marketo Engage アドビアプリ {#core-marketo-engage-adobe-application}

* [Adobe Experience Manager Asset Selector](/help/marketo/product-docs/adobe-experience-cloud-integrations/importing-assets-with-adobe-experience-manager.md)：Marketo Engage で直接使用できる AEM アセットでブランドに合ったアセットにすばやくアクセスできます。メモ：この機能は、Marketo Sky と従来の両方のエクスペリエンスで使用できますが、管理機能は Classic エクスペリエンスで使用できます。バージョン 6.5 以降の AEM Assets を使用中が必要です。

>[!NOTE]
>
>現在、AEM Asset Selector は Firefox でのみ完全にサポートされています。Safari ではサポートされていません。また、SameSite の Cookie 設定によっては、最新バージョンの Chrome（v.80）では動作しない可能性があります。

* **[!DNL Microsoft Dynamics]- リードをリアルタイムで CRM に同期**：Marketo Engage と [!DNL Microsoft Dynamics] の間でのリードと取引先責任者のリアルタイム同期。「リードを Microsoft に同期」フローアクションを使用して、リードまたは取引先責任者を作成し、[!DNL Microsoft Dynamics] ですぐに確認できます。
* **[!DNL LinkedIn]リードジェネレーションフォームの追加フィールドマッピング**：[!DNL LinkedIn] リードジェネレーションフォームからリードデータをキャプチャして、セールスとマーケティングの両方のタッチポイントに、より関連性の高いエクスペリエンスを作成できます。非表示のフィールド、同意フィールド、およびテストリードフィールドを Marketo Engage に取り込みます。
* **メールテンプレート依存関係 API**：メールテンプレートに依存するアセットのリストを取得して、変更の可能性の範囲と、テンプレートに対するアドレスの依存関係を把握し、テンプレートの変更と削除を迅速におこなうことができます。
* **マルチインスタンス管理の強化**：購読のスクロール可能なドロップダウンメニューとアルファベット順のドロップダウンメニューから、必要なインスタンスにすばやく移動します。

## アカウントベースドマーケティング {#account-based-marketing}

![（星印）](assets/yellow-star.png)

* [新しいアカウントの検出（ベータ版）](https://docs.marketo.com/x/WQA6Ag) ![（星）](assets/yellow-star.png)：アカウントプロファイルを使用して、AI を利用した理想的な顧客プロファイルモデルに基づいて、ABM 戦略の新しいターゲットアカウントを検出します。ABM ターゲティング用の Marketo Engage リードおよびアカウントデータベース内にまだ存在しない、推奨される新しいアカウントと、AI ベースの適合および目的データ指標を表示、選択、インポートします。資格のある顧客プロファイルを持つ顧客はすぐに使用できます。

<br> 

**_四半期を通した段階的リリース_**

以下の機能はリリース後約 1～2 か月の間に段階的にリリースされます。

## [!DNL Bizible] {#bizible}

![（星印）](assets/yellow-star.png)

* **Marketo Engage リード統合**：セールスとマーケティングに、[!DNL Bizible] と Marketo Engage をまたいだリードの統合ビューを提供します。このアップデートにより、Marketo Engage を追加のリードデータソースとして使用できるようになったので、リードが CRM と同期してリードジェネレーションに関するレポートを作成するのを待つ必要がなくなりました。
* **Discover の機能強化**：[!DNL Bizible] の Discover ボードの機能をさらに活用しましょう。お客様からのフィードバックに基づいて、タイルや属性からトランザクションレコードをドリルダウン、重要なレコード数と対応するコストパーメトリクスを追加、複数のダッシュボードのダッシュボードフィルターを追加／削除などの機能強化が行われました。また、ログイン時にデフォルトのダッシュボードに直接移動します。

## [!DNL Marketo Sky] {#marketo-sky}

* [画像編集](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/marketo-image-editor.html?lang=ja#design-studio)：Marketo Engage を終了せずに、アドビの編集機能にアクセスできます。この新しい機能により、[!UICONTROL Design Studio] で直接画像の拡張、切り抜き、画像へのテキストの追加などを簡単に実行できます。

## [!DNL Sales Insight] {#sales-insight}

* **[!DNL Salesforce Lightning]一括アクション**：[!DNL Salesforce Lightning] を使用して、最大 200 名の取引先責任者／リードをキャンペーンに追加し、Marketo Engage メールを一括で送信する機能でセールス効率を高め、購入者のエンゲージメントを維持します。
* **[!DNL Salesforce1]** のモバイルサポート：[!DNL Salesforce1] アプリで、注目のアクションや web アクティビティ、メールなど、すべての [!DNL Sales Insight] 機能に対するモバイルアクセスを外出先で利用できるようになりました。
* **UI の強化**：インターフェイスを更新して、読みやすさを強化し、[!DNL Marketo Sky] エクスペリエンスと一貫性のあるデザインにしました。

## [!DNL Sales Connect] {#sales-connect}

* **グリッドコンポーネント**：新しいグリッドカスタマイズ機能で [!DNL Sales Connect] インスタンスを最適化します。表示する列の選択、列の検索、すべての列の選択／選択解除、各ページに表示するデータの行数の指定をおこないます。
* **[コンテンツのロックダウン](/help/marketo/product-docs/marketo-sales-connect/admin/content-lockdown.md)**：管理者以外のユーザがテンプレートやキャンペーンを作成および編集できるかどうかを制御する、購読全体の設定によるブランドの調整を最大化します。

>[!NOTE]
>
>* **TLS 1.0 および 1.1 の廃止**：アドビのリリース構造との統合に向けて、TLS 1.0 および TLS 1.1 の廃止を 2020 年 1 月 13 日に移動しています。詳細は[こちら](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq)をご覧ください。
>
>* **ITP 2.1+ [!DNL Munchkin] のアップデート**：[!DNL Safari] の cookie ポリシーが変更されたので、[!DNL Munchkin] が同じドメインで複数のセッションをまたいでユーザを追跡する機能は、ITP によって、訪問者が使用しているブラウザーとブラウザーのバージョンに基づいて 1 日または 7 日に制限されます。これを考慮して、新しい web サービスを実装し、HTTP 応答を介して Set-Cookie ヘッダーで Munchkin の Cookie を設定できるようにしています。この新しいサービスの実装方法の詳細については、[こちら](https://nation.marketo.com/docs/DOC-7351)を参照してください。

**_製品リリースウェビナー_**：3 月 3 日午前 11 時（PT）／午後 2 時（ET）に開催される製品チーム主催のライブウェビナーに[参加](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html)して、今回のリリースに含まれる機能の詳細をご確認ください
