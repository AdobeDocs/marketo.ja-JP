---
unique-page-id: 12979858
description: パフォーマンスインサイトFAQ — マーケティングツールドキュメント — 製品ドキュメント
title: パフォーマンスインサイトFAQ
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '1404'
ht-degree: 0%

---


# パフォーマンスインサイトFAQ {#performance-insights-faq}

## 「エンゲージメント」タブの「成功」の定義は何ですか。 {#what-is-the-definition-of-success-in-the-engagement-tab}

成功とは、マーケティングにおける意味のあるインタラクションの尺度です。 プログラムの目的は、人や見込み客との有意義なインタラクションを作成することです。 成功は、その目標を達成したステータスに達したときにマークされます。 ウェビナーに参加したり、電子メール内のリンクをクリックしたり、Webフォームに入力したりできます。 成功は、プログラムのチャネルによって異なります。

>[!NOTE]
>
>**例**
>
>ウェビナープログラムでは、次のような複数のステータスがある場合があります。招待、登録および参加。 招待や登録は、実際にウェビナーを見ないので、意味のあるインタラクションではありません。 この場合、「出席」は成功と見なされます。

## MPIはどのCRMでも動作しますか。 {#will-mpi-work-with-any-crm}

はい。 技術的には、MPIはCRMと直接やり取りしてデータ同期を行いません。 MPIは、Marketo AnalyticsData Warehouseに保存されたデータを利用します。 CRMの同期はリード管理アプリケーションで行われるので、リード管理アプリケーションに統合されたマーケティング担当者がサポートするCRMには、データが正しく表示されます。 ただし、CRMのオポチュニティフィールドは、Marketoのオポチュニティフィールドに正しくマップされている必要があります。

## 他のMarketing Analytics製品(ARB、RCE、RCA、プログラム分析)はありません。 MPIは私のために機能するの？ {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPIは、リード管理アプリケーションに対する独立したアドオンです。 他の解析製品を使用する必要はありません。

## RCAはプログラムのパフォーマンスデータも表示します。 MPIとRCAに表示されるデータに違いはありますか。 {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

いいえ。 MPIソースのデータは、RCAと同じデータウェアハウスから取得されます。 したがって、この2つのデータの違いは一切見られません。 RCAを使用すると、自分のレポートをその場で作成できます。 MPIを使用すると、わかりやすいビジュアルダッシュボードにアクセスできます。

## MPIでプログラム（運用環境など）の一部を表示したくない。 特定のプログラムの表示/非表示を制御する方法を教えてください。 {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

プログラムのAnalytics動作を「運用」に設定することで、プログラムの表示を制御できます。 これにより、プログラムが分析の計算から除外されます。

>[!NOTE]
>
>解析動作の設定について詳しくは、 [ここを参照してください](http://docs.marketo.com/display/public/DOCS/Edit+Analytics+Behavior+Settings)。

## 新製品の発売時にマルチチャネルキャンペーンを実行しています。 このキャンペーンのパフォーマンスを、様々なチャネル全体で1か所に表示する方法を教えてください。 {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

このようなキャンペーンのプログラムには、プログラムタグを使用することをお勧めします。 プログラムタグはMPIに自動的に同期され、すべてのMPIダッシュボードでフィルタリングして、マルチチャネルキャンペーンのパフォーマンスを表示できます。

## RCAがない場合、アトリビューション設定にアクセスできますか？ {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

MPIを使用している場合は、RCAの有無に関係なく、アトリビューション設定にアクセスできます。

## MPIでログイン時に、属性設定が正しくないという警告が表示されます。 何か問題が？ {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPIは、すべてのオポチュニティが分析に含まれているかどうかを計算します。 そうでない場合は、より多くのオポチュニティを含めるためにアトリビューション設定（明示的、暗黙的、ハイブリッド）の変更を検討するよう求められます。

また、プログラムにプログラムコストがないためにオポチュニティが見つからない場合もあります。 プログラムのAnalyticsの動作を確認してください。 次のように指定できます。

1. デフォルト — MPI ONLYに含まれるプログラムは、期間コストが1つ以上の場合（ドルがゼロの場合も含む）のみです。
1. 包括的 — このオプションは、期間のコストが含まれているかどうかに関係なく、MPIでプログラムを使用できるようにします。
1. [操作](http://docs.marketo.com/display/DOCS/Best+Practice%3A+How+to+Organize+your+Programs#BestPractice:HowtoOrganizeyourPrograms-OperationalPrograms) — このオプションを選択すると、MPIにプログラムが表示されません。

>[!NOTE]
>
>エンゲージメントダッシュボード **の成功と新しい名前のレポートに対して期間コストを設定する必要があります** 。 このダッシュボードでは、集計の成功や新しい名前に期間コストのデータを利用します。 期間コストが設定されていない場合、上記のAnalyticsの動作設定に関係なく、エンゲージメントダッシュボードは正しくレポートされません。

## MPIで機会が欠けているのはなぜですか。 {#why-am-i-missing-some-opportunities-in-mpi}

MPIでオポチュニティが見つからない主な理由は次の2つです。

1. アトリビューション設定が「明示的」に設定されているが、オポチュニティに連絡先ロールが割り当てられていない
1. 期間コストはプログラムに含まれません

MPIは、すべてのオポチュニティが分析に含まれているかどうかを計算します。 そうでない場合は、より多くのオポチュニティを含めるためにアトリビューション設定（明示的、暗黙的、ハイブリッド）の変更を検討するよう求められます。

また、プログラムにプログラムコストがないためにオポチュニティが見つからない場合もあります。 警告が表示されますが、コストの不足しているプログラムは示されません。 プログラムの設定を確認してコストを含め、プログラムとオポチュニティがすべてMPIに含まれていることを確認してください。

## アクションダッシュボードにカスタムフィールド、オポチュニティタイプ、ABMフィルターが表示されないのはなぜですか。 {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

カスタムフィールド、オポチュニティタイプ、ABMフィルターは、すべてオポチュニティに関連する属性です。 「エンゲージメント」ダッシュボードを使用すると、エンゲージメントおよびリードの獲得を、オポチュニティに関連付けられているかどうかに関係なく測定できます。 エンゲージメントダッシュボードではオポチュニティが考慮されないので、「カスタムフィールド」、「オポチュニティタイプ」および「ABM」フィルターは適用されません。

## 標準のSalesforce Opportunity Amountフィールドではなく、売上高のレポートにカスタムのSalesforce Opportunityフィールドを使用したい。 MPIは私にそれを許可するのか？ {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

はい。 [マーケティング担当者サポート](http://docs.marketo.com/cdn-cgi/l/email-protection#b5c6c0c5c5dac7c1f5d8d4c7ded0c1da9bd6dad8) (Marketo Support)は、フィールドタイプが通貨である限り、マーケティング担当者の「Opportunity Amount」フィールドをカスタムのSalesforce Opportunityフィールドに再マップできます。 MPIは「Marketo Opportunity amount」フィールドを指すので、MPIは、再マッピングされたカスタムSalesforceフィールドのデータを使用できます。

>[!NOTE]
>
>再マッピング後、MPIはデータを今後表示します。 履歴金額は変更されません。

## オポチュニティを使用しない場合でもMPIを使用できますか。 {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPIは、ファネルの上部から売上高への影響まで、プログラムのパフォーマンスを測定できるように設計されています。 オポチュニティを使用しない場合でも、次のことが可能です。

* オーディエンス関与のための育成プログラムの表示パフォーマンス。
* リード獲得プログラムの表示パフォーマンス。
* プログラムタグを使用したマルチチャネルキャンペーンの表示パフォーマンス。
* 過去12か月間のオーディエンス関与の傾向を確認。
* PowerPointでパフォーマンスデータを保存およびエクスポートします。

## MPIでアカウント・ベースの戦略の成功を測定できますか。 {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

はい。 MPIは、 [Marketo ABMと統合され](http://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) 、ABMアカウントリストをMPIにシームレスに取り込みます。 「ABMアカウントリスト」フィルタを使用して、データをフィルタするABMリストを選択できます。

## MPIを購入するとすぐにアトリビューションが利用できますか。 {#is-attribution-instantly-available-when-i-purchase-mpi}

マーケティングアトリビューション機能は、MPIを購入したお客様が利用できます。 ただし、オポチュニティと [プログラムデータがMPIに正しくフローするように適切なセットアップ](http://docs.marketo.com/x/mRPG) が必要です。

## アトリビューションの設定に必要な作業 {#what-do-i-have-to-do-to-set-up-attribution}

1. 営業案件の設定

   1. オポチュニティがCRMと同期されていることを確認する
   1. アトリビューション設定が「明示的」に設定されている場合は、オポチュニティに関する連絡先の役割が表示されていることを確認します
   1. アトリビューション設定をハイブリッドに変更することをお勧めします
   1. プログラム設定

      1. プログラムにプログラムコストを含める
      1. 解析の動作を確認して、プログラムを解析に含めるかどうかを指定します
      1. チャネルの成功基準を設定する
      1. 人をプログラムに結び付ける

         1. ファーストタッチアトリビューションが機能するように、データベース内の各ユーザーに対して獲得プログラムと獲得日が設定されていることを確認します。
         1. プログラムがデータベース内のユーザーの成功状態を設定していることを確認します。

>[!TIP]
>
>必要なすべての設定手順について詳し [く説明します](http://docs.marketo.com/x/mRPG)。

## MPIとプログラム・アナライザの違いは何ですか？ {#whats-the-difference-between-mpi-and-the-program-analyzer}

プログラム・アナライザを使用すると、最大4つの測定でプログラムを比較できます。 MPIを使用すると、成功、新しいオポチュニティ作成など、選択した指標に対するチャネルとプログラムの貢献度を分析できます。 また、選択した1つの特定の指標に基づいて、12か月のチャネルトレンドを表示することもできます。

## MPIとアドバンスReport Builderの違いは何ですか。 {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

アドバンスReport Builder（RCEとも呼ばれます）は、通常、マーケティングオペレーションが行うセルフサービス（アドホック）レポート向けに設計されています。 MPIは、マーケティングリーダーやマーケターがパフォーマンスの分析にワンクリックでアクセスできるように設計されています。 最小限の設定が必要です。

## 貢献度の日付フィルターの「前年」オプションはどうなりましたか？ {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

「前年」の選択を一時的に解除しました。 「カスタム日付範囲」を選択して、年間のパフォーマンスデータを表示することもできます。
