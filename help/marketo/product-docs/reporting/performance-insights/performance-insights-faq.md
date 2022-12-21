---
unique-page-id: 12979858
description: パフォーマンスインサイトに関する FAQ — Marketo ドキュメント — 製品ドキュメント
title: パフォーマンスインサイトに関する FAQ
exl-id: cee791c3-1845-4fca-b803-c0dc1c644549
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1357'
ht-degree: 100%

---

# パフォーマンスインサイトに関する FAQ {#performance-insights-faq}

## 「エンゲージメント」タブの「成功」の定義は何ですか？ {#what-is-the-definition-of-success-in-the-engagement-tab}

成功は、Marketo での有意義なインタラクションの尺度です。プログラムの目的は、リードまたは見込み客との有意義なインタラクションを作成することです。成功は、その目標を達成したステータスに達したときにマークされます。オンラインセミナーへの参加、メールのリンククリック、web フォームの記入などです。成功は、プログラムチャネルによって異なります。

>[!NOTE]
>
>ウェビナープログラムには、招待、登録、出席のような複数のステータスがあります。「招待」や「登録」は、実際にウェビナーを見たわけではないので、意味のあるインタラクションではありません。この場合、「出席済み」は成功と見なされます。

## MPI は任意の CRM で動作しますか？ {#will-mpi-work-with-any-crm}

はい。技術的には、MPI はデータ同期用に CRM と直接やり取りしません。MPI では、Marketo AnalyticsData Warehouse に保存されたデータが利用されます。リード管理アプリケーションで CRM 同期がおこなわれるので、Marketo でサポートされているリード管理アプリケーションと統合された CRM では、データが正しく表示されます。ただし、CRM 商談フィールドを Marketo 商談フィールドに正しくマッピングする必要があります。

## 他のマーケティング分析製品（ARB、RCE、RCA、プログラム分析）を持っていません。MPI を使用できますか？ {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI は、リード管理アプリケーションへの独立したアドオンです。他の Analytics 製品を使用する必要はありません。

## RCA はプログラムのパフォーマンスデータも表示します。MPI と RCA に示されるデータに違いはありますか？ {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

いいえ。MPI は RCA と同じデータウェアハウスからデータをソースします。したがって、2 つの間のデータの違いは一切見られません。RCA を使用すると、すぐに独自のレポートを作成できます。MPI を使用すると、わかりやすいビジュアルダッシュボードにアクセスできます。

## MPI に一部のプログラム（オペレーショナルなど）を表示させたくありません。特定のプログラムの表示を制御するには、どうすればよいですか？ {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

プログラムの Analytics 動作を「オペレーショナル」に設定することで、プログラムの表示を制御できます。これにより、分析の計算からプログラムが除外されます。

>[!NOTE]
>
>分析動作の設定の詳細については[こちら](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/edit-analytics-behavior-settings.md)をご覧ください。

## 新しい製品ローンチ用にマルチチャネルキャンペーンを実行しています。すべての様々なチャネルにわたって、このキャンペーンのパフォーマンスを 1 か所で表示するにはどうすればよいですか？ {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

このようなキャンペーンの一部となるプログラムには、プログラムタグを利用することをお勧めします。プログラムタグは MPI に自動的に同期され、すべての MPI ダッシュボードでフィルタリングして、マルチチャネルキャンペーンのパフォーマンスを表示できます。

## RCA がない場合、属性設定にアクセスできますか？ {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

RCA を持っているかどうかに関係なく、MPI を持っている場合は、属性設定にアクセスできます。

## ログイン時に、属性設定が正しくないことを示す警告が MPI に表示されます。何が問題なのですか？ {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI は、すべての商談が分析に含まれているかどうかを計算します。含まれていない場合は、より多くの商談を含めるために、属性設定（明示的、暗黙的、ハイブリッド）の変更を検討するよう求められます。

また、プログラムのコストが見つからないため、商談が見つからない場合もあります。プログラムの Analytics の動作を確認してください。次のことが可能です。

1. デフォルト — デフォルトの動作は、1 つ以上の期間原価がある場合に MPI にのみ含まれます（0 ドルが割り当てられている場合も含む）。

1. 含む — このオプションは、期間原価を含めているかどうかに関係なく、MPI でプログラムを使用できるようにします。

1. [オペレーショナル](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#operational-programs)  — このオプションを選択すると、プログラムが MPI に表示されなくなります。

>[!NOTE]
>
>期間原価は、成功名と新しい名前のレポートをエンゲージメントダッシュボードで設定する&#x200B;**必要**&#x200B;があります。このダッシュボードでは、期間原価データを使用して、成功と新しい名前を集計します。期間原価が設定されていない場合、上記の Analytics の動作設定に関係なく、エンゲージメントダッシュボードは正しくレポートされません。

## MPI からいくつかの商談が欠落しているのはなぜですか？ {#why-am-i-missing-some-opportunities-in-mpi}

MPI で商談が欠落している主な理由は次の 2 つです。

1. 属性設定は「明示」に設定されているが、商談に連絡先の役割が割り当てられていない
1. 期間原価がプログラムに含まれていない

MPI は、すべての商談が分析に含まれているかどうかを計算します。含まれていない場合は、より多くの商談を含めるために、属性設定（明示的、暗黙的、ハイブリッド）の変更を検討するよう求められます。

また、プログラムのコストが見つからないため、商談が見つからない場合もあります。警告が表示されますが、どのプログラムにコストが足りないかは示されません。すべてのプログラムと商談が MPI に含まれていることを確認するには、コストを含むようにプログラムの設定を確認してください。

## エンゲージメントダッシュボードにカスタムフィールド、商談タイプ、ABM フィルターが表示されないのはなぜですか？ {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

カスタムフィールド、商談タイプ、ABM フィルタは、商談に関連するすべての属性です。エンゲージメントダッシュボードを使用すると、エンゲージメントとリード獲得を、商談に関連付けられているかどうかを測定できます。エンゲージメントダッシュボードでは商談を考慮していないので、カスタムフィールド、商談タイプ、ABM フィルターは適用されません。

## 売上高レポートに、標準の「Salesforce 商談額」フィールドではなく、カスタムの「Salesforce 商談」フィールドを使用したいのですが、可能ですか? {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

はい。[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)は、フィールドタイプが通貨である限り、Marketo の「商談額」フィールドをカスタムの「Salesforce 商談」フィールドに再マッピングできます。MPI は「Marketo 商談額」フィールドを参照するので、MPI は再マッピングされたカスタム Salesforce フィールドのデータを使用できます。

>[!NOTE]
>
>再マッピング後、MPI は今後のデータを表示します。履歴金額は変更されません。

## 商談を使用しない場合、MPI を引き続き使用できますか？ {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPI は、ファネルの上部から収益への影響まで、プログラムのパフォーマンスを測定できるように設計されています。商談を利用しない場合でも、次のことが可能です。

* オーディエンスエンゲージメントのための育成プログラムのパフォーマンスを表示する。
* リード獲得プログラムの実績を表示する。
* プログラムタグを使用して、マルチチャネルキャンペーンのパフォーマンスを表示する。
* 過去 12 か月間のオーディエンスエンゲージメントの傾向を確認する。
* PowerPoint でパフォーマンスデータを保存および書き出す。

## MPI ではアカウントベースの戦略の成功を測定できますか？ {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

はい。MPI では [Marketo TAM](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) ABM アカウントリストがシームレスに取り込まれます。「ABM アカウントリスト」フィルターを使用して、データをフィルターする目的の ABM リストを選択できます。

## MPI を購入すると、属性は即座に利用できますか？ {#is-attribution-instantly-available-when-i-purchase-mpi}

Marketo 属性機能は、MPI を購入した際に利用できます。ただし、商談とプログラムのデータが MPI に正しく流れるようにするためには、[適切な設定](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md)が必要です。

## 属性を設定するには、どうすればよいですか？ {#what-do-i-have-to-do-to-set-up-attribution}

1. 商談の設定

   1. 商談が CRM と同期されていることを確認します。
   1. 「属性」設定が「明示」に設定されている場合は、商談に関する連絡先の役割が必ず設定されるようにします
   1. 「属性」設定を「ハイブリッド」に変更することをお勧めします
   1. プログラムセットアップ

      1. プログラムにプログラムコストを含める
      1. 分析動作をレビューして、プログラムを分析に含める必要があるかどうかを示します
      1. あるすべてのチャネルの達成基準を設定します
      1. 担当者をプログラムに結び付ける

         1. ファーストタッチ属性を機能させるために、データベース内の各ユーザーに対して獲得プログラムと獲得日が設定されていることを確認します。
         1. プログラムで、データベース内のユーザーに対して成功状態が設定されていることを確認します

>[!TIP]
>
>必要なすべての設定手順について詳しくは、[この記事](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md)で説明されています。

## MPI とプログラムアナライザーの違いは何ですか？ {#whats-the-difference-between-mpi-and-the-program-analyzer}

プログラムアナライザーを使用すると、最大 4 つの測定をまたいでプログラムを比較できます。MPI を使用すると、成功、新規商談の作成など、選択した指標に対するチャネルおよびプログラムの貢献度を分析できます。また、選択した 1 つの特定の指標に基づいて、12 か月のチャネルトレンドを表示できます。

## MPI と Advanced Report Builder の違いは何ですか？ {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

Advanced Report Builder（RCE とも呼ばれます）は、セルフサービス（またはアドホック）レポート用に設計されています。通常は Marketing Operations がおこないます。MPI は、マーケティングリーダーとマーケターがパフォーマンス分析に 1 回のクリックでアクセスできるように設計されています。最小限の設定が必要です。

## 貢献度の日付フィルターの「前年」オプションはどうなりましたか？ {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

「前年」の選択を一時的に解除しました。「カスタムデータ範囲」選択を使用することで、引き続き、年全体のパフォーマンスデータ全体を表示するオプションがあります。
