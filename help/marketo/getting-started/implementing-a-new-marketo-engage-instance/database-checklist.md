---
description: 新しいMarketo Engageインスタンスにデータベース セクションを設定します。
title: 新しいインスタンスのベストプラクティス – データベースチェックリスト
feature: Getting Started
exl-id: 996ea2db-a00c-48e5-97a8-00f869c261b1
source-git-commit: df8087dbaf2b621d0d877eba1c16f160ee9bf460
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 70%

---

# 新しいインスタンスのベストプラクティス：データベースのチェックリスト {#new-instance-best-practices-database-checklist}

「データベース」セクションには、インスタンス内のユーザーの主要な属性が表示されます。 データベース内の様々なリストやセグメント間を移動するために必要な手順、および人物レコードの管理について説明します。

忘れずに[チェックリストをダウンロード](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx)し、進捗状況を追跡してください。

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
    <td><li>CRM との1 対 1 の同期を実装するか、システム間を移動する人物とタイミングを制限するフィルターを適用するかを決定します。</li> 
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html?lang=ja" target="_blank">Marketo Engage データベース</a>内の人物とマーケティング可能な人物の合計数を確認します。</li></td>
  </tr>
  <tr>
    <td>ブロックリスト</td>
    <td><li>ブロックリストの条件を定義します。競合他社のドメインを <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html?lang=ja" target="_blank">ブロックリスト</a> に追加して、競合他社がメールを受信するのを防ぐことを検討します。</li></td>
  </tr>
  <tr>
    <td>マーケティング中断</td>
    <td><li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe#marketing-suspended" target="_blank">マーケティング中断</a>の条件を定義します。</li></td>
  </tr>
  <tr>
    <td>バウンスしたメールアドレス </td>
    <td><li>バウンスメールアドレスの条件を定義します。</li>
    <li>「無効なメール」カテゴリの人物を確認し、メールが <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html?lang=ja" target="_blank"> 手動でのリセット </a> 必要かどうかを判断します。</li></td>
  </tr>
  <tr>
    <td>重複の可能性</td>
    <td><li>重複の可能性のあるリスト内の人物を確認します。</li> 
    <li>重複管理戦略を定義して、<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html?lang=ja" target="_blank">人物を手動で統合</a>するかどうかを決定します。</li>  
    <li>CRM 統合を行っている場合は、プロセスを定義し、<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people#effect-in-salesforce" target="_blank">CRM でリードを結合する効果</a>を考慮します。</li></td>
  </tr>
  <tr>
    <td>獲得プログラムなし</td>
    <td><li>特にグローバルフォームを使用している場合は、獲得プログラムを設定するプログラムテンプレートでキャンペーンを確立します。</li></td>
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
    <li>データベースでメインリストを追跡します。</li></td>
  </tr>
</tbody>
</table>

## セグメント化 {#segmentation}

<table>
<thead>
  <tr>
    <th style="width:21%">エリア</th>
    <th style="width:79%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>セグメント化</td>
    <td><li>ビジネスニーズに基づいて<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html?lang=ja" target="_blank">セグメント化を作成</a>します。各サブスクリプションは、20 個のセグメント化と、各セグメント化内の 100 個のセグメントに制限されます。</li></td>
  </tr>
</tbody>
</table>
