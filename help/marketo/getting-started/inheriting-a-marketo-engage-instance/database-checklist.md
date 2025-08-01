---
description: 継承インスタンスデータベースのチェックリスト - Marketo ドキュメント - 製品ドキュメント
title: 継承インスタンスデータベースのチェックリスト
feature: Getting Started
exl-id: 278a6a2f-7b68-4003-8727-129e0dc96c12
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 94%

---

# 継承インスタンス：データベースのチェックリスト {#inherited-instance-database-checklist}

サブスクリプションでのユーザ、市場価値の高いユーザ、トップのユーザ獲得ソースの合計数を把握します。忘れずに[チェックリストをダウンロード](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx)し、進捗状況を追跡してください。

## システムスマートリスト {#system-smart-lists}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">エリア</th>
   <th>レビューフォーカス</th>
  </tr>
  <tr>
   <td>すべてのユーザ</td>
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md" target="_blank">データベース</a>に存在するユーザは何人ですか？</li>
<li>データベース容量がほぼいっぱいの場合、会社のポリシーではデータベースのサイズを拡張するか、履歴データを消去することが推奨されていますか？</li>
<li>データベース全体で少なくとも 85% はマーケティング可能ですか？
<br/>     お使いのシステムがこのしきい値に該当する場合は、他のシステムスマートリスト（ブロックリスト、マーケティングの中断、重複、登録解除）を詳細に調べてください。</li></td>
  </tr>
  <tr>
   <td>登録解除済みのユーザ</td>
   <td><li><a href="/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md#marketing-suspended" target="_blank">登録解除済みのユーザ</a>の条件は何ですか？登録解除済みのユーザが多すぎますか？</li>
<li>登録解除の方法は、データプライバシー要件に合致していますか？</li>
<li>登録解除の設定は最新ですか？市場価値のないレコードは、どのくらいの期間、データベース内に残っていますか？</li></td>
  </tr>
  <tr>
   <td>マーケティング中断</td>
   <td><li><a href="/help/marketo/product-docs/email-marketing/deliverability/durable-unsubscribe.md#marketing-suspended" target="_blank">マーケティング中断</a>の条件は何ですか？マーケティングを中断されているユーザが多すぎますか？</li>
<li>レコードが「マーケティング中断」ステータスのままになっている期間はどのくらいですか？</li>
<p>マーケティング中断のユースケース例：マーケティングコミュニケーションを抑制したい最終段階の商談で営業に積極的に関与しているユーザのレコード。</td>
  </tr>
   <tr>
   <td>ブロックリスト</td>
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md" target="_blank">レコードのブロックリストへの登録</a>の条件は何ですか？ブロックリストに登録するユーザが多すぎますか？</li></td>
  </tr>
  <tr>
   <td>バウンスしたメールアドレス</td>
   <td><li>データベースには、<a href="/help/marketo/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.md" target="_blank">バウンスしたユーザ</a>が多数いますか？
   <br/>     その場合は、理由の調査を検討してください。</li></td></li></td>
  </tr>
  <tr>
   <td>重複の可能性</td>
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md" target="_blank">重複する可能性のあるレコード</a>はいくつありますか？
   <br/>     削除またはマージを検討してください。</li></td>
  </tr>
   <tr>
   <td>獲得プログラムなし</td>
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md#acquisition-program" target="_blank">獲得プログラム</a>を持っていない人は何人いますか？
   <br/>     多数いる場合は、理由の調査を検討してください。</li></td>
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
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md" target="_blank">スマートリスト</a>はいくつありますか？それらは、このインスタンスでどのように使用されていますか？</li>
   <p><img src="assets/note-icon.png" alt="メモアイコン"> メモ：「データベース」セクションで、グループスマートリストはユーザが生成するもので、システムスマートリストは Marketo Engage が作成するデフォルトのリストです。
<li>リストはまとまりのあるフォルダー構造で整理されていますか？
<br/>     孤立リストがある場合は、アセットを見つけやすいようにツリーを整理することを検討してください。</li>
<p><img src="assets/tip-icon.png" alt="ヒントアイコン">ヒント：不要になったスマートリストを<a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md#archive-a-folder" target="_blank">アーカイブ</a>すると、整理とパフォーマンスに役立ちます。</td>
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
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/understanding-static-lists.md" target="_blank">静的リスト</a>はいくつありますか？それらは、このインスタンスでどのように使用されていますか？</li>
   <p><img src="assets/note-icon.png" alt="メモアイコン"> メモ：「データベース」セクションで、グループリストは静的リストです。</td>
  </tr>
 </tbody>
</table>

## セグメント化 {#segmentations}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">エリア</th>
   <th>レビューフォーカス</th>
  </tr>
  <tr>
   <td>セグメント化</td>
   <td><li>どの<a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md" target="_blank">セグメント化</a>がありますか？どのように使用されていますか？</li>
<li><a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md" target="_blank">デフォルトセグメント</a>にいるユーザが多すぎますか？</li>
<li>マーケティング可能なオーディエンスに対するセグメント化はありますか？
<br/>     設定していない場合は、新たに設定することを検討してください。</li></td>
  </tr>
 </tbody>
</table>
