---
unique-page-id: 7514009
description: プログラム売上高ステージ分析領域について — Marketto Docs — 製品ドキュメント
title: プログラム売上高ステージ分析領域について
translation-type: tm+mt
source-git-commit: 1c4c4c62215550a09125f76fb76017348aba2bdf
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---


# プログラム売上高ステージ分析領域について {#understanding-the-program-revenue-stage-analysis-area}

この分析領域では、個々のプログラムの有効性を分析したり、チャネル別に要約された結果を表示したりできます。 これは、生成された新しい名前のうち、売上高サイクルモデル内の特定の成功パスステージに到達した名前の数に関する洞察を提供します。

**この分析領域を使用して回答できるビジネスの質問の例を次に示します。**

特定のプログラムの新しい名前が、モデルの特定の段階に到達したことがある場合、

![](assets/one-3.png)

現在、モデルの特定の段階にある特定のプログラムの新しい名前は何名か。

![](assets/two-3.png)

現在のステージに到達するまでに何日かかりますか。

![](assets/three-3.png)

**プログラム売上高段階分析のDimensionと測定**

Dimensionとメジャーは機能別に分類され、システムでは黄色または青の点で表されます。寸法は黄色、測定値は青です。 プログラム売上高ステージ分析のディメンションとメジャーを使用して、レポート内の特定の質問に答えます。

カテゴリ内で使用可能なディメンションまたはメジャーを表示するには、カテゴリ名の横の右矢印をクリックして、カテゴリリストを展開します。 下向き矢印をクリックして、カテゴリリストを折りたたみます。

>[!TIP]
>
>レポート内で特定のディメンションまたはメジャーに関する詳細を取得するには、その上にカーソルを置きます。

**モデル属性**

<table> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Dimension</strong></td> 
   <td colspan="1" rowspan="1"><p><strong>説明</strong></p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>モデルがアクティブ</p></td> 
   <td colspan="1" rowspan="1"><p>モデルが現在承認され、アクティブであるかどうかを示します。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Is Stage Active</p></td> 
   <td colspan="1" rowspan="1"><p>ステージがアクティブかどうかを示します。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>成功パス</p></td> 
   <td colspan="1" rowspan="1"><p>ステージが成功パス上にあるかどうかを説明します。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>モデル</p></td> 
   <td colspan="1" rowspan="1"><p>モデル名</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>ステージ</p></td> 
   <td colspan="1" rowspan="1"><p>売上高サイクルモデルに存在するステージ。 2つのステージ間のメジャーを分析する際に、Fromステージとして使用</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>ステージタイプ</p></td> 
   <td colspan="1" rowspan="1"><p>どのタイプかを説明します。インベントリ、SLA、またはゲートの各段階は</p></td> 
  </tr> 
 </tbody> 
</table>

**プログラム属性**

<table> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Dimension</strong></p></td> 
   <td colspan="1" rowspan="1"><p><strong>説明</strong></p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>プログラムチャネル</p></td> 
   <td colspan="1" rowspan="1"><p>プログラムチャネル</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>プログラム名</p></td> 
   <td colspan="1" rowspan="1"><p>プログラム名</p></td> 
  </tr> 
 </tbody> 
</table>

**プログラムコスト期間**

<table> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Dimension</strong></p></td> 
   <td colspan="1" rowspan="1"><p><strong>説明</strong></p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>コスト年</p></td> 
   <td colspan="1" rowspan="1"><p>プログラム原価期間</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>コスト四半期</p></td> 
   <td colspan="1" rowspan="1"><p>プログラム原価期間</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>コスト月</p></td> 
   <td colspan="1" rowspan="1"><p>プログラム原価期間</p></td> 
  </tr> 
 </tbody> 
</table>

**Stage Membership**

<table> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>測定</strong></p></td> 
   <td colspan="1" rowspan="1"><p><strong>説明</strong></p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>モデルがアクティブ</p></td> 
   <td colspan="1" rowspan="1"><p>モデルが現在承認され、アクティブであるかどうかを示します。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Is Stage Active</p></td> 
   <td colspan="1" rowspan="1"><p>ステージがアクティブかどうかを示します。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>成功パス</p></td> 
   <td colspan="1" rowspan="1"><p>ステージが成功パス上にあるかどうかを説明します。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>新しい名前当たりのコスト</p></td> 
   <td colspan="1" rowspan="1"><p>ステージに到達したことのある新しい名前の平均コスト</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>新しい名前（現在）</p></td> 
   <td colspan="1" rowspan="1"><p>現在ステージにあり、プログラムが獲得したリードの合計数</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>新しい名前（絶対）</p></td> 
   <td colspan="1" rowspan="1"><p>どのタイプかを説明します。インベントリ、SLA、またはゲートの各段階は</p></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**関連記事**
>
>[売上高エクスプローラレポートの作成](../../../../product-docs/reporting/revenue-cycle-analytics/revenue-explorer/create-a-revenue-explorer-report.md)
