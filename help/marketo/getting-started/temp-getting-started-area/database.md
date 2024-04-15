---
description: 新しい Marketo Engage インスタンスの「データベース」セクションを設定します。
title: 新しい領域のデータベース
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: 1966bc6f-9384-4c51-b3aa-57d5e52781f1
source-git-commit: dae00c6877e638ae60305122f3f3e17b3c922e10
workflow-type: ht
source-wordcount: '296'
ht-degree: 100%

---

# 新しい領域：データベースチェックリスト {#new-area-database-checklist}

新しい Marketo Engage インスタンスの「データベース」セクションに必要な手順を実装する方法について説明します。「新しいインスタンスの実装」ガイドに従って、進行中のタスクを追跡し、長期的な効率を実現するインスタンスの設定に役立ちます。

## システムスマートリスト {#system-smart-lists}

<table>
<thead>
  <tr>
    <th>エリア</th>
    <th>アクション項目</th>
    <th>優先度</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>すべてのユーザ</td>
    <td><li>CRM との1 対 1 の同期を実装するか、システム間を移動する人物とタイミングを制限するフィルターを適用するかを決定します。</li> 
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html?lang=ja" target="_blank" rel="noopener noreferrer">データベース</a>内の人物とマーケティング可能な人物の合計数を確認します。</li></td>
    <td>テキスト</td>
  </tr>
  <tr>
    <td>ブロックリスト</td>
    <td><li>ブロックリストの条件を定義します。競合他社のドメインを<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html?lang=ja" target="_blank" rel="noopener noreferrer">ブロックリスト</a>に追加して、マーケティングメールやオペレーショナルメールを受信できないようにすることを考慮します。</li></td>
    <td>テキスト</td>
  </tr>
  <tr>
    <td>マーケティング中断</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html?lang=ja#marketing-suspended" target="_blank" rel="noopener noreferrer">マーケティング中断</a>の条件を定義します。</li></td>
    <td>テキスト</td>
  </tr>
  <tr>
    <td>バウンスしたメールアドレス </td>
    <td><li>バウンスメールアドレスの条件を定義します。</li>
    <li>「メールが無効です」カテゴリにある人物を確認し、メールを<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html?lang=ja" target="_blank" rel="noopener noreferrer">手動でリセット</a>する必要があるかどうかを確認します。</li></td>
    <td>テキスト</td>
  </tr>
  <tr>
    <td>重複の可能性</td>
    <td><li>重複の可能性のあるリスト内の人物を確認します。</li> 
    <li>重複管理戦略を定義して、<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html?lang=ja" target="_blank" rel="noopener noreferrer">人物を手動で結合</a>するかどうかを決定します。</li>  
    <li>CRM 統合を行っている場合は、プロセスを定義し、<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html?lang=ja#effect-in-salesforce" target="_blank" rel="noopener noreferrer">CRM でリードを結合する効果</a>を考慮する必要があります。</li></td>
    <td>テキスト</td>
  </tr>
  <tr>
    <td>獲得プログラムなし</td>
    <td><li>特にグローバルフォームを使用している場合は、獲得プログラムを設定するプログラムテンプレートでキャンペーンを確立します。</li></td>
    <td>テキスト</td>
  </tr>
  <tr>
    <td>登録解除済みのユーザ</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html?lang=ja" target="_blank" rel="noopener noreferrer">登録解除済みの人物</a>の基準を確認します。</li></td>
    <td>テキスト</td>
  </tr>
</tbody>
</table>

## グループスマートリスト {#group-smart-lists}

<table>
<thead>
  <tr>
    <th>エリア</th>
    <th>アクション項目</th>
    <th>優先度</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>グループスマートリスト</td>
    <td><li>リストが重複しないように、グループスマートリストの作成に注意してください。</li>
    <li>ここのデータベースでメインリストを追跡します。</li></td>
    <td>テキスト</td>
  </tr>
</tbody>
</table>

## セグメント化 {#segmentation}

<table>
<thead>
  <tr>
    <th>エリア</th>
    <th>アクション項目</th>
    <th>優先度</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>セグメント化</td>
    <td><li>ビジネスニーズに基づいて<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html?lang=ja" target="_blank" rel="noopener noreferrer">セグメント化を作成</a>します。各サブスクリプションは、20 個のセグメント化と、各セグメント化内の 100 個のセグメントに制限されます。</li></td>
    <td>テキスト</td>
  </tr>
</tbody>
</table>
