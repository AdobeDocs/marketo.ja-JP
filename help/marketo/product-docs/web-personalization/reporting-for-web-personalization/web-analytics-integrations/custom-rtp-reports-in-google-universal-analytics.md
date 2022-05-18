---
unique-page-id: 7504218
description: Google ユニバーサルアナリティクスでのカスタム RTP レポート - Marketo ドキュメント - 製品ドキュメント
title: Google ユニバーサルアナリティクスでのカスタム RTP レポート
exl-id: c8b1e653-03b8-48bc-b80d-3e6cdf3485c3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '386'
ht-degree: 100%

---

# Google ユニバーサルアナリティクスでのカスタム RTP レポート {#custom-rtp-reports-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[RTP を Google ユニバーサルアナリティクスに連携](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

この記事では、Google ユニバーサルアナリティクス（GUA）用に RTP カスタムレポートを設定する方法を説明します。RTP から GUA に送信されるデータは、次の 2 つの異なるカスタムレポートとして設定できます。

* RTP B2B
* RTP エンゲージメント

## カスタムレポートの設定 {#setting-up-a-custom-report}

1. Google Analytics にログインします。

1. 上部のメニューの「**カスタマイズ**」をクリックします。

1. 「**+新規カスタムレポート**」をクリックします。

![](assets/image2015-3-22-16-3a10-3a48.png)

## RTP B2B レポート {#rtp-b-b-report}

1. レポートに **RTP B2B レポート**&#x200B;と名前を付けます。

1. 1 番目のタブに&#x200B;**業界**&#x200B;と名前を付けます。

>[!NOTE]
>
>手順 5 で、**このタブを複製**&#x200B;して追加の類似したものを作成します

1. **エクスプローラー**&#x200B;レポートタイプを選択します。

   ![](assets/image2015-3-22-16-3a15-3a25.png)

1. **指標グループ**&#x200B;セクションで、ビジネスに関連する指標を選択します。

   a. 以下をお勧めします。

   ![](assets/image2015-3-22-16-3a16-3a40.png)

1. このタブを 4 回複製し、名前を付けます。

   1. **業界**
   1. **グループ**
   1. **カテゴリ**
   1. **ABM**
   1. **組織**

   ![](assets/image2015-3-22-16-3a17-3a41.png)

1. **ディメンションドリルダウン**&#x200B;セクションで、各タブの関連するディメンションを次のように設定します。

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      タブ名 
    </div></th> 
   <th> 
    <div>
      ディメンションドリルダウン
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

1. フィルターを設定せず、このレポートを&#x200B;**すべてのウェブサイトデータ**&#x200B;で使用できるように設定します（または特定の Analytics アカウントに関連する場合は変更します）。

1. 「**保存**」をクリックします。

   ![](assets/image2015-3-22-16-3a21-3a23.png)

## RTP エンゲージメントレポート {#rtp-engagement-report}

1. レポートに **RTP エンゲージメントレポート**&#x200B;と名前を付けます。

1. 1 番目のタブ名を&#x200B;**すべてのエンゲージメント**&#x200B;に設定します。

>[!NOTE]
>
>手順 5 で、このタブを複製して追加の類似したものを作成します

1. **エクスプローラー**&#x200B;レポートタイプを選択します。

   ![](assets/image2015-3-22-16-3a23-3a36.png)

1. 指標グループセクションで、ビジネスに関連する指標を選択します。次に推奨事項を示します。

   ![](assets/image2015-3-22-16-3a24-3a57.png)

1. このタブを 4 回複製し、名前を付けます。

   1. **すべてのエンゲージメント**
   1. **業界別のエンゲージメント**
   1. **グループ別のエンゲージメント**
   1. **カテゴリ別のエンゲージメント**
   1. **ABM によるエンゲージメント**

   ![](assets/image2015-3-22-16-3a26-3a21.png)

1. **ディメンションドリルダウン**&#x200B;セクションで、各タブの関連するディメンションを次のように設定します。

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      タブ名 
    </div></th> 
   <th> 
    <div>
      ディメンションドリルダウン 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>すべてのエンゲージメント</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>ABM 別のエンゲージメント</td> 
   <td><img width="277" src="assets/4.png" data-linked-resource-id="7514678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>カテゴリ別のエンゲージメント</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>グループ別のエンゲージメント</td> 
   <td><img src="assets/c.png" data-linked-resource-id="7514681" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>業界別のエンゲージメント</td> 
   <td><img src="assets/b.png" data-linked-resource-id="7514682" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. 次のフィルターを設定します。

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Inc／Exc 
    </div></th> 
   <th> 
    <div>
      フィールド 
    </div></th> 
   <th> 
    <div>
      一致のタイプ 
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
   <td><p>含む</p></td> 
   <td><p>イベントカテゴリ</p></td> 
   <td>正規表現</td> 
   <td>RTP-Campaigns|RTP-Recommendations|RTP-Segments</td> 
   <td colspan="1">RTP に関連していない他のすべてのカスタムイベントをフィルタリングします</td> 
  </tr> 
  <tr> 
   <td>除外する</td> 
   <td>イベントラベル</td> 
   <td>正規表現</td> 
   <td>#</td> 
   <td colspan="1">キャンペーン名に#を使用して、レポートキャンペーンからフィルタリングできます</td> 
  </tr> 
 </tbody> 
</table>

1. このレポートを&#x200B;**すべてのウェブサイトデータ**&#x200B;で使用できるように設定します（必要に応じて変更します）。

   ![](assets/image2015-3-22-16-3a29-3a5.png)

1. 「**保存**」をクリックします。

![](assets/image2015-3-22-16-3a30-3a0.png)

>[!MORELIKETHIS]
>
>[RTP を Google ユニバーサルアナリティクスに連携](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)
>
>[Google ユニバーサルアナリティクスでのカスタム RTP ダッシュボード](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-dashboards-in-google-universal-analytics.md)
