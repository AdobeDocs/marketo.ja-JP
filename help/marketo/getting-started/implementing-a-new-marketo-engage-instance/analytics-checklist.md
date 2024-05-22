---
description: 新しいエリア分析 – Marketo ドキュメント – 製品ドキュメント
title: 新しいインスタンスのベストプラクティス - Analytics チェックリスト
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: ae40e26966ed85da9c55fc510732841fa1e5212a
workflow-type: tm+mt
source-wordcount: '1419'
ht-degree: 3%

---

# 新しい領域：Analytics チェックリスト {#new-area-analytics-checklist}

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
    <td>組織：命名、フォルダー、アーカイブ <br> </td>
    <td>レポート命名規則を使用して、「グローバルレポート」タブでレポートを区別します。 <br>命名規則に関する適切なプラクティスの例としては、[Report Type][Global vs. BU-Specific Tag][Report Description] があります。例えば、[Email Performance]-[Global]-[180 Days Email Engagement] などです。  <br>組織内の様々なユーザーグループ（営業チーム、マーケティングリーダーなど）と共有する必要があるレポートを特定し、Analytics for Global Reports のグループレポートフォルダー内のフォルダー別にレポートを整理します。 <br>グローバルレポートは常に表示されるレポートなので、アーカイブはグローバルレポートフォルダーに限定する必要があります。   <br>ビジネス・ユニット構造に基づいてレポートする場合は、関連するビジネス・ユニットの削減や追加など、組織の変更にアーカイブを制限します。</td>
  </tr>
  <tr>
    <td>ワークスペース（該当する場合） </td>
    <td>ワークスペースを使用している場合は、ワークスペース間でグローバルレポートおよびフォルダー構造をレプリケートして、チームの一貫性のあるレポートを維持します。 これらのレポートは、Group Reports フォルダーに格納されます。</td>
  </tr>
  <tr>
    <td>マイ レポート </td>
    <td>での使用に必要なレポートを特定し、作成する <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/creating-reports/understanding-my-reports-and-group-reports">マイレポート</a> セクション。 このプライベートレポートセクションは、グローバルレポートのサンドボックスとして使用します。 これらは、レポートを作成するユーザーのみが使用できます。   <br>組織の命名規則を使用してレポートと使用方法を特定し、マイレポートのレポートとグループレポートのレポートを紐付けることができます。</td>
  </tr>
  <tr>
    <td>グループレポート </td>
    <td>グループレポートは、組織のグローバルレポートであり、Marketo Engage組織の全体的なアクティビティを報告する必要があります。   <br>の作成を検討 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/clone-a-report-to-group-reports" target="_blank" rel="noopener noreferrer">複製可能なコアレポート</a> レポートの取得に要する時間を短縮し、データの正確性を確保するために、各事業部門が最大限に活用することを期待します。 「基本レポート – グローバルレポート」テーブルの詳細を参照してください [ ブックマークされたセクションへのリンクを挿入 ]。 <br>人物パフォーマンスレポート（すべての時間および時間ベース） – ソース別、月別 <br>プログラムパフォーマンスレポート（コスト月別、時間ベース） <br>メールパフォーマンスレポート（時間ベース） <br><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/report-email-campaign-performance-across-workspaces" target="_blank" rel="noopener noreferrer">「グローバルレポート」をオンにします。</a> レポートの「設定」タブを使用して、電子メールのパフォーマンスおよび電子メールのリンクのパフォーマンス レポート内のすべてのワークスペースのデータを含めます。 複数のワークスペースがある場合は、デフォルトのワークスペースでこれを有効にするだけです。  <br>ヒント： <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists" target="_blank" rel="noopener noreferrer">スマート・リスト</a> ほとんどのレポートの「データベース」セクションに含めるフィルターを使用します。 スマートリスト条件を更新する必要がある場合は、すべてのグローバルレポートで更新するのではなく、1 か所で更新できます。</td>
  </tr>
</tbody>
</table>

## 購読 {#subscriptions}

<table>
<thead>
  <tr>
    <th>エリア </th>
    <th>アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>購読 </td>
    <td>実装時にレポート結果とケイデンスをレビューする必要がある人物に関して、マーケティングリーダーと連携します。 <br>サブスクリプションを使用すると、指定されたユーザーライセンスを使い果たすことなく、組織内の知る必要のあるユーザーにデータを配信できます。 <br>ヒント：購読メールは通常、夜間に送信されます。 ユーザーにリアルタイムレポートデータへのアクセスを許可する場合は、ユーザーをユーザーとして追加し、レポートを直接確認できるようにする必要があります。 <br><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/subscribe-to-a-basic-report">購読の設定</a> 各チームが継続的に監視する場合の望ましい頻度（毎日/毎週/毎月）に応じて調整します。 以下の手順でも可能です <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/manage-report-subscriptions">購読をすべて表示</a> analytics の「購読」タブの下の 1 か所。</td>
  </tr>
</tbody>
</table>

## グローバルレポート {#global-reports}

組織内の様々なユーザーグループ（セールスチーム、マーケティングリーダーシップなど）と共有する必要があるレポートを特定します。 各チーム/ユーザーグループ/ビジネスユニットに対して適切なフォルダー構造を作成し、レポートのクローン作成時にグループレポート内でレポートを整理します。 次のようなグローバルレポートの設定を検討します。

<table>
<thead>
  <tr>
    <th style="width:20%">レポートのタイプ</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>メールの効果レポート </td>
    <td>適切なメールが選択された状態で、ワークスペース/ビジネスユニット全体にわたるグローバルレポートを作成します。  <br>すべての複製可能なプログラムテンプレートで、ローカルの電子メールパフォーマンスレポートを作成します。 <br><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame">関連する期間を使用</a> このレポートで（年、過去 180 日間、過去 90 日間）標準のメールエンゲージメントと配信品質指標の正確なビューを提供します。 <br>ヒント： <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/email-setup/filtering-email-bot-activity">「管理者/電子メール」で「ボットアクティビティ」フィルタリングを有効にする</a> ログに記録されないようにしたり、ボットアクティビティのログが有効かどうかを識別したりします。 <a href="https://nation.marketo.com/t5/product-documents/filtering-email-bot-activity-feature-latest-release/ta-p/324860">「ボットアクティビティである」が「False」に設定されている場合に開封/ クリックされたアクティビティのみを許可するフィルターを含める</a> 複製可能なグローバルレポートのスマートリスト内にあります。</td>
  </tr>
  <tr>
    <td>人物の効果レポート</td>
    <td>メモ：を正しく設定することをお勧めします。 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags">チャネルとタグ戦略</a> すべてのMarketo Engage導入について、各チャネルを通じて獲得した人材とマーケティング投資の ROI をトラッキングできます。 <br>リード獲得プログラムのパフォーマンスを測定するために使用する条件を決定し、次の指標に基づいて時間ベース（現在の年、過去 12 か月単位のビュー、または 180 日間）の標準レポートを作成します。 <br>獲得プログラム：リードを獲得したクレジットが付与されるMarketo Engageプログラム。  <br>人物ソース：レコードがデータベースに認識されるきっかけとなったソースカテゴリ（CRM の値のソースリストに基づく） <br>週または月ごとに作成されたユーザーを測定します。 このレポートは、データベースの増加率の測定値と、データベース サイズの上限に近づいているか、まもなく超えるかを示します。 <br>人物パフォーマンスレポートの指標のフィルタリング基準 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report">スマート・リストをカスタム列として使用します。</a>  <br>ヒント：データベースの人物パフォーマンスレポートに「マーケティングアクティビティ」ではなく追加するカスタム列のスマートリストを作成して、レポートで選択したスマートリスト名を適切かつ明確に確認できます。</td>
  </tr>
  <tr>
    <td>プログラム効果レポート</td>
    <td>注意：このレポートを作成するには、 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/tags/create-a-program-channel">管理者/ タグ エリア</a>. <br><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report">マーケティング戦術の有効性の測定</a> 選択的なプログラム内。 <br>マーケティングアクティビティ内のベストプラクティスに従って、プログラムメンバーシップを管理します（スマートキャンペーンを使用して、獲得プログラム、ステータス、成功ステータスを更新します）。  <br>今年のコストと 12 か月周期のコストに基づいて測定します。  <br>次を維持することを忘れないでください <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program">期間コスト</a> は、プログラムパフォーマンスレポートを活用するうえで非常に重要です。 <br>ヒント：いずれかを集約して表示するには <a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people">インポートしたリスト</a> プログラムパフォーマンスレポートで、チームがタグ付けに適切な獲得プログラムを選択していることを確認します。 考慮 <a href="https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/programs-and-campaigns/default-programs/create-and-measure-default-programs">デフォルトプログラムの作成</a> 読み込まれたリストがどのチャネルにも適用されない場合に、獲得プログラムとして選択するリスト。 これにより、読み込んだユーザーはソース、ビジネスユニット、チャネルなどに関連する有効な獲得プログラムを確実に保持できます。 空白の値の代わりに使用します。</td>
  </tr>
  <tr>
    <td>ランディングページ効果レポート</td>
    <td> を作成 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">ランディングページのパフォーマンスレポート</a> グローバルレポートとしての機能 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/filter-a-landing-page-performance-report">数値のフィルタリングとレビュー</a> すべての Design Studio ランディングページまたはマーケティングアクティビティのランディングページが 1 か所にまとめられています。 <br>ランディングページを使用するプログラムの場合は、 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">プログラムテンプレート内での専用のローカルレポートの作成</a> そのため、プログラムレベルでパフォーマンスを確認できます。</td>
  </tr>
  <tr>
    <td>Web ページアクティビティレポート </td>
    <td>メモ：次の条件を満たす Web ページ（外部ランディングページとMarketo ランディングページ）のみ <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website">Munchkin JavaScript</a> 有効はこの報告書で追跡されます。 次のような JavaScript コードをTag Management Platform に配置することを検討してください <a href="https://developers.marketo.com/blog/integrating-munchkin-with-google-tag-manager/">Google Tag Manager</a>を使用して、すべての web ページでコードがハードコーディングされるのを回避できます。  <br>を作成 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/web-page-activity-report">Web ページアクティビティレポート</a> グローバルレポートとして機能するので、すべての web ページの数を 1 か所で確認できます。 外部 web ページのアクティビティは、web ページのアクティビティレポートにのみ反映されます。 </td>
  </tr>
</tbody>
</table>

## ローカルレポート {#local-reports}

一部のMarketo Engageレポートは、使用するプログラムやアセットの数がより限られているので、「マーケティングアクティビティ」の特定のプログラム内にローカルアセットとしてデプロイするのが最適です。 次のような基本的なレポートの設定を検討します。

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
    <td>作成 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report" target="_blank" rel="noopener noreferrer">メールリンクのパフォーマンスレポート</a> メールを送信するプログラムやドリップキャンペーン内で。メール送信内でユーザーがクリックしたリンクに関するインサイトを提供します。</td>
  </tr>
  <tr>
    <td>キャンペーンアクティビティレポート</td>
    <td>を作成 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank" rel="noopener noreferrer">キャンペーン活動レポート</a> 「マーケティングアクティビティ」の運用フォルダー内で期間を選択します。 <br>各ユースケースのトリガーを監視するレポートの設定 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank" rel="noopener noreferrer">キャンペーンフィルターの適用</a>例えば、行動スコアリングトリガー、ライフサイクルの選定トリガー、注目のモーメントトリガーなどです。</td>
  </tr>
  <tr>
    <td>エンゲージメントストリームのパフォーマンスレポート（該当する場合）</td>
    <td>作成 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/engagement-stream-performance-report" target="_blank" rel="noopener noreferrer">エンゲージメントストリームのパフォーマンスレポート</a> お客様のエンゲージメントプログラム内にデプロイされたコンテンツとストリームの有効性を測定するため。 <br>考慮 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/group-email-reports-by-segmentations" target="_blank" rel="noopener noreferrer">レポートの「設定」タブで「セグメント化」フィルターを使用する</a> および次を使用したレポートデータのグループ化 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation" target="_blank" rel="noopener noreferrer">セグメント</a> エンゲージメントプログラムで使用される（担当者、業界など）。 これにより、各セグメントのエンゲージメントパターンに関する深いインサイトを得ることができ、エンゲージメントプログラム（コンテンツ、ストリーム、ストリームケイデンスなど）を改善するための戦略的な変更を行うことができるようになります。</td>
  </tr>
</tbody>
</table>
