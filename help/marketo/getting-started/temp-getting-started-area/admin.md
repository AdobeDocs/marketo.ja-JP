---
description: 新しい領域 — Marketoドキュメント — 製品ドキュメント
title: 新しい領域
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 7d8cdb2da42769ee0326a3d585ad32a3405dfac1
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 9%

---

# 新しい領域：管理チェックリスト {#new-area-admin-checklist}

概要テキスト。

## ロール {#roles}

<table>
<thead>
  <tr>
    <th>エリア </th>
    <th>アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>ロール </td>
    <td><li>事前に作成された役割を確認し、各役割に割り当てられている権限/アクセスを確認します。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role">新しいロールを作成</a> または <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role">役割の編集</a> 組織のニーズとユーザーのログイン頻度に応じて異なります。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#assign-roles-to-a-user">適切な役割へのユーザーの割り当て</a>.</li>
    <li>ユーザーの役割を割り当てた後で、役割ごとのユーザー数を確認します。</li>  <li>トラブルシューティングを容易におこなえるよう、各 API ユーザーに固有の役割を実装します。</li></td>
  </tr>
  <tr>
    <td>ドキュメント </td>
    <td>組織のユーザーと役割を定義します。 <br>新しいユーザー/管理者を追加するプロセスを定義します。 </td>
  </tr>
  <tr>
    <td>サンドボックス（該当する場合） </td>
    <td>サンドボックスにカテゴリがある場合は、そのカテゴリを確認します。 </td>
  </tr>
</tbody>
</table>

## ワークスペースとパーティション {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th>エリア</th>
    <th>アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>ワークスペースとパーティション </td>
    <td><li>次の数を決定：<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html"> workspaces</a> 組織が必要とするおよび/またはパーティション <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html">各ワークスペースにアクセスできるユーザーの数。</a></li>
    <li>各ワークスペースとパーティションの主な目的を定義します。</li>
    <li>ワークスペースとパーティション間の関係を定義します。</li></td>
  </tr>
  <tr>
    <td>ドキュメント </td>
    <td><li>ワークスペースの定義方法と、それがデータベースパーティション（すなわち全員を表示するグローバルワークスペースとビジネスセクター）にどのように関連しているかを文書化します。</li>
    <li>適切なパーティションに新しいレコードをインポートします。</li>
    <li>ユーザーを適切なパーティションに配置する CRM で値を定義します。</li></td>
  </tr>
</tbody>
</table>

## スマートキャンペーン設定 {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th>エリア</th>
    <th>アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>スマートキャンペーン設定 </td>
    <td><li>を追加します。 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html">スマートキャンペーンサイズの制限</a>：データベース全体に誤って電子メールを送信するのを防ぎます。</li>
    <li>スマートキャンペーンの担当者制限の有効化</li></td>
  </tr>
</tbody>
</table>

## メール設定 {#email-settings}

<table>
<thead>
  <tr>
    <th>エリア</th>
    <th>アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>電子メールのデフォルト</td>
    <td><li>「ブランディングドメイン」で、ドメインを選択し、E メール CNAME を追加します。 これは、[EmailTrackingCNAME] の形式で記述する必要があります。[CompanyDomain].com</li></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html">SPF および DKIM の設定</a> （e メールの配信品質）。</li></td>
  </tr>
</tbody>
</table>

## 通信制限 {#communication-limits}

<table>
<thead>
  <tr>
    <th>エリア</th>
    <th>アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>通信制限</td>
    <td><li>場所 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html">通信制限</a>.</li>
    <li>ビジネスで通信制限に関するポリシーが必要かどうかを判断します。</li></td>
  </tr>
</tbody>
</table>

## タグ {#tags}

<table>
<thead>
  <tr>
    <th>エリア</th>
    <th>アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>チャネル</td>
    <td><li>使用方法の定義 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html">channels</a>.</li></td>
  </tr>
  <tr>
    <td>タグ </td>
    <td><li>使用方法の定義 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">タグ</a>.</li></td>
  </tr>
  <tr>
    <td>カレンダー（該当する場合） </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html">マーケティングカレンダーシートの発行</a> アクセスを必要とするユーザーに対して</li> 
    <li>設定 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">カレンダー</a>.</li></td>
  </tr>
</tbody>
</table>

## データベース管理 {#database-management}

<table>
<thead>
  <tr>
    <th>エリア</th>
    <th>アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>フィールド管理</td>
    <td><li>の命名規則を実装します。 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank" rel="noopener noreferrer">カスタムフィールド。</a> 例えば、「MKTO」で始まります。</li>
    <li>同期するフィールドを選択してください。 同期するフィールドが多いほど、同期サイクルが遅くなります。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank" rel="noopener noreferrer">フィールドの更新をブロックする</a> 1 回だけ書き込む（元のリードソース、元のリードソースの詳細、ファーストタッチ UTM フィールドなど）</li></td>
  </tr>
  <tr>
    <td>カスタムアクティビティ </td>
    <td><li>定義 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html" target="_blank" rel="noopener noreferrer">カスタムアクティビティ</a> お客様のビジネスに固有の</li></td>
  </tr>
  <tr>
    <td>カスタムオブジェクト </td>
    <td><li>レビューする数 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html" target="_blank" rel="noopener noreferrer">カスタムオブジェクト</a> 必要です。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html" target="_blank" rel="noopener noreferrer">これらのカスタムオブジェクトを CRM に同期</a>.</li></td>
  </tr>
</tbody>
</table>

## 統合 {#integrations}

<table>
<thead>
  <tr>
    <th>エリア</th>
    <th>アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM</td>
    <td><li>CRM 同期を開始します。 会社が使用している CRM に応じて、次の中から選択します。 <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html" target="_blank" rel="noopener noreferrer">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html" target="_blank" rel="noopener noreferrer">Microsoft Dynamics</a>.</li>
    <li>CRM にアクセスするために必要なアクセスのタイプを特定します。</li>
    <li>トラブルシューティング用の CRM 管理者を特定します。</li></td>
  </tr>
  <tr>
    <td>Sales Insight（該当する場合）</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html" target="_blank" rel="noopener noreferrer">Sales Insight を設定します。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions" target="_blank" rel="noopener noreferrer">適切なユーザーにシートを発行します。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html" target="_blank" rel="noopener noreferrer">API の設定</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html" target="_blank" rel="noopener noreferrer">リードスコアをカスタマイズします。</a></li></td>
  </tr>
</tbody>
</table>
