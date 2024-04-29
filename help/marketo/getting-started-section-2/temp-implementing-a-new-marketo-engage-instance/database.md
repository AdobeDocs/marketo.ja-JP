---
description: 新しい Marketo Engage インスタンスの「データベース」セクションを設定します。
title: 新しい領域のデータベース
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: 1966bc6f-9384-4c51-b3aa-57d5e52781f1
source-git-commit: 8473c4d59210bb18c3968a56883034febf00c320
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 53%

---

# 新しい領域：データベースチェックリスト {#new-area-database-checklist}

新しい Marketo Engage インスタンスの「データベース」セクションに必要な手順を実装する方法について説明します。「新しいインスタンスの実装」ガイドに従って、進行中のタスクを追跡し、長期的な効率を実現するインスタンスの設定に役立ちます。

## システムスマートリスト {#system-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>すべてのユーザ</td>
    <td><li>CRM との 1 対 1 の同期を実装するか、フィルターを適用してシステム間およびシステム間を移動するユーザーを制限するかを決定します。</li> 
    <li>の担当者とマーケティング可能な担当者の合計数を確認します <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html?lang=ja" target="_blank">Marketo Engageデータベース</a>.</li></td>
  </tr>
  <tr>
    <td>ブロックリスト</td>
    <td><li>ブロックリストの条件を定義します。競合他社のドメインをに追加することを検討します <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html?lang=ja" target="_blank">ブロックリスト</a> を設定して、メールが受信者に届かないようにします。</li></td>
  </tr>
  <tr>
    <td>マーケティング中断</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html?lang=ja#marketing-suspended" target="_blank">マーケティング中断</a>の条件を定義します。</li></td>
  </tr>
  <tr>
    <td>バウンスしたメールアドレス </td>
    <td><li>バウンスメールアドレスの条件を定義します。</li>
    <li>「メール無効」カテゴリの人物と、メールが必要かどうかを確認します <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html?lang=ja" target="_blank">手動でリセット</a>.</li></td>
  </tr>
  <tr>
    <td>重複の可能性</td>
    <td><li>重複の可能性のあるリスト内の人物を確認します。</li> 
    <li>重複管理戦略を定義し、次の操作を実行するかどうかを決定します <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html?lang=ja" target="_blank">ユーザーを手動で結合</a>.</li>  
    <li>CRM 統合がある場合、のプロセスとアカウントを定義します <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html?lang=ja#effect-in-salesforce" target="_blank">crm でのリードの結合の効果</a>.</li></td>
  </tr>
  <tr>
    <td>獲得プログラムなし</td>
    <td><li>特にグローバルフォームを使用する場合は、獲得プログラムを設定するキャンペーンをプログラムテンプレートに確立します。</li></td>
  </tr>
  <tr>
    <td>登録解除済みのユーザ</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html?lang=ja" target="_blank">登録解除済みの人物</a>の基準を確認します。</li></td>
  </tr>
</tbody>
</table>

## グループスマートリスト {#group-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>グループスマートリスト</td>
    <td><li>リストが重複しないように、グループスマートリストの作成に注意してください。</li>
    <li>データベース内のマスターリストを追跡します。</li></td>
  </tr>
</tbody>
</table>

## セグメント化 {#segmentation}

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>セグメント化</td>
    <td><li>ビジネスニーズに基づいて<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html?lang=ja" target="_blank">セグメント化を作成</a>します。各サブスクリプションは、20 個のセグメント化と、各セグメント化内の 100 個のセグメントに制限されます。</li></td>
  </tr>
</tbody>
</table>
