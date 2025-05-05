---
description: 新しいMarketo Engageインスタンスに Analytics セクションを設定します。
title: 新しいインスタンスのベストプラクティス - Analytics チェックリスト
feature: Getting Started
exl-id: ddbb9bc7-d06a-4a2e-a560-9d308630ae3f
source-git-commit: 7a847ece020ea0c0001241abf8e49b9eadf8edce
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 5%

---

# 新しいインスタンスのベストプラクティス：Analytics のチェックリスト {#new-instance-best-practices-analytics-checklist}

「分析」セクションには、マーケティング活動のパフォーマンスを分析するグローバルレポートが表示されます。 これらを移動するために必要な手順について説明します。

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
    <ul><li>命名規則に関する適切なプラクティスの例としては、[Report Type][Global vs. BU-Specific Tag][Report Description] があります。例えば、[Email Performance]-[Global]-[180 Days Email Engagement] などです。</li></ul><br>
    <li>組織内の様々なユーザーグループ（営業チーム、マーケティングリーダーなど）と共有する必要があるレポートを特定し、Analytics for Global Reports のグループレポートフォルダー内のフォルダー別にレポートを整理します。</li> 
    <li>グローバルレポートは常に表示されるレポートなので、アーカイブはグローバルレポートフォルダーに限定する必要があります。   <ul><li>ビジネス・ユニット構造に基づいてレポートする場合は、関連するビジネス・ユニットの削減や追加など、組織の変更にアーカイブを制限します。</li></ul>
    </td>
  </tr>
  <tr>
    <td>ワークスペース（該当する場合）</td>
    <td><li>チームの一貫性のあるレポートを維持するために、ワークスペース間でグローバルレポートとフォルダー構造をレプリケートします。 これらのレポートは、グループ レポート フォルダーに格納されます。</li></td>
  </tr>
  <tr>
    <td>マイ レポート</td>
    <td><li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/reporting/basic-reporting/creating-reports/understanding-my-reports-and-group-reports"> マイレポート </a> セクションで使用するために必要なレポートを特定および作成します。 このプライベートレポートセクションは、グローバルレポートのサンドボックスとして使用します。 これらは、レポートを作成するユーザーのみが使用できます。</li>
    <li>組織の命名規則を使用してレポートと使用方法を特定し、マイレポートのレポートとグループレポートのレポートを紐付けることができます。</li></td>
  </tr>
  <tr>
    <td>グループレポート</td>
    <td><li>グループレポートは、組織のグローバルレポートであり、組織の全体的なアクティビティを報告する必要があります。</li>
    <li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/clone-a-report-to-group-reports" target="_blank"> 複製可能なコアレポート </a> の作成を検討してください。各ビジネスユニットは、レポートの取得に必要な時間を短縮し、データの正確性を確保するために、最も頻繁に使用されると予想されます。 詳しくは、以下の <a href="#global-reports"> グローバルレポートの表 </a> を参照してください。
    <ul><li>人物パフォーマンスレポート（すべての時間および時間ベース）ソース別、月別</li>
    <li>プログラムパフォーマンスレポート（コスト月別、時間ベース）</li>
    <li>メールパフォーマンスレポート（時間ベース）</li></ul>
    <li>レポートの「設定」タブで <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/report-email-campaign-performance-across-workspaces" target="_blank"> 「グローバルレポート」をオンに </a> ると、メールのパフォーマンスおよびメールのリンクのパフォーマンスレポートのすべてのワークスペースのデータが含まれます。 複数のワークスペースがある場合は、デフォルトワークスペースでそのワークスペースを有効にするだけです。</li>
    <p><img src="assets/tip-icon.png" alt="メモアイコン"> ヒント：「データベース」セクションのほとんどのレポートに含めるフィルタを使用して、<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists" target="_blank"> スマート・リスト </a> を作成します。 スマートリスト条件を更新する必要がある場合は、すべてのグローバルレポートで更新するのではなく、1 か所で更新できます。</td>
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
    <td><li>実装時にレポート結果とケイデンスをレビューする必要がある人物に関して、マーケティングリーダーと連携します。</li> <li>サブスクリプションを使用すると、指定されたユーザーライセンスを使い果たすことなく、組織内の知る必要のあるユーザーにデータを配信できます。</li>
    <p><img src="assets/tip-icon.png" alt="メモアイコン"> ヒント：ユーザーにリアルタイムレポートデータへのアクセスを許可する場合は、ユーザーとして追加して、レポートを表示できるようにする必要があります。
    <p>
    <li>各チームの継続的な監視に適した頻度（毎日/毎週/毎月）で <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/subscribe-to-a-basic-report"> サブスクリプションを設定 </a> します。 また、Analytics の「購読 <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/manage-report-subscriptions"> タブの下で、1 か所ですべての購読を表示 </a> することもできます。</li></td>
  </tr>
</tbody>
</table>

## グローバルレポート {#global-reports}

組織内の様々なユーザーグループ（セールスチーム、マーケティングリーダーシップなど）と共有する必要があるレポートを特定します。 各チーム/ユーザーグループ/ビジネスユニットに対して適切なフォルダー構造を作成し、グループレポート内でクローンレポートを整理します。 次のようなグローバルレポートの設定を検討します。

<table>
<thead>
  <tr>
    <th style="width:20%">レポートのタイプ</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>メールの効果レポート</td>
    <td><li>適切なメールを選択した、グローバルなWorkspace/ビジネスユニット全体のレポートを作成します。</li>
    <li>すべての複製可能なプログラムテンプレートで、ローカルの電子メールパフォーマンスレポートを作成します。</li>
    <li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame"> 関連する期間を使用 </a> （YTD、過去 90 日間など） レポートで、標準のメールエンゲージメントと配信品質指標の正確なビューを提供する。</li>
    <p><img src="assets/tip-icon.png" alt="メモアイコン"> ヒント：<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/email-setup/filtering-email-bot-activity"> 管理者/メール <strong> で「ボットアクティビティ」フィルタリングをオンにしてログに記録しないようにするか </strong></a> ボットアクティビティのログが有効になっているかどうかを確認します。 複製可能なグローバルレポートのスマートリストで、「ボットアクティビティである」が「False」に設定されている <a href="https://nation.marketo.com/t5/product-documents/filtering-email-bot-activity-feature-latest-release/ta-p/324860"> 開かれた/クリックされたアクティビティ </a> のみを許可するフィルターを含めます。</td>
  </tr>
  <tr>
    <td>人物の効果レポート</td>
    <td><img src="assets/note-icon.png" alt="メモアイコン"> メモ：獲得した人材を追跡し、チャネル別にマーケティング投資の ROI を追跡する前に、Marketo Engageの導入ごとに適切な <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags"> チャネルとタグの戦略 </a> を立てることをお勧めします。
    <p>
    <li>リード獲得プログラムのパフォーマンスを測定するために使用する条件を決定し、次の指標に基づいて時間ベース（現在の年、過去 12 か月単位のビュー、または 180 日間）の標準レポートを作成します。 <ul><li>獲得プログラム：人物を獲得するためにクレジットされるMarketo Engageプログラム。</li>
    <li>人物Source: レコードがデータベースに認識されるきっかけとなったソースカテゴリ（CRM の値のソースリストに基づく）
    </li></ul>
    <li>週または月ごとに作成されたユーザーを測定します。 このレポートは、データベースの増加率の測定値と、データベースのサイズ制限に近づいているかどうかを示します。</li>
    <li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report"> スマート・リストをカスタム列として使用 </a> して、個人情報パフォーマンス・レポートの指標をフィルタ処理します。</li>
    <p><img src="assets/tip-icon.png" alt="メモアイコン"> ヒント：マーケティングアクティビティではなく、データベースの人物パフォーマンスレポートに追加するカスタム列のスマートリストを作成して、レポートでスマートリスト名が選択されたときにわかりやすく表示できるようにします。</td>
  </tr>
  <tr>
    <td>プログラム効果レポート</td>
    <td><p><img src="assets/note-icon.png" alt="メモアイコン"> メモ：このレポートを使用するには、<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/tags/create-a-program-channel"><strong> 管理者 </strong>/<strong> タグ </strong></a> でチャネル、進捗ステータスおよび成功ステップを定義している必要があります。
    <p>
    <li>選択したプログラム内で <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report"> マーケティング戦術の有効性を測定 </a> します。</li>
    <li>マーケティングアクティビティ内のベストプラクティスに従って、プログラムメンバーシップを管理します（スマートキャンペーンを使用して、獲得プログラム、ステータス、成功ステータスを更新します）。</li>
    <li>今年のコストと 12 か月周期に基づいて測定します。
    <ul><li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program"> 期間コスト </a> の維持は、プログラムパフォーマンスレポートを活用するうえで重要であることに注意してください。</li></ul></li>
    <p>
    <img src="assets/tip-icon.png" alt="メモアイコン"> ヒント：プログラムのパフォーマンスレポートで <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people"> インポートされたリスト </a> を集計および表示するには、チームがタグ付けに適した獲得プログラムを選択していることを確認します。 読み込まれたリストがどのチャネルにも適用されない場合は、獲得プログラムとして選択する <a href="https://experienceleague.adobe.com/ja/docs/marketo-learn/tutorials/programs-and-campaigns/default-programs/create-and-measure-default-programs"> デフォルトプログラムの作成 </a> を検討してください。 これにより、読み込んだユーザーが、空白の値ではなく、ソース、ビジネスユニット、チャネルなどに関連する有効な獲得プログラムを持つようになります。</td>
  </tr>
  <tr>
    <td>ランディングページ効果レポート</td>
    <td><li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report"> ランディングページパフォーマンスレポート </a> をグローバルレポートとして作成すると、すべての Design Studio/Marketing Activities ランディングページの <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/filter-a-landing-page-performance-report"> 数値のフィルタリングとレビュー </a> を 1 か所で行うことができます。</li>
    <li>ランディングページを使用するプログラムの場合は、プログラムレベルでパフォーマンスを確認できるように、<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report"> プログラムテンプレート内で専用のローカルレポートを作成する </a> を検討してください。</li></td>
  </tr>
  <tr>
    <td>Web ページアクティビティレポート</td>
    <td><img src="assets/note-icon.png" alt="メモアイコン"> メモ：このレポートでは、（Munchkin JavaScript<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website"> が有効になっている web ページ（外部およびMarketo ランディングページ </a> のみが追跡されます。 すべての web ページにコードをハードコーディングするのを避けるために、<a href="https://developers.marketo.com/blog/integrating-munchkin-with-google-tag-manager/">Google Tag Manager</a> などのJavaScript コードをTag Management Platform に配置することを検討してください。
    <p>
    <li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/web-page-activity-report">Web ページアクティビティレポート </a> をグローバルレポートとして作成すると、すべての Web ページの数を 1 か所で確認できます。 外部 web ページのアクティビティは、web ページのアクティビティレポートにのみ反映されます。</li></td>
  </tr>
</tbody>
</table>

## ローカルレポート {#local-reports}

一部のMarketo Engageレポートは、より限られたプログラムとアセットのセットで使用するのが一般的なので、マーケティングアクティビティの特定のプログラム内にローカルアセットとしてデプロイするのが最適です。 次のような基本的なレポートの設定を検討します。

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
    <td><li>メールとドリップキャンペーンを送信するプログラム内に <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report" target="_blank"> メールリンクのパフォーマンスレポート </a> を作成して、ユーザーがメールでクリックしたリンクに関するインサイトを提供します。</li></td>
  </tr>
  <tr>
    <td>キャンペーンアクティビティレポート</td>
    <td><li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank"> キャンペーンアクティビティレポート </a> を作成し、マーケティングアクティビティで運用フォルダー内の期間を選択します。</li>
    <li>各ユースケースのトリガーをモニタリングするレポートを設定し、<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/filter-a-campaign-activity-report" target="_blank"> キャンペーンフィルターを適用 </a> できます（行動スコアリングトリガー、ライフサイクルの選定トリガー、注目のモーメントのトリガーなど）。</li></td>
  </tr>
  <tr>
    <td>エンゲージメントストリームのパフォーマンスレポート（該当する場合）</td>
    <td><li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/engagement-stream-performance-report" target="_blank"> エンゲージメントストリームパフォーマンスレポート </a> を作成して、エンゲージメントプログラム内にデプロイされたコンテンツとストリームの効果を測定します。</li>
    <li>レポートの「設定」タブで <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/group-email-reports-by-segmentations" target="_blank"> 「セグメント化」フィルターを使用し </a> エンゲージメントプログラムで使用する <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation" target="_blank"> セグメント </a> （個人ソース、業界など）でレポートデータをグループ化することを検討します。 これにより、各セグメントのエンゲージメントパターンに関する深いインサイトを得ることができ、エンゲージメントプログラム（コンテンツ、ストリーム、ストリームケイデンスなど）を改善するための戦略的な変更を行うことができるようになります。</li></td>
  </tr>
</tbody>
</table>
