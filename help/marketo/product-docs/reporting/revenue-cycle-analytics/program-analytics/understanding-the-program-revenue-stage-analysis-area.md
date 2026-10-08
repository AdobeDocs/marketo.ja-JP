---
unique-page-id: 7514009
description: Adobe Marketo Engageのプログラムのレベニューステージ分析領域について詳しく説明します。 このガイドを使用して、次のステップを完了してください。
title: プログラム収益ステージ分析領域について
exl-id: 7310655f-a06e-4e02-a094-d942fff689c3
feature: Reporting, Revenue Cycle Analytics
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
    internal-label: Reporting
  - id: 126e34f9-e02a-505e-9978-ea36537f3ef9
    internal-label: Revenue Cycle Analytics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 94%
---
# プログラム収益ステージ分析領域について {#understanding-the-program-revenue-stage-analysis-area}

この分析領域では、個々のプログラムの効果を分析することも、特定の期間のチャネルごとに要約した結果を確認することもできます。 生成された新しい名前のうち、収益サイクルモデルの成功パス内で特定のステージに到達したものがどれだけあるかについてのインサイトを提供します。

**この分析領域を使用して回答できるビジネスの質問の例を次に示します**。

特定のプログラムで、モデルの特定のステージに達した新しい名前はいくつあるか。

![](assets/one-3.png)

特定のプログラムで、モデルの特定のステージにある新しい名前は現在いくつあるか。

![](assets/two-3.png)

リードが現在のステージに達するまでに何日かかっているか。

![](assets/three-3.png)

**プログラム収益ステージ分析のディメンションと測定**

ディメンションと測定値は機能別に分類され、システムでは黄色と青色のドットで表されます。黄色のドットがディメンション、青色のドットが測定値です。 プログラム収益ステージ分析の各ディメンションと測定を使用して、レポートで特定の質問に答えます。

カテゴリ内で使用可能なディメンションまたは測定を表示するには、カテゴリ名の横にある右矢印をクリックして、カテゴリリストを展開します。 下矢印をクリックして、カテゴリリストを折りたたみます。

>[!TIP]
>
>レポート内で特定のディメンションまたは指標に関する詳細情報を表示するには、その項目にポインタを合わせます。

**モデルの属性**

<table>
 <tbody>
  <tr>
   <td colspan="1" rowspan="1"><strong>ディメンション</strong></td>
   <td colspan="1" rowspan="1"><p><strong>説明</strong></p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>モデルはアクティブか</p></td>
   <td colspan="1" rowspan="1"><p>現在モデルが承認済みでアクティブかどうかを示します。</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>ステージはアクティブか</p></td>
   <td colspan="1" rowspan="1"><p>ステージがアクティブかどうかを示します。</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>成功パス上</p></td>
   <td colspan="1" rowspan="1"><p>ステージが成功パス上にあるかどうかを説明します</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>モデル</p></td>
   <td colspan="1" rowspan="1"><p>モデル名</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>ステージ</p></td>
   <td colspan="1" rowspan="1"><p>収益サイクルモデルに存在するステージ。 2 つのステージ間の測定を分析する際に、「開始」ステージとして使用されます</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>ステージタイプ</p></td>
   <td colspan="1" rowspan="1"><p>各ステージが在庫、SLA、またはゲートのどのタイプに分類されるかを説明します。</p></td>
  </tr>
 </tbody>
</table>

**プログラムの属性**

<table>
 <tbody>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>ディメンション</strong></p></td>
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
   <td colspan="1" rowspan="1"><p><strong>ディメンション</strong></p></td>
   <td colspan="1" rowspan="1"><p><strong>説明</strong></p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>コスト年</p></td>
   <td colspan="1" rowspan="1"><p>プログラムコスト期間</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>コスト四半期</p></td>
   <td colspan="1" rowspan="1"><p>プログラムコスト期間</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>コスト月</p></td>
   <td colspan="1" rowspan="1"><p>プログラムコスト期間</p></td>
  </tr>
 </tbody>
</table>

**ステージメンバーシップ**

<table>
 <tbody>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>測定</strong></p></td>
   <td colspan="1" rowspan="1"><p><strong>説明</strong></p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>モデルはアクティブか</p></td>
   <td colspan="1" rowspan="1"><p>現在モデルが承認済みでアクティブかどうかを示します。</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>ステージはアクティブか</p></td>
   <td colspan="1" rowspan="1"><p>ステージがアクティブかどうかを示します。</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>成功パス上</p></td>
   <td colspan="1" rowspan="1"><p>ステージが成功パス上にあるかどうかを説明します</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>新しい名前あたりのコスト</p></td>
   <td colspan="1" rowspan="1"><p>ステージに到達した新しい名前の平均コスト</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>新しい名前（現在）</p></td>
   <td colspan="1" rowspan="1"><p>現在ステージに存在し、プログラムによって取得されたリードの合計数を示します。</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>新しい名前（かつて）</p></td>
   <td colspan="1" rowspan="1"><p>各ステージが在庫、SLA、またはゲートのどのタイプに分類されるかを説明します。</p></td>
  </tr>
 </tbody>
</table>
