---
description: ドキュメントを継承 2 - Marketoドキュメント — 製品ドキュメント
title: ドキュメント 2 を継承
hide: true
hidefromtoc: true
source-git-commit: 4b726947bfaf9f8e4dcf48076e1148124fb46d25
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 9%

---

# ドキュメント 2 を継承 {#inherit-doc-2}

別の管理者から既存のMarketo Engageインスタンスを継承したか。 その場合は、この記事があなたのためのものです。

>[!TIP]
>
>新規のMarketo Engageユーザーで、多くの用語に精通していない場合は、 [Marketo用語集](/help/marketo/getting-started/marketo-glossary.md){target="_blank"}.

## システム スマート リスト {#system-smart-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>エリア</th> 
   <th>レビューフォーカス</th>
  </tr> 
  <tr> 
   <td>すべてのリード</td> 
   <td><li>には何人のユーザーが存在しますか？ <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md" target="_blank">データベース</a>?</li>
<li>データベース容量がほぼ満杯に近い場合、会社のポリシーでは、データベースサイズの拡大や履歴データの消去を推奨していますか？</li>
<li>全体的なデータベースは 85%以上の市場で利用できますか？ 
<br/>お使いのシステムがこのしきい値に該当する場合は、他のシステムスマートリスト (ブロックリストに加える、マーケティングを中断した、重複、配信停止 ) を詳細に調べてください。</li></td>
  </tr>
  <tr> 
   <td>登録解除済みのリード</td> 
   <td><li>の条件 <a href="/help/marketo/product-docs/email-marketing/deliverability/durable-unsubscribe.md" target="_blank">配信停止済みの担当者</a>? 配信停止済みの担当者が多すぎますか？</li>
<li>登録解除の方法は、データのプライバシー要件と一致していますか？</li>
<li>配信停止の設定は最新の状態ですか？ レコードは、どのくらいの期間、データベース内にマーケティング対象外として残っていますか？</li></td>
  </tr>
  <tr> 
   <td>マーケティングを中断したリード</td> 
   <td><li>の条件 <a href="/help/marketo/product-docs/email-marketing/deliverability/durable-unsubscribe.md#marketing-suspended" target="_blank">マーケティング中断</a>? マーケティングが中断されている担当者が多すぎますか？</li>
<li>レコードが「マーケティングの中断」ステータスのままの期間はどれくらいですか？</li>
<p>マーケティングの中断の使用例：マーケティングコミュニケーションを抑制したい最後の段階での商談の販売に積極的に関与しているレコード。</td>
  </tr>
   <tr> 
   <td>ブロックリスト</td> 
   <td><li>の条件 <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md" target="_blank">レコードブロックリストに加えるの</a>? 人が多すぎまブロックリストに加えるすか？</li></td>
  </tr>
  <tr> 
   <td>バウンスメールアドレス</td> 
   <td><li>テキスト</li></td>
  </tr>
  <tr> 
   <td>重複の可能性</td> 
   <td><li>数 <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md" target="_blank">重複レコードの可能性がある</a> いるの？
   <br/>削除またはマージを検討してください。</li></td>
  </tr>
   <tr> 
   <td>獲得プログラムなし</td> 
   <td><li>割り当てられていないユーザーの数 <a href="/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md#acquisition-program" target="_blank">獲得プログラム</a>?
   <br/>多くの場合は、理由を調べることを検討します。</li></td>
  </tr>
 </tbody> 
</table>

## グループ スマート リスト {#group-smart-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>エリア</th> 
   <th>レビューフォーカス</th>
  </tr> 
  <tr> 
   <td>グループ スマート リスト</td> 
   <td><li>スマートリストのグループはどれですか？ このインスタンスでの使用方法</li>
<li>リストは、まとまったフォルダ構造で整理されていますか？ <br/>孤立したリストがある場合は、アセットを見つけやすくするためにツリーを整理することを検討します。</li>
<p>ヒント： <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md#archive-a-folder" target="_blank">アーカイブ</a> 組織とパフォーマンスの問い合わせ、レポート、または参照に不要になったグループスマートリスト。</td>
  </tr>
 </tbody> 
</table>

## グループ リスト {#group-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>エリア</th> 
   <th>レビューフォーカス</th>
  </tr> 
  <tr> 
   <td>グループ リスト</td> 
   <td><li>どのグループリストがありますか？</li>
<li>このインスタンスでの使用方法</li></td>
  </tr>
 </tbody> 
</table>

## セグメンテーション {#segmentations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>エリア</th> 
   <th>レビューフォーカス</th>
  </tr> 
  <tr> 
   <td>セグメンテーション</td> 
   <td><li>対象 <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md" target="_blank">セグメント化</a> いるの？ どのように使用されていますか？</li>
<li>人が多すぎますか？ <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md" target="_blank">デフォルトセグメント</a>?</li>
<li>マーケティング可能なオーディエンスのセグメント化はありますか？ 
<br/>そうでない場合は、作成することを検討してください。</li></td>
  </tr>
 </tbody> 
</table>
