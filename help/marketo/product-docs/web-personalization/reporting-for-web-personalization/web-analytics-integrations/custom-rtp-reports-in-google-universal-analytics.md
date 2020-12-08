---
unique-page-id: 7504218
description: Google Universal Analytics - Marketto Docs — 製品ドキュメント内のカスタムRTPレポート
title: Google Universal AnalyticsでのカスタムRTPレポート
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---


# Google Universal AnalyticsでのカスタムRTPレポート {#custom-rtp-reports-in-google-universal-analytics}

>[!NOTE]
>
>**前提条件**
>
>[RTPとGoogle Universal Analyticsの統合](integrate-rtp-with-google-universal-analytics.md)

この投稿では、Google Universal Analytics(GUA)用のRTPカスタムレポートの設定方法を説明します。  RTPからGUAに送信されるデータは、次の2つのカスタムレポートとして設定できます。

* RTP B2B
* RTPエンゲージメント

## カスタムレポートの設定 {#setting-up-a-custom-report}

1. Google Analyticsにログインします。
1. 上部のメニューにある「**カスタマイズ**」をクリックします。
1. 「 **新規カスタムレポート」をクリックします。**

** ![](assets/image2015-3-22-16-3a10-3a48.png)

**

## RTP B2Bレポート {#rtp-b-b-report}

1. レポートに「 **RTP B2B Report**」という名前を付けます。
1. 「1st」タブに**Industry **という名前を付けます。

   1. (注意：このタブを **重複し** 、同様のタブを追加作成します（手順5）。

1. 「**エクスプローラ**」レポートタイプを選択します。\
   ** ![](assets/image2015-3-22-16-3a15-3a25.png)

   **

1. 「 **指標グループ** 」セクションで、ビジネスに関連する指標を選択します。

   1. 以下を推奨します。\
      ** ![](assets/image2015-3-22-16-3a16-3a40.png)

      **

1. このタブを4回重複し、名前を付けます。

   1. **業界**
   1. **グループ**
   1. **カテゴリ**
   1. **ABM**
   1. **組織**

   ![](assets/image2015-3-22-16-3a17-3a41.png)

1. 「 **Dimensionドリルダウン** 」セクションで、各タブに関連するディメンションを以下のように設定します。

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      タブ名 
    </div></th> 
   <th> 
    <div>
      Dimensionのドリルダウン 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>業界</td> 
   <td><img src="assets/1.png" data-linked-resource-id="7514675" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>グループ</td> 
   <td><img src="assets/2.png" data-linked-resource-id="7514674" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>カテゴリ</td> 
   <td><img src="assets/3.png" data-linked-resource-id="7514673" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>ABM</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>組織</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. フィルターを設定せず、このレポートを**すべてのWebサイトデータ**で使用できるように設定します（または、特定のAnalyticsアカウントに関連する場合は変更します）。
1. 「 **保存**」をクリックします。\
   ![](assets/image2015-3-22-16-3a21-3a23.png)

## RTPエンゲージメントレポート {#rtp-engagement-report}

1. レポートに「 **RTPエンゲージメントレポート」という名前を付けます。**
1. 1番目のタブ名を「 **すべてのエンゲージメント」に設定します**

   1. (注意：このタブを重複し、同様のタブを追加作成します — 手順5)

1. 「 **エクスプローラ** 」レポートタイプを選択します。\
   ![](assets/image2015-3-22-16-3a23-3a36.png)

1. 「指標グループ」セクションで、ビジネスに関連する指標を選択します。 次に推奨事項を示します。\
   ![](assets/image2015-3-22-16-3a24-3a57.png)

1. このタブを4回重複し、名前を付けます。

   1. **すべてのアクション**
   1. **業種別関与**
   1. **グループ別のエンゲージメント**
   1. **カテゴリ別関与**
   1. **ABMによるエンゲージメント**

   ** ![](assets/image2015-3-22-16-3a26-3a21.png)\**

1. 「 **Dimensionドリルダウン** 」セクションで、各タブに関連するディメンションを次のように設定します。

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      タブ名 
    </div></th> 
   <th> 
    <div>
      Dimensionのドリルダウン 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>すべてのアクション</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>ABMによるエンゲージメント</td> 
   <td><img width="277" src="assets/4.png" data-linked-resource-id="7514678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>カテゴリ別関与</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>グループ別のエンゲージメント</td> 
   <td><img src="assets/c.png" data-linked-resource-id="7514681" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>業種別関与</td> 
   <td><img src="assets/b.png" data-linked-resource-id="7514682" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. 次のフィルターを設定します。
1. 

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Inc/Exc 
    </div></th> 
   <th> 
    <div>
      フィールド 
    </div></th> 
   <th> 
    <div>
      一致タイプ 
    </div></th> 
   <th> 
    <div>
      値 
    </div></th> 
   <th colspan="1"> 
    <div>
      コメント 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><p>含める</p></td> 
   <td><p>イベントカテゴリ</p></td> 
   <td>Regex</td> 
   <td>RTPキャンペーン|RTP-Recommendations|RTPセグメント</td> 
   <td colspan="1">RTPに関連しない他のカスタムイベントをすべてフィルタします。</td> 
  </tr> 
  <tr> 
   <td>除外</td> 
   <td>イベントラベル</td> 
   <td>Regex</td> 
   <td>#</td> 
   <td colspan="1">キャンペーン名に#を使用して、レポートキャンペーンからフィルタできます。</td> 
  </tr> 
 </tbody> 
</table>

1. このレポートを**すべてのウェブサイトデータ**で使用可能に設定する（または必要に応じて変更）

   ![](assets/image2015-3-22-16-3a29-3a5.png)

1. 「 **保存**」をクリックします。

![](assets/image2015-3-22-16-3a30-3a0.png)

>[!NOTE]
>
>**関連記事**
>
>[RTPとGoogle Universal Analyticsの統合](integrate-rtp-with-google-universal-analytics.md)
>
>[Google Universal AnalyticsでのカスタムRTPダッシュボード](custom-rtp-dashboards-in-google-universal-analytics.md)

