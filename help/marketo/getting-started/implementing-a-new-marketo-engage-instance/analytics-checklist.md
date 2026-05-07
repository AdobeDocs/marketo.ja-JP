---
description: 新しいMarketo Engage インスタンスの「分析」セクションを設定します。
title: 新しいインスタンスのベストプラクティス - Analytics チェックリスト
feature: Getting Started
exl-id: ddbb9bc7-d06a-4a2e-a560-9d308630ae3f
source-git-commit: 240b78561db11e169188698880d4707a5c1f64de
workflow-type: tm+mt
source-wordcount: '1869'
ht-degree: 5%

---

# 新しいインスタンスのベストプラクティス：Analytics のチェックリスト {#new-instance-best-practices-analytics-checklist}

「分析」セクションでは、マーケティング施策のパフォーマンスを分析するグローバルレポートを提供します。 それらを操作するために必要な手順について説明します。

忘れずに[チェックリストをダウンロード](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx)し、進捗状況を追跡してください。

## 樹木 {#tree}

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
    <th></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>組織：命名、フォルダー、アーカイブ</td>
    <td><li>レポート命名規則を使用して、「グローバルレポート」タブでレポートを区別します。
    <ul><li>適切な命名規則の実践の例として、[ レポートタイプ ] [ グローバルとBU固有のタグ ] [ レポートの説明] [ メールパフォーマンス ]-[ グローバル ]-[ メールエンゲージメント 180日間]などがあります。</li></ul><br>
    <li>組織内のさまざまなユーザーグループ（営業部門、マーケティング部門など）と共有する必要があるレポートを特定し、Analytics for Global Reportsのグループレポートフォルダー内のフォルダーごとにレポートを整理します。</li>
    <li>アーカイブは、常に実行されるレポートなので、グローバルレポートフォルダーに限定する必要があります。   <ul><li>事業部構造に基づいてレポートを作成する場合は、関連する事業部の削減や追加などの組織変更にアーカイブを制限します。</li></ul>
    </td>
  </tr>
  <tr>
    <td>ワークスペース（該当する場合）</td>
    <td><li>ワークスペースをまたいでグローバルレポートとフォルダー構造を複製し、チームの一貫したレポートを維持します。 これらのレポートは、グループレポートフォルダーに保存されます。</li></td>
  </tr>
  <tr>
    <td>マイ レポート</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/creating-reports/understanding-my-reports-and-group-reports"> マイレポート </a> セクションで使用するために必要なレポートを特定して作成します。 このプライベートレポートセクションをグローバルレポートのサンドボックスとして使用します。 レポートを作成するユーザーのみが使用できます。</li>
    <li>組織の命名規則を使用してレポートと使用状況を特定し、マイレポートのレポートとグループレポートのレポートを照合できるようにします。</li></td>
  </tr>
  <tr>
    <td>グループレポート</td>
    <td><li>グループレポートは、組織のグローバルレポートであり、組織の全体的なアクティビティをレポートする必要があります。</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/clone-a-report-to-group-reports" target="_blank"> クローン可能なコアレポート </a>の作成を検討します。レポートを取得してデータの正確性を確保するために必要な時間を短縮するために、各事業部門が最も頻繁に使用する必要があります。 詳細については、以下の<a href="#global-reports"> グローバルレポートの表</a>を参照してください。
    <ul><li>ソース別、月別の個人パフォーマンスレポート（すべての時間および時間ベース）</li>
    <li>プログラムパフォーマンスレポート（コスト月別、時間ベース）</li>
    <li>メールパフォーマンスレポート（時間ベース）</li></ul>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/report-email-campaign-performance-across-workspaces" target="_blank"> レポートの「設定」タブで「グローバルレポート」 </a>をオンにして、すべてのワークスペースのデータをメールパフォーマンスレポートとメールリンクパフォーマンスレポートに含めます。 複数のワークスペースがある場合は、デフォルトのワークスペースでのみ有効にする必要があります。</li>
    <p><img src="assets/tip-icon.png" alt="メモアイコン"> ヒント：データベース セクションのほとんどのレポートに含めるフィルターを使用して、<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists" target="_blank"> スマートリスト </a>を作成します。 スマートリストの条件を更新する必要がある場合は、すべてのグローバルレポートで更新するのではなく、1か所で更新できます。</td>
  </tr>
</tbody>
</table>

## 購読 {#subscriptions}

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>購読</td>
    <td><li>レポート結果を確認する必要がある担当者と、その実施中の頻度について、マーケティングリーダーと連携します。</li> <li>サブスクリプションを使用すると、ユーザー指定ライセンスを使い果たすことなく、組織内の必要なユーザーにデータを配布できます。</li>
    <p><img src="assets/tip-icon.png" alt="メモアイコン"> ヒント：リアルタイムのレポートデータにアクセスする場合は、ユーザーとして追加して、レポートを表示できるようにする必要があります。
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/subscribe-to-a-basic-report">各チームの継続的な監視のために、希望する頻度（毎日/毎週/毎月）でサブスクリプション </a>を設定します。 また、<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/manage-report-subscriptions">Analyticsの「購読」タブで、すべての購読</a>を1か所で表示することもできます。</li></td>
  </tr>
</tbody>
</table>

## グローバルレポート {#global-reports}

組織内のさまざまなユーザーグループ（営業部門、マーケティングリーダーシップなど）と共有する必要があるレポートを特定します。 グループ/ユーザーグループ/事業部門ごとに適切なフォルダー構造を作成し、グループレポート内で複製されたレポートを整理します。 次のようなグローバルレポートの設定を検討します。

<table>
<thead>
  <tr>
    <th style="width:20%">レポートのタイプ</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>メールパフォーマンスレポート</td>
    <td><li>適切な電子メールを選択し、グローバル、Workspace、事業部門全体のレポートを作成します。</li>
    <li>クローン可能なすべてのプログラムテンプレートで、ローカルのメールパフォーマンスレポートを作成します。</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame">関連する期間</a>を使用（例：YTD、過去90日間） 標準メールのエンゲージメントと配信品質の指標を正確に把握することができます。</li>
    <p><img src="assets/tip-icon.png" alt="メモアイコン"> ヒント：<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/email-setup/filtering-email-bot-activity">管理者/電子メール </strong></a>で「ボットアクティビティ」フィルタリングをオンにしてログを回避するか、ボットアクティビティでログが有効になっているかどうかを特定します。 <strong>クローン可能なグローバルレポートのスマートリストで、「Is Bot Activity」制約が「False」に設定されている<a href="https://nation.marketo.com/t5/product-documents/filtering-email-bot-activity-feature-latest-release/ta-p/324860">開封済み/クリック済みアクティビティのみを許可するフィルターを含めます</a>。</td>
  </tr>
  <tr>
    <td>人物のパフォーマンスレポート</td>
    <td><img src="assets/note-icon.png" alt="メモアイコン"> 注：Marketo Engageの実装ごとに適切な<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags"> チャネルとタグ戦略</a>を設定してから、取得した人物やチャネル別のマーケティング投資のROIを追跡することをお勧めします。
    <p>
    <li>リード獲得プログラムのパフォーマンスを測定するための基準を決定し、次の指標にもとづいて時間ベース（今年、最後の12か月の表示、180日）の標準レポートを作成します。 <ul><li>取得プログラム：個人を取得するためにクレジットされるMarketo Engageプログラム。</li>
    <li>人物Source: レコードがデータベースに認識された方法のソースカテゴリ（CRM内の値のソースリストに基づく）
    </li></ul>
    <li>週または月ごとに作成されたユーザーを測定。 このレポートでは、データベースの増加率と、データベース・サイズの制限に近づいているかどうかを示す指標を提供します。</li>
    <li>スマート リストをカスタム列として使用して、<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report">人物パフォーマンスレポートの指標をフィルタリングします。</a></li>
    <p><img src="assets/tip-icon.png" alt="メモアイコン"> ヒント：マーケティングアクティビティではなくデータベースの人物パフォーマンスレポートに追加するカスタム列のスマートリストを作成して、レポートでスマートリスト名が選択されたときにスマートリスト名を適切かつ明確に確認できるようにします。</td>
  </tr>
  <tr>
    <td>プログラムパフォーマンスレポート</td>
    <td><p><img src="assets/note-icon.png" alt="メモアイコン"> メモ：このレポートでは、<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/tags/create-a-program-channel"><strong>管理者</strong> &gt; <strong> タグ </strong></a>でチャネル、進行ステータス、成功ステップが定義されている必要があります。
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report">選択プログラム内のマーケティング戦術の効果を測定</a>。</li>
    <li>マーケティングアクティビティ内のベストプラクティスに従って、プログラムメンバーシップを管理（スマートキャンペーンを使用して、獲得プログラム、ステータス、成功ステータスを更新）。</li>
    <li>当年と12か月間のコストにもとづいて測定します。
    <ul><li>プログラム パフォーマンス レポートを活用するには、<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program">期間費用</a>を維持することが重要です。</li></ul></li>
    <p>
    <img src="assets/tip-icon.png" alt="メモアイコン"> ヒント：プログラムパフォーマンスレポートで<a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people"> インポートしたリスト </a>を集計して表示するには、タグ付けに適した獲得プログラムをチームが選択していることを確認してください。 読み込んだリストがどのチャネルにも適用されない場合に、取得プログラムとして選択するデフォルトプログラム </a>の作成を<a href="https://experienceleague.adobe.com/ja/docs/marketo-learn/tutorials/programs-and-campaigns/default-programs/create-and-measure-default-programs">検討してください。 これにより、インポートされたユーザーが、空白の値ではなく、ソース、事業部、チャネルなどに関連する有効な取得プログラムを持っていることを確認できます。</td>
  </tr>
  <tr>
    <td>ランディングページ効果レポート</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report"> ランディングページパフォーマンスレポート </a>をグローバルレポートとして作成し、すべてのデザインスタジオ/マーケティングアクティビティランディングページの数値</a>を<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/filter-a-landing-page-performance-report"> フィルタリングして確認できるようにします。</li>
    <li>ランディングページを含むプログラムの場合は、プログラムテンプレート </a>内に専用のローカルレポートを作成して、プログラムレベルでパフォーマンスを確認できるようにすることを検討してください。<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report"></li></td>
  </tr>
  <tr>
    <td>Web ページアクティビティレポート</td>
    <td><img src="assets/note-icon.png" alt="メモアイコン"> メモ：このレポートでは、<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website">Munchkin JavaScript</a>が有効になっているweb ページ（外部およびMarketo ランディングページ）のみが追跡されます。 すべてのweb ページにコードがハードコーディングされないようにするために、<a href="https://developers.marketo.com/blog/integrating-munchkin-with-google-tag-manager/">Google Tag Manager</a>などのTag Management PlatformにJavaScript コードを配置することを検討してください。
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/web-page-activity-report">Web ページアクティビティレポート </a>をグローバルレポートとして作成して、すべてのweb ページの数値を1か所で確認できるようにします。 外部web ページのアクティビティは、Web ページアクティビティレポートにのみ反映されます。</li></td>
  </tr>
</tbody>
</table>

## ローカルレポート {#local-reports}

Marketo Engage レポートの中には、一般的に使用できるプログラムやアセットが限られているため、マーケティング活動の特定のプログラム内のローカルアセットとして最適なものもあります。 次のような基本的なレポートの設定を検討します。

<table>
<thead>
  <tr>
    <th style="width:20%">レポートのタイプ</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>メールリンク効果レポート</td>
    <td><li>メール送信プログラム内に<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report" target="_blank"> メールリンクパフォーマンスレポート </a>を作成し、ドリップキャンペーンを実施することで、メール送信でユーザーがクリックしたリンクに関するインサイトを得ることができます。</li></td>
  </tr>
  <tr>
    <td>キャンペーンアクティビティレポート</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank"> キャンペーンアクティビティレポート </a>を作成し、マーケティングアクティビティの運用フォルダー内で期間を選択します。</li>
    <li>ユースケースごとにトリガーをモニターし、<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/filter-a-campaign-activity-report" target="_blank"> キャンペーンフィルターを適用する</a> レポートを設定します（例：ビヘイビアースコアリングトリガー、ライフサイクルの選定トリガー、注目のアクションのトリガー）。</li></td>
  </tr>
  <tr>
    <td>エンゲージメントストリームパフォーマンスレポート（該当する場合）</td>
    <td><li>エンゲージメントプログラムにデプロイされたコンテンツとストリームの有効性を測定するために、<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/engagement-stream-performance-report" target="_blank"> エンゲージメントストリームパフォーマンスレポート </a>を作成します。</li>
    <li>レポートの「設定」タブ </a>で<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/group-email-reports-by-segmentations" target="_blank"> 「セグメント化」フィルターを使用し、エンゲージメントプログラムで使用されている<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation" target="_blank"> セグメント </a> （例：人物ソース、業界）でレポートデータをグループ化することを検討してください。 これにより、各セグメントのエンゲージメントパターンに関するより深いインサイトを得ることができ、エンゲージメントプログラム（コンテンツ、ストリーム、ストリームの頻度など）を改善するための戦略的な変更を行うことができます。</li></td>
  </tr>
</tbody>
</table>
