---
unique-page-id: 7504238
description: Google ユニバーサルアナリティクスでのカスタム RTP ダッシュボード — Marketo ドキュメント — 製品ドキュメント
title: Google ユニバーサルアナリティクスでのカスタム RTP ダッシュボード
exl-id: 712c71b6-74eb-4743-9ca8-50c912278e62
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '748'
ht-degree: 100%

---

# Google ユニバーサルアナリティクスでのカスタム RTP ダッシュボード {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[RTP を Google ユニバーサルアナリティクスに連携する](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

この投稿では、Google ユニバーサルアナリティクス（GUA）で RTP ダッシュボードを設定する方法を説明します。RTP から GUA に送信されるデータは、次の 2 つの異なるカスタムダッシュボードとして設定できます。

* RTP B2B
* RTP エンゲージメント

## カスタムダッシュボードを設定する {#setting-up-a-custom-dashboard}

1. Google Analytics にログインします。上部のメニューの「**レポート**」をクリックします。「**マイレポート**」、「**+新しいマイレポート**」の順にクリックします。

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. 「**空白のキャンバス**」を選択し、**ダッシュボード名**&#x200B;を入力して「**マイレポートを作成**.」をクリックします。

1. 「**ウィジェットを追加**」をクリックし、新しいウィジェットを作成します。

   ![](assets/image2015-3-22-16-3a46-3a48.png)

## RTP B2B ダッシュボード {#rtp-b-b-dashboard}

このダッシュボードでは、B2B の観点から Web サイトのパフォーマンスを分析できます。

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
     <li>ウィジェットタイプ：棒グラフ<br></li> 
     <li>次の棒グラフを作成：セッション</li> 
     <li>グループ分けの単位：イベントラベル</li> 
     <li>ピボット：デフォルトチャネルグループ</li> 
     <li>フィルター：<br>［表示の絞り込み］イベントカテゴリ（含む）：RTP-Segments</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>名前：RTP でセグメント化されたユーザー数</li> 
     <li>タイプ：2.1 指標</li> 
     <li>次の指標を表示：ユーザー<br></li> 
     <li>フィルター：<br>［表示の絞り込み］イベントカテゴリ（含む）：RTP-Segments</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>名前：業種別セッション</li> 
     <li>タイプ：円グラフ<br></li> 
     <li>次の円グラフを作成：セッション</li> 
     <li>グループ分けの単位：RTP-Industry</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <th> 
    <ul> 
     <li><strong>名前：業種およびチャネル別セッション</strong></li> 
     <li><strong>ウィジェットタイプ：棒グラフ</strong></li> 
     <li><strong>次の棒グラフを作成：セッション</strong></li> 
     <li><strong>グループ分けの単位：RTP-Industry</strong></li> 
     <li><strong>ピボット：デフォルトチャネルグループ</strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>名前：国別のセグメント化セッション</strong></li> 
     <li><strong>タイプ：地図表示</strong></li> 
     <li><strong>選択した指標をプロット：国 | セッション</strong></li> 
     <li><strong>地域を選択：世界</strong></li> 
     <li><strong>フィルター：［表示の絞り込み］イベントカテゴリ（含む）：RTP-Segments</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>名前：RTP カテゴリ別セッション</strong></li> 
     <li><strong>タイプ：円グラフ</strong></li> 
     <li><strong>次の円グラフを作成：セッション</strong></li> 
     <li><strong>グループ分けの単位：RTP-Category</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>名前：上位ターゲットセグメント</li> 
     <li>タイプ：棒グラフ</li> 
     <li>次の棒グラフを作成：ユーザー</li> 
     <li>グループ分けの単位：イベントアクション</li> 
     <li>フィルター：［表示の絞り込み］イベントカテゴリ（含む）：RTP-Segments</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>名前：RTP グループ別セッション</li> 
     <li>タイプ：棒グラフ<br></li> 
     <li>次の棒グラフを作成：セッション</li> 
     <li>グループ分けの単位：RTP-Group</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>名前：上位セグメント別セッションおよび目標</li> 
     <li>タイプ：表形式<br></li> 
     <li>次の列を表示します。<br>イベントラベル | セッション |目標コンバージョン率</li> 
     <li>フィルター：<br>［表示の絞り込み］イベントカテゴリ（含む）：RTP-Segments</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
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
     <li>フィルター：<br><strong>［表示の絞り込み］イベントカテゴリ（含む）：RTP-Campaigns</strong><br><strong>［表示の絞り込み］イベントアクション（完全に一致）：インプレッション</strong><strong>［表示しない］イベントラベル（含む）：#</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>名前：<strong>合計 CTA（クリックスルー）</strong></li> 
     <li>タイプ：<strong>2.1 指標</strong></li> 
     <li>次の指標を表示：<strong>合計イベント数</strong></li> 
     <li>フィルター：<br><strong>［表示の絞り込み］イベントカテゴリ（含む）：RTP-Campaigns</strong><br><strong>［表示の絞り込み］イベントアクション（完全に一致）：インプレッション</strong><strong>［表示しない］イベントラベル（含む）：#</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>名前：<strong>CRE - 合計クリック数</strong></li> 
     <li>タイプ：<strong>2.1 指標</strong><br></li> 
     <li>次の指標を表示：<strong>ページビュー</strong></li> 
     <li>フィルター：<strong>表示の絞り込み | ページ含む）：rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>名前：<strong>平均セッション時間（エンゲージメント）</strong></li> 
     <li>タイプ：<strong>2.1 指標</strong></li> 
     <li>次の指標を表示：<strong>平均セッション時間</strong></li> 
     <li>フィルター：<br><strong>［表示の絞り込み］イベントカテゴリ（含む）：RTP-Campaigns</strong><br><strong>［表示の絞り込み］イベントアクション（完全に一致）：インプレッション</strong><strong>［表示しない］イベントラベル（含む）：#</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>名前：<strong>平均セッション時間（クリックスルー）</strong></li> 
     <li>タイプ：<strong>2.1 指標</strong></li> 
     <li>次の指標を表示：<strong>平均セッション時間</strong></li> 
     <li>フィルター：<br><strong>［表示の絞り込み］イベントカテゴリ（完全に一致）：RTP-Campaigns</strong><br><strong>［表示の絞り込み］イベントアクション（完全に一致）：クリック数</strong><strong>［表示しない］イベントラベル（含む）：#</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>名前：<strong>CRE - 推奨される上位のコンテンツ</strong></li> 
     <li>タイプ：<strong>表形式</strong><br></li> 
     <li>表示する列：<br><strong>ページタイトル | ページビュー</strong><br></li> 
     <li>フィルター：<br>フィルター：<strong>表示の絞り込み：ページ（含む）：rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>名前：<strong>ページ／セッション（エンゲージメント））</strong></li> 
     <li>タイプ：<strong>2.1 指標</strong></li> 
     <li>次の指標を表示：<strong>ページ／セッション</strong></li> 
     <li>フィルター：<br><strong>［表示の絞り込み］イベントカテゴリ（完全一致）：RTP-Campaigns</strong></li> 
     <li><strong>［表示の絞り込み］イベントアクション（完全一致）：インプレッション</strong></li> 
     <li><strong>［表示しない］イベントラベル（含む）：#</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>名前：<strong>ページ/セッション（クリックスルー）</strong></li> 
     <li>タイプ：<strong>2.1 指標</strong></li> 
     <li>次の指標を表示：<strong>ページ／セッション</strong></li> 
     <li>フィルター：<br><strong>［表示の絞り込み］イベントカテゴリ（完全一致）：RTP-Campaigns</strong></li> 
     <li><strong>［表示の絞り込み］イベントアクション（完全一致）：クリック数</strong></li> 
     <li><strong>［表示しない］イベントラベル（含む）：#</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>名前：<strong>CTA 別インプレッション</strong></li> 
     <li>タイプ：<strong>表形式</strong></li> 
     <li>表示する列：<strong>イベントラベル | 合計イベント数 | ユーザー</strong></li> 
     <li>フィルター：<br><strong>［表示の絞り込み］イベントカテゴリ（含む）：RTP-Campaigns</strong><br><strong>［表示の絞り込み］イベントアクション（完全に一致）：インプレッション</strong><strong>［表示しない］イベントラベル（含む）：#</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>名前：<strong>CTA 別クリックスルー率</strong></li> 
     <li>タイプ：<strong>表形式</strong></li> 
     <li>表示する列：<strong>イベントラベル | 合計イベント数 | ユーザー</strong></li> 
     <li>フィルター：<br><strong>［表示の絞り込み］イベントカテゴリ（完全に一致）：RTP-Campaigns</strong><br><strong>［表示の絞り込み］イベントアクション（完全に一致）：クリック数</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a43-3a4.png" data-linked-resource-id="7504270" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[RTP を Google ユニバーサルアナリティクスに連携する](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
>
>[Google ユニバーサルアナリティクスでのカスタム RTP レポート](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
