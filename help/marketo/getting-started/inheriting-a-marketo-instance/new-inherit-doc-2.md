---
description: ドキュメントを継承 2 - Marketoドキュメント — 製品ドキュメント
title: ドキュメント 2 を継承
hide: true
hidefromtoc: true
source-git-commit: 77314760bfd188725440311f3dc9da2005488ee5
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 8%

---

# 監査データベースチェックリスト {#inherit-doc-2}

サブスクリプションでの人数、マーケティング可能な人数、トップの人物獲得ソースの合計数を把握します。

## システム スマート リスト {#system-smart-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">エリア</th> 
   <th>レビューフォーカス</th>
  </tr> 
  <tr> 
   <td>すべてのリード</td> 
   <td><li>には何人のユーザーが存在しますか？ <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md" target="_blank">データベース</a>?</li>
<li>データベース容量がほぼ満杯に近い場合、会社のポリシーでは、データベースサイズの拡大や履歴データの消去を推奨していますか？</li>
<li>全体的なデータベースは 85%以上の市場で利用できますか？ 
<br/>     お使いのシステムがこのしきい値に該当する場合は、他のシステムスマートリスト (ブロックリストに加える、マーケティングを中断した、重複、配信停止 ) を詳細に調べてください。</li></td>
  </tr>
  <tr> 
   <td>登録解除済みのリード</td> 
   <td><li>の条件 <a href="/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md#marketing-suspended" target="_blank">配信停止済みの担当者</a>? 配信停止済みの担当者が多すぎますか？</li>
<li>登録解除の方法は、データのプライバシー要件と一致していますか？</li>
<li>配信停止の設定は最新の状態ですか？ レコードは、どのくらいの期間、データベース内にマーケティング対象外として残っていますか？</li></td>
  </tr>
  <tr> 
   <td>マーケティングを中断したリード</td> 
   <td><li>の条件 <a href="/help/marketo/product-docs/email-marketing/deliverability/durable-unsubscribe.md#marketing-suspended" target="_blank">マーケティング中断</a>? マーケティングが中断されている担当者が多すぎますか？</li>
<li>レコードが「マーケティングの中断」ステータスのままの期間はどれくらいですか？</li>
<p>マーケティングの中断の使用例：マーケティングコミュニケーションを抑制したい最後の段階の商談で、販売に積極的に関与している人物レコード。</td>
  </tr>
   <tr> 
   <td>ブロックリスト</td> 
   <td><li>の条件 <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md" target="_blank">レコードブロックリストに加えるの</a>? 人が多すぎまブロックリストに加えるすか？</li></td>
  </tr>
  <tr> 
   <td>バウンスメールアドレス</td> 
   <td><li>KG — 配信品質の待機中</li></td>
  </tr>
  <tr> 
   <td>重複の可能性</td> 
   <td><li>数 <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md" target="_blank">重複レコードの可能性がある</a> いるの？
   <br/>     削除またはマージを検討してください。</li></td>
  </tr>
   <tr> 
   <td>獲得プログラムなし</td> 
   <td><li>割り当てられていないユーザーの数 <a href="/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md#acquisition-program" target="_blank">獲得プログラム</a>?
   <br/>     多くの場合は、理由を調べることを検討します。</li></td>
  </tr>
 </tbody> 
</table>

## スマートリスト {#smart-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">エリア</th> 
   <th>レビューフォーカス</th>
  </tr> 
  <tr> 
   <td>スマートリスト</td> 
   <td><li>数 <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md" target="_blank">スマートリスト</a> いるの？ このインスタンスでの使用方法</li>
<li>リストは、まとまったフォルダ構造で整理されていますか？ 
<br/>     孤立したリストがある場合は、アセットを見つけやすくするためにツリーを整理することを検討します。</li>
<p><img src="assets/tip-icon.png" alt="ヒントアイコン">ヒント： <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md#archive-a-folder" target="_blank">アーカイブ</a> 不要になったスマートリストは、組織とパフォーマンスに役立ちます。</td>
  </tr>
 </tbody> 
</table>

## 静的リスト {#static-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">エリア</th> 
   <th>レビューフォーカス</th>
  </tr> 
  <tr> 
   <td>静的リスト</td> 
   <td><li>数 <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/understanding-static-lists.md" target="_blank">静的リスト</a> いるの？ このインスタンスでの使用方法</li></td>
  </tr>
 </tbody> 
</table>

## セグメンテーション {#segmentations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">エリア</th> 
   <th>レビューフォーカス</th>
  </tr> 
  <tr> 
   <td>セグメンテーション</td> 
   <td><li>対象 <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md" target="_blank">セグメント化</a> いるの？ どのように使用されていますか？</li>
<li>の担当者が多すぎます <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md" target="_blank">デフォルトセグメント</a>?</li>
<li>マーケティング可能なオーディエンスのセグメント化はありますか？ 
<br/>     そうでない場合は、作成することを検討してください。</li></td>
  </tr>
 </tbody> 
</table>

<br> 

[◄継承されたインスタンスの監査：管理者](/help/marketo/getting-started/inheriting-a-marketo-instance/new-inherit-doc-1.md)

[継承されたインスタンスの監査：マーケティングアクティビティ►](/help/marketo/getting-started/inheriting-a-marketo-instance/new-inherit-doc-3.md)
