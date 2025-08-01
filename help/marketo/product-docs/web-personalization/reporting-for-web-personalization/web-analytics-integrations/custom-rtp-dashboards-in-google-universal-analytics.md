---
unique-page-id: 7504238
description: Google ユニバーサルアナリティクスでのカスタム RTP ダッシュボード — Marketo ドキュメント — 製品ドキュメント
title: Google ユニバーサルアナリティクスでのカスタム RTP ダッシュボード
exl-id: 712c71b6-74eb-4743-9ca8-50c912278e62
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 70%

---

# Google ユニバーサルアナリティクスでのカスタム RTP ダッシュボード {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[RTP を Google ユニバーサルアナリティクスに連携](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

この投稿では、Google ユニバーサルアナリティクス（GUA）で RTP ダッシュボードを設定する方法を説明します。RTP から GUA に送信されるデータは、次の 2 つの異なるカスタムダッシュボードとして設定できます。

* RTP B2B
* RTP エンゲージメント

## カスタムダッシュボードを設定する {#setting-up-a-custom-dashboard}

1. Google Analytics にログインします。上部のメニューの「**[!UICONTROL レポート]**」をクリックします。**[!UICONTROL ダッシュボード]** および **[!UICONTROL 新規ダッシュボード]** をクリックします。

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. 「**空白のキャンバス**」を選択し、**ダッシュボード名**&#x200B;を入力して「**[!UICONTROL マイレポートを作成]**.」をクリックします。

1. 「**[!UICONTROL ウィジェットを追加]**」をクリックし、新しいウィジェットを作成します。

   ![](assets/image2015-3-22-16-3a46-3a48.png)

## RTP B2B ダッシュボード {#rtp-b-b-dashboard}

このダッシュボードでは、B2B の観点からウェブサイトのパフォーマンスを分析できます。

業種、売上高、規模、アカウントベースリスト、ターゲットセグメントなどの基準で、訪問元やオンサイトの行動といった情報が表示されます。

ダッシュボードは、3 つの列で構成されています。

* トラフィックソース
* セグメント化
* ファーモグラフィックドリルダウン

1. **RTP B2B ダッシュボード**」という新しいダッシュボードを作成し、以下のようにウィジェットを定義します。

![](assets/image2015-3-22-16-3a50-3a3.png)

<table>
 <thead>
  <tr>
   <th>
    <div>
      列 1 - トラフィックソース
    </div></th>
   <th>
    <div> <strong>列 2 - セグメント化</strong>
    </div></th>
   <th>
    <div> <strong>列 3 - ファーモグラフィックドリルダウン</strong>
    </div></th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>
    <ul>
     <li>名前：セグメントおよびチャネル別セッション</li>
     <li>ウィジェットタイプ：<span class="uicontrol"> 棒グラフ </span><br></li>
     <li><span class="uicontrol"> 次を表示する棒グラフを作成 </span>: <span class="uicontrol"> セッション </span></li>
     <li><span class="uicontrol"> グループ化基準 </span>:<span class="uicontrol"> イベントラベル </span></li>
     <li><span class="uicontrol"> ピボットの基準 </span>: <span class="uicontrol"> 既定のチャネル グループ化 </span></li>
     <li>フィルター：<br><span class="uicontrol"> 表示のみ </span> | <span class="uicontrol"> イベントカテゴリ </span> （<span class="uicontrol"> 含む </span>） RTP セグメント</li>
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td>
    <ul>
     <li>名前：RTP でセグメント化されたユーザー数</li>
     <li>タイプ：<span class="uicontrol">2.1 指標</span></li>
     <li><span class="uicontrol"> 次の指標を表示 </span>: <span class="uicontrol"> ユーザー </span><br></li>
     <li>フィルター：<br><span class="uicontrol"> 表示のみ </span> | <span class="uicontrol"> イベントカテゴリ </span> （含む） RTP セグメント</li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td>
    <ul>
     <li>名前：業種別セッション</li>
     <li>タイプ：<span class="uicontrol"> 円グラフ </span><br></li>
     <li><span class="uicontrol"> 次を表示する円グラフを作成 </span>: <span class="uicontrol"> セッション </span></li>
     <li><span class="uicontrol"> グループ化基準 </span> : <span class="uicontrol">RTP-Industry</span></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
  </tr>
  <tr>
   <th>
    <ul>
     <li><strong>名前：業種およびチャネル別セッション</strong></li>
     <li><strong>ウィジェットタイプ：<span class="uicontrol"> 棒グラフ </span></strong></li>
     <li><strong><span class="uicontrol"> 次を表示する棒グラフを作成 </span>: <span class="uicontrol"> セッション </span></strong></li>
     <li><strong><span class="uicontrol"> グループ化基準 </span>:<span class="uicontrol">RTP-Industry</span></strong></li>
     <li><strong><span class="uicontrol"> ピボットの基準 </span>: <span class="uicontrol"> 既定のチャネル グループ化 </span></strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li>
    </ul></th>
   <th>
    <ul>
     <li><strong>名前：国別のセグメント化セッション</strong></li>
     <li><strong>タイプ：<span class="uicontrol"> ジオマップ </span></strong></li>
     <li><strong><span class="uicontrol"> 選択した指標をプロット </span>: <span class="uicontrol"> 国 </span> | <span class="uicontrol"> セッション </span></strong></li>
     <li><strong><span class="uicontrol"> 地域を選択 </span>: <span class="uicontrol"> 世界 </span></strong></li>
     <li><strong>フィルター：<span class="uicontrol"> 表示のみ </span> | <span class="uicontrol"> イベントカテゴリ </span> （含む） RTP セグメント</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th>
   <th>
    <ul>
     <li><strong>名前：RTP カテゴリ別セッション</strong></li>
     <li><strong>タイプ：<span class="uicontrol"> 円グラフ </span></strong></li>
     <li><strong><span class="uicontrol"> 次を表示する円グラフを作成 </span>: <span class="uicontrol"> セッション </span></strong></li>
     <li><strong><span class="uicontrol"> グループ化基準 </span>:<span class="uicontrol">RTP-Category</span></strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th>
  </tr>
  <tr>
   <th> </th>
   <th>
    <ul>
     <li>名前：上位ターゲットセグメント</li>
     <li>タイプ：<span class="uicontrol">Bar</span></li>
     <li><span class="uicontrol"> 次を表示する棒グラフを作成 </span>: <span class="uicontrol"> ユーザー </span></li>
     <li><span class="uicontrol"> グループ化 </span>: <span class="uicontrol"> イベントアクション </span></li>
     <li>フィルター：<span class="uicontrol"> 表示のみ </span> | <span class="uicontrol"> イベントカテゴリ </span> （含む） RTP セグメント</li>
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th>
   <th>
    <ul>
     <li>名前：RTP グループ別セッション</li>
     <li>タイプ：棒グラフ<br></li>
     <li>次の棒グラフを作成：セッション</li>
     <li>グループ分けの単位：RTP-Group</li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th>
  </tr>
  <tr>
   <th> </th>
   <th>
    <ul>
     <li>名前：上位セグメント別セッションおよび目標</li>
     <li>タイプ：表形式<br></li>
     <li>次の列を表示します。<br>イベントラベル | セッション |目標コンバージョン率</li>
     <li>フィルター：<br>［表示の絞り込み］イベントカテゴリ（含む）：RTP-Segments</li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th>
   <th> </th>
  </tr>
 </tbody>
</table>

## RTP エンゲージメントダッシュボード {#rtp-engagement-dashboard}

このダッシュボードでは、RTP キャンペーンのパフォーマンスと、レコメンデーションエンジンのエンゲージメントを分析できます。平均の比較を提供します。セッション時間と、セッションごとのページ数：

* エンゲージなし
* エンゲージ済み（パーソナライズしたキャンペーンのインプレッションおよびクリック数）  
* レコメンデーションエンジンのクリック数と、推奨される上位のコンテンツ

**RTP エンゲージメントダッシュボード**&#x200B;という新しいダッシュボードを作成し、以下のようにウィジェットを定義します。

![](assets/image2015-3-22-17-3a7-3a19.png)

<table>
 <thead>
  <tr>
   <th>
    <div> <strong>列 1 - キャンペーンの露出</strong>
    </div></th>
   <th>
    <div> <strong>列 2 - キャンペーンのクリックスルー率</strong>
    </div></th>
   <th>
    <div> <strong>列 3 - レコメンデーションエンジン</strong>
    </div></th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>
    <ul>
     <li>名前：<strong>合計 CTA（エンゲージメント）</strong></li>
     <li>タイプ：<strong>2.1 指標</strong></li>
     <li>次の指標を表示：<strong>合計イベント数</strong></li>
     <li>フィルター：<br><strong>[表示の絞り込み] イベントカテゴリ（含む）：RTP-Campaigns</strong><br><strong>[表示の絞り込み] イベントアクション（完全に一致）：インプレッション</strong>[表示しない] イベントラベル（含む）：#</li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td>
    <ul>
     <li>名前：<strong>合計 CTA（クリックスルー）</strong></li>
     <li>タイプ：<strong>2.1 指標</strong></li>
     <li>次の指標を表示：<strong>合計イベント数</strong></li>
     <li>フィルター：<br><strong>［表示の絞り込み］イベントカテゴリ（含む）：RTP-Campaigns</strong><br><strong>［表示の絞り込み］イベントアクション（完全に一致）：インプレッション</strong><strong>［表示しない］イベントラベル（含む）：#</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td>
    <ul>
     <li>名前：<strong>CRE - 合計クリック数</strong></li>
     <li>タイプ：<strong><span class="uicontrol">2.1 指標</span></strong><br></li>
     <li><span class="uicontrol"> 次の指標を表示 </span>: <strong><span class="uicontrol"> ページビュー数 </span></strong></li>
     <li>フィルター：<strong>[<span class="uicontrol">only show</span>] <span class="uicontrol"> ページ </span> （<span class="uicontrol">containing</span>）: rcmd</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
  </tr>
  <tr>
   <td colspan="1">
    <ul>
     <li>名前：<strong>平均セッション時間（エンゲージメント）</strong></li>
     <li>タイプ：<strong>2.1 指標</strong></li>
     <li>次の指標を表示：<strong>平均セッション時間</strong></li>
     <li>フィルター：<br><strong>［表示の絞り込み］イベントカテゴリ（含む）：RTP-Campaigns</strong><br><strong>［表示の絞り込み］イベントアクション（完全に一致）：インプレッション</strong><strong>［表示しない］イベントラベル（含む）：#</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td colspan="1">
    <ul>
     <li>名前：<strong>平均セッション時間（クリックスルー）</strong></li>
     <li>タイプ：<strong>2.1 指標</strong></li>
     <li>次の指標を表示：<strong>平均セッション時間</strong></li>
     <li>フィルター：<br><strong>［表示の絞り込み］イベントカテゴリ（完全に一致）：RTP-Campaigns</strong><br><strong>［表示の絞り込み］イベントアクション（完全に一致）：クリック数</strong><strong>［表示しない］イベントラベル（含む）：#</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td colspan="1">
    <ul>
     <li>名前：<strong>CRE - 推奨される上位のコンテンツ</strong></li>
     <li>タイプ：<strong><span class="uicontrol">表形式</span></strong><br></li>
     <li><span class="uicontrol"> 次の列を表示 </span>:<br><strong><span class="uicontrol"> ページタイトル </span> | <span class="uicontrol"> ページビュー </span></strong><br></li>
     <li>フィルター：<br> フィルター：<strong>[<span class="uicontrol">only show</span>] <span class="uicontrol"> ページ </span> （<span class="uicontrol">containing</span>）: rcmd</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
  </tr>
  <tr>
   <td>
    <ul>
     <li>名前：<strong>ページ／セッション（エンゲージメント））</strong></li>
     <li>タイプ：<strong><span class="uicontrol">2.1 Metric</span> </strong></li>
     <li><span class="uicontrol"> 次の指標を表示 </span>:<strong><span class="uicontrol"> ページ/セッション </span></strong></li>
     <li>フィルター：<br><strong>[<span class="uicontrol">only show</span>] <span class="uicontrol"> イベントカテゴリ </span> （<span class="uicontrol">exactly matching</span>）: RTP-Campaigns</strong></li>
     <li><strong>[<span class="uicontrol"> のみ表示 </span>] <span class="uicontrol"> イベント アクション </span> （<span class="uicontrol"> 完全一致 </span>）: インプレッション</strong></li>
     <li><strong>[<span class="uicontrol"> 表示しない </span>] <span class="uicontrol"> イベント ラベル </span> （<span class="uicontrol"> 含む </span>）: #</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td>
    <ul>
     <li>名前：<strong>ページ/セッション（クリックスルー）</strong></li>
     <li>タイプ：<strong>2.1 指標</strong></li>
     <li>次の指標を表示：<strong>ページ／セッション</strong></li>
     <li>フィルター：<br><strong>［表示の絞り込み］イベントカテゴリ（完全一致）：RTP-Campaigns</strong></li>
     <li><strong>［表示の絞り込み］イベントアクション（完全一致）：クリック数</strong></li>
     <li><strong>［表示しない］イベントラベル（含む）：#</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td> </td>
  </tr>
  <tr>
   <td>
    <ul>
     <li>名前：<strong>CTA 別インプレッション</strong></li>
     <li>タイプ：<strong><span class="uicontrol">表形式</span></strong></li>
     <li><span class="uicontrol"> 次の列を表示 </span>:<strong><span class="uicontrol"> イベントラベル </span> | <span class="uicontrol"> 合計イベント数 </span> | <span class="uicontrol"> ユーザー </span></strong></li>
     <li>フィルター：<br><strong>[<span class="uicontrol">only show</span>] <span class="uicontrol"> イベントカテゴリ </span> （<span class="uicontrol">exactly matching</span>）: RTP-Campaigns</strong><br><strong>[<span class="uicontrol">only show</span>] <span class="uicontrol"> イベントアクション </span> （<span class="uicontrol">exactly matching</span>）: impression</strong><strong>[<span class="uicontrol">don't show</span>] <span class="uicontrol"> イベントラベル </span> （<span class="uicontrol"></span> </strong> containingTeam）:</li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td>
    <ul>
     <li>名前：<strong>CTA 別クリックスルー率</strong></li>
     <li>タイプ：<strong><span class="uicontrol">表形式</span></strong></li>
     <li><span class="uicontrol"> 次の列を表示 </span>:<strong><span class="uicontrol"> イベントラベル </span> | <span class="uicontrol"> 合計イベント数 </span> | <span class="uicontrol"> ユーザー </span></strong></li>
     <li>フィルター：<br><strong>[<span class="uicontrol">only show</span>] <span class="uicontrol"> イベントカテゴリ </span> （<span class="uicontrol">exactly matching</span>）: RTP-Campaigns</strong><br><strong>[<span class="uicontrol">only show</span>] <span class="uicontrol"> イベントアクション </span> （<span class="uicontrol">exactly matching</span>）：クリック数 </strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a43-3a4.png" data-linked-resource-id="7504270" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td> </td>
  </tr>
 </tbody>
</table>

>[!MORELIKETHIS]
>
>[RTP を Google ユニバーサルアナリティクスに連携](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
>
>[Google ユニバーサルアナリティクスでのカスタム RTP レポート](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
