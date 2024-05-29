---
description: 新しいMarketo Engageインスタンスに Analytics セクションを設定します。
title: 新しいインスタンスのベストプラクティス - Analytics チェックリスト
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 6aeb894e6a36064825a25474c67f53a291f548ab
workflow-type: tm+mt
source-wordcount: '1615'
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
    <td><li>レポート命名規則を使用して、「グローバルレポート」タブでレポートを区別します。</li>
    <ul><li>命名規則に関する適切なプラクティスの例としては、[Report Type][Global vs. BU-Specific Tag][Report Description] があります。例えば、[Email Performance]-[Global]-[180 Days Email Engagement] などです。</li></ul><br>
    <li>組織内の様々なユーザーグループ（営業チーム、マーケティングリーダーなど）と共有する必要があるレポートを特定し、Analytics for Global Reports のグループレポートフォルダー内のフォルダー別にレポートを整理します。</li> 
    <li>グローバルレポートは常に表示されるレポートなので、アーカイブはグローバルレポートフォルダーに限定する必要があります。   <ul>
    <li>ビジネス・ユニット構造に基づいてレポートする場合は、関連するビジネス・ユニットの削減や追加など、組織の変更にアーカイブを制限します。</li>
    </ul></td>
  </tr>
  <tr>
    <td>ワークスペース（該当する場合）</td>
    <td><li>チームの一貫性のあるレポートを維持するために、ワークスペース間でグローバルレポートとフォルダー構造をレプリケートします。 これらのレポートは、グループ レポート フォルダーに格納されます。</li></td>
  </tr>
  <tr>
    <td>マイ レポート</td>
    <td><li>での使用に必要なレポートの特定と作成 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/creating-reports/understanding-my-reports-and-group-reports">マイレポート</a> セクション。 このプライベートレポートセクションは、グローバルレポートのサンドボックスとして使用します。 これらは、レポートを作成するユーザーのみが使用できます。</li>
    <li>組織の命名規則を使用してレポートと使用方法を特定し、マイレポートのレポートとグループレポートのレポートを紐付けることができます。</li></td>
  </tr>
  <tr>
    <td>グループレポート</td>
    <td><li>グループレポートは、組織のグローバルレポートであり、組織の全体的なアクティビティを報告する必要があります。</li>
    <li>の作成を検討 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/clone-a-report-to-group-reports" target="_blank">複製可能なコアレポート</a> レポートの取得に要する時間を短縮し、データの正確性を確保するために、各事業部門が最も頻繁に使用することを期待します。 詳細については、を参照してください。 <a href="#global-reports">以下のグローバルレポートテーブル</a>.
    <ul><li>人物パフォーマンスレポート（すべての時間および時間ベース）ソース別、月別</li>
    <li>プログラムパフォーマンスレポート（コスト月別、時間ベース）</li>
    <li>メールパフォーマンスレポート（時間ベース）</li></ul>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/report-email-campaign-performance-across-workspaces" target="_blank">「グローバルレポート」をオンにする</a> レポートの「設定」タブを使用して、電子メールのパフォーマンスおよび電子メールのリンクのパフォーマンス レポート内のすべてのワークスペースのデータを含めます。 複数のワークスペースがある場合は、デフォルトワークスペースでそのワークスペースを有効にするだけです。</li>
    <p><img src="assets/tip-icon.png" alt="メモアイコン"> ヒント： <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists" target="_blank">スマート・リスト</a> ほとんどのレポートの [ データベース ] セクションに含めるフィルターを指定します。 スマートリスト条件を更新する必要がある場合は、すべてのグローバルレポートで更新するのではなく、1 か所で更新できます。</td>
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
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/subscribe-to-a-basic-report">購読の設定</a> 各チームが継続的に監視するのに必要なサイクル（毎日/毎週/毎月）で行います。 以下の手順でも可能です <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/manage-report-subscriptions">購読をすべて表示</a> analytics の「購読」タブの下の 1 か所。</li></td>
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
    <td><li>適切なメールが選択された状態で、ワークスペース/ビジネスユニット全体にわたるグローバルレポートを作成します。</li>
    <li>すべての複製可能なプログラムテンプレートで、ローカルの電子メールパフォーマンスレポートを作成します。</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame">関連する期間を使用</a> （YTD、過去 90 日間など） レポートで、標準のメールエンゲージメントと配信品質指標の正確なビューを提供する。</li>
    <p><img src="assets/tip-icon.png" alt="メモアイコン"> ヒント： <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/email-setup/filtering-email-bot-activity">で「ボットアクティビティ」フィルタリングを有効にする <strong>管理者/ メール</strong></a> ログに記録されないようにするか、ボットアクティビティのログが有効かどうかを識別します。 許可するフィルターのみを含める <a href="https://nation.marketo.com/t5/product-documents/filtering-email-bot-activity-feature-latest-release/ta-p/324860">「ボットアクティビティである」が「False」に設定された状態でアクティビティを開く/クリックする</a> 複製可能なグローバルレポートのスマートリスト内にあります。</td>
  </tr>
  <tr>
    <td>人物の効果レポート</td>
    <td><img src="assets/note-icon.png" alt="メモアイコン"> メモ：を正しく設定することをお勧めします。 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags">チャネルとタグ戦略</a> すべてのMarketo Engage導入について、獲得した人物とマーケティング投資の ROI をチャネル別にトラッキングできます。
    <p>
    <li>リード獲得プログラムのパフォーマンスを測定するために使用する条件を決定し、次の指標に基づいて時間ベース（現在の年、過去 12 か月単位のビュー、または 180 日間）の標準レポートを作成します。</li> <ul><li>獲得プログラム：人物を獲得するためにクレジットされるMarketo Engageプログラム。</li>
    <li>人物ソース：レコードがデータベースに認識されるきっかけとなったソースカテゴリ（CRM の値のソースリストに基づく）
    </li></ul>
    <li>週または月ごとに作成されたユーザーを測定します。 このレポートは、データベースの増加率の測定値と、データベースのサイズ制限に近づいているかどうかを示します。</li>
    <li>人物パフォーマンスレポートの指標のフィルタリング基準 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report">スマート・リストをカスタム列として使用します。</a></li>
    <p><img src="assets/tip-icon.png" alt="メモアイコン"> ヒント：マーケティングアクティビティではなく、データベースの人物パフォーマンスレポートに追加するカスタム列のスマートリストを作成して、レポートでスマートリスト名が選択されたときにわかりやすく表示できるようにします。</td>
  </tr>
  <tr>
    <td>プログラム効果レポート</td>
    <td><p><img src="assets/note-icon.png" alt="メモアイコン"> 注意：このレポートを作成するには、チャネル、進捗ステータスおよび成功ステップがで定義されている必要があります。 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/tags/create-a-program-channel"><strong>Admin</strong> &gt; <strong>タグ</strong></a>.
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report">マーケティング戦術の有効性の測定</a> 選択的なプログラム内。</li>
    <li>マーケティングアクティビティ内のベストプラクティスに従って、プログラムメンバーシップを管理します（スマートキャンペーンを使用して、獲得プログラム、ステータス、成功ステータスを更新します）。</li>
    <li>今年のコストと 12 か月周期に基づいて測定します。
    <ul><li>次を維持することを忘れないでください <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program">期間コスト</a> は、プログラムパフォーマンスレポートを活用するうえで非常に重要です。</li></ul>
    <br>
    <br><img src="assets/tip-icon.png" alt="メモアイコン"> ヒント：いずれかを集約して表示するには <a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people">インポートしたリスト</a> プログラムパフォーマンスレポートで、チームがタグ付けに適した獲得プログラムを選択していることを確認します。 考慮 <a href="https://experienceleague.adobe.com/ja/docs/marketo-learn/tutorials/programs-and-campaigns/default-programs/create-and-measure-default-programs">デフォルトプログラムの作成</a> 読み込まれたリストがどのチャネルにも適用されない場合に、獲得プログラムとして選択するリスト。 これにより、読み込んだユーザーが、空白の値ではなく、ソース、ビジネスユニット、チャネルなどに関連する有効な獲得プログラムを持つようになります。</td>
  </tr>
  <tr>
    <td>ランディングページ効果レポート</td>
    <td><li>を作成 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">ランディングページのパフォーマンスレポート</a> グローバルレポートとしての機能 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/filter-a-landing-page-performance-report">数値のフィルタリングとレビュー</a> すべての Design Studio/マーケティングアクティビティのランディングページを 1 か所にまとめることができます。</li>
    <li>ランディングページを持つプログラムの場合は、 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">プログラムテンプレート内での専用のローカルレポートの作成</a> そのため、プログラムレベルでパフォーマンスを確認できます。</li></td>
  </tr>
  <tr>
    <td>Web ページアクティビティレポート</td>
    <td><img src="assets/note-icon.png" alt="メモアイコン"> メモ：次の条件を満たす Web ページ（外部ランディングページとMarketo ランディングページ）のみ <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website">Munchkin JavaScript</a> 有効はこの報告書で追跡されます。 次のような JavaScript コードをTag Management Platform に配置することを検討してください <a href="https://developers.marketo.com/blog/integrating-munchkin-with-google-tag-manager/">Google Tag Manager</a>（すべての web ページでコードがハードコーディングされるのを回避するため）。
    <p>
    <li>を作成 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/web-page-activity-report">Web ページアクティビティレポート</a> グローバルレポートとして機能するので、すべての web ページの数を 1 か所で確認できます。 外部 web ページのアクティビティは、web ページのアクティビティレポートにのみ反映されます。</li></td>
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
    <td><li>を作成 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report" target="_blank">メールリンクのパフォーマンスレポート</a> メールを送信するプログラムやドリップキャンペーン内で、メール送信でユーザーがクリックしたリンクに関するインサイトを提供します。</li></td>
  </tr>
  <tr>
    <td>キャンペーンアクティビティレポート</td>
    <td><li>を作成 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank">キャンペーン活動レポート</a> マーケティングアクティビティで、運用フォルダー内の期間を選択します。</li>
    <li>各ユースケースのトリガーを監視するレポートの設定 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/filter-a-campaign-activity-report" target="_blank">キャンペーンフィルターの適用</a> （例：行動スコアリングトリガー、ライフサイクル選定トリガー、注目のモーメントトリガー）。</li></td>
  </tr>
  <tr>
    <td>エンゲージメントストリームのパフォーマンスレポート（該当する場合）</td>
    <td><li>を作成 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/engagement-stream-performance-report" target="_blank">エンゲージメントストリームのパフォーマンスレポート</a> お客様のエンゲージメントプログラム内にデプロイされたコンテンツとストリームの有効性を測定するため。</li>
    <li>の使用を検討してください。 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/group-email-reports-by-segmentations" target="_blank">レポートの「設定」タブの「セグメント化」フィルター</a> および次を使用したレポートデータのグループ化 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation" target="_blank">セグメント</a> エンゲージメントプログラムで使用される（担当者、業界など）。 これにより、各セグメントのエンゲージメントパターンに関する深いインサイトを得ることができ、エンゲージメントプログラム（コンテンツ、ストリーム、ストリームケイデンスなど）を改善するための戦略的な変更を行うことができるようになります。</li></td>
  </tr>
</tbody>
</table>

作業中の箇条書きを含むテーブル

<table>
<tbody>
<tr>
    <td>グループレポート</td>
    <td><img src="assets/note-icon.png" alt="メモアイコン"> 注：テキスト。
    <p>
    <li>テキスト。</li>
    <li>テキスト。
    <ul><li>テキスト</li>
    <li>テキスト</li></ul>
    <li>テキスト。</li>
    <li>テキスト。</li>
    <p><img src="assets/tip-icon.png" alt="メモアイコン"> ヒント：テキスト。</td>
  </tr>
  </tbody>
</table>

テスト修正 1

<table>
<tbody>
<tr>
    <td>人物の効果レポート</td>
    <td><img src="assets/note-icon.png" alt="メモアイコン"> メモ：を正しく設定することをお勧めします。 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags">チャネルとタグ戦略</a> すべてのMarketo Engage導入について、獲得した人物とマーケティング投資の ROI をチャネル別にトラッキングできます。
    <p>
    <li>リード獲得プログラムのパフォーマンスを測定するために使用する条件を決定し、次の指標に基づいて時間ベース（現在の年、過去 12 か月単位のビュー、または 180 日間）の標準レポートを作成します。</li>
    <ul><li>獲得プログラム：個人を獲得するためにクレジットされるMarketo Engageプログラム</li>
    <li>人物ソース：レコードがデータベースに認識されるきっかけとなったソースカテゴリ（CRM の値のソースリストに基づく）</li></ul>
    <li>週または月ごとに作成されたユーザーを測定します。 このレポートは、データベースの増加率の測定値と、データベースのサイズ制限に近づいているかどうかを示します。</li>
    <li>人物パフォーマンスレポートの指標のフィルタリング基準 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report">スマート・リストをカスタム列として使用します。</a></li>
    <p><img src="assets/tip-icon.png" alt="メモアイコン"> ヒント：マーケティングアクティビティではなく、データベースの人物パフォーマンスレポートに追加するカスタム列のスマートリストを作成して、レポートでスマートリスト名が選択されたときにわかりやすく表示できるようにします。</td>
  </tr>
  </tbody>
</table>
