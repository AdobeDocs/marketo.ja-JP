---
description: 新しいMarketo Engageインスタンスの「管理者」セクションを設定します。
title: 新しいインスタンスのベストプラクティス – 「管理者」セクションのチェックリスト
feature: Getting Started
exl-id: 4fa90a32-7e97-404c-90b1-90d05c2561d0
source-git-commit: df8087dbaf2b621d0d877eba1c16f160ee9bf460
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 67%

---

# 新しいインスタンスのベストプラクティス：「管理者」セクションのチェックリスト {#new-instance-best-practices-admin-section-checklist}

新しい管理者が新しいMarketo Engageインスタンスに移動する際には、以下のチェックリストを適用すると、実装プロセスを導くことができます。 これらのすべてのガイドと同様に、[ チェックリストをダウンロード ](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) したり、進行状況を追跡したりすることもできます。

## ロール {#roles}

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>ロール</td>
    <td><li>事前に作成されたロールを確認し、各ロールに割り当てられている権限／アクセス権を確認します。</li>
    <li>組織のニーズに基づいて、<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=ja#create-a-new-role" target="_blank">新しいロールを作成</a>または<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=ja#edit-a-role" target="_blank">ロールを編集</a>します。</li>
    <li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user" target="_blank">ユーザを適切なロールに割り当てます</a>。ユーザーは、「ロール」でロールを付与する前に、Adobe Admin Consoleの購読に追加される必要があります。 <a href="/help/marketo/getting-started/initial-setup/user-setup.md"> 初期設定チェックリスト </a> のユーザーの節を参照してください。</li>
    <li>ユーザにロールを割り当てた後、ロールごとのユーザ数を確認します。</li>
    <li>トラブルシューティングを簡単に行うために、各 API ユーザに一意のロールを実装します。</li></td>
  </tr>
  <tr>
    <td>サンドボックス（該当する場合）</td>
    <td><li>お使いの<a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">サンドボックス</a>で上記のカテゴリを確認します。</li></td>
  </tr>
</tbody>
</table>

## ワークスペースとパーティション {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>ワークスペースとパーティション（該当する場合）</td>
    <td><li>組織に必要な<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html?lang=ja" target="_blank">ワークスペース</a>やパーティションの数と、<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html?lang=ja" target="_blank">各ワークスペースにアクセス権があるユーザの数</a>を決定します。</li>
    <li>各ワークスペースとパーティションの主な目的を定義します。</li>
    <li>ワークスペースとパーティションの間の関係を定義します。</li></td>
  </tr>
</tbody>
</table>

## スマートキャンペーン設定 {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>スマートキャンペーン設定</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html?lang=ja" target="_blank">スマートキャンペーンのサイズに関する制限</a>を追加すると、データベース全体に誤ってメールを送信することを防ぎます。</li></td>
  </tr>
</tbody>
</table>

## 通信制限 {#communication-limits}

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>通信制限</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html?lang=ja" target="_blank"> 通信制限 </a> を実装します。</li>
    <li>ビジネスに通信制限に関するポリシーが必要かどうかを判断します。</li></td>
  </tr>
</tbody>
</table>

## タグ {#tags}

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>チャネル</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html?lang=ja" target="_blank">チャネル</a>の使用方法を定義します。</li></td>
  </tr>
  <tr>
    <td>タグ</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html?lang=ja" target="_blank">タグ</a>の使用方法を定義します。</li></td>
  </tr>
  <tr>
    <td>カレンダー <br> 
    （該当する場合）</td>
    <td><li>アクセスを必要とするユーザに対して、<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html?lang=ja" target="_blank">マーケティングカレンダーシートを発行</a>します。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html?lang=ja" target="_blank">カレンダー</a>を設定します。</li></td>
  </tr>
</tbody>
</table>

## データベース管理 {#database-management}

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>フィールド管理</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html?lang=ja" target="_blank">カスタムフィールド</a>の命名規則を実装します（例えば、「MKTO」で始まる）。</li>
    <li>同期するフィールドについては慎重に選択してください。同期するフィールドが多いほど、同期サイクルが遅くなります。</li>
    <li>（元のリードソース、元のリードソースの詳細、ファーストタッチ UTM フィールドなど）1 回書き込む<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html?lang=ja" target="_blank">フィールドへの更新をブロックします</a>。</li></td>
  </tr>
  <tr>
    <td>カスタムアクティビティ</td>
    <td><li>ビジネスに固有の<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html?lang=ja" target="_blank">カスタムアクティビティ</a>を定義します。</li></td>
  </tr>
  <tr>
    <td>カスタムオブジェクト</td>
    <td><li>必要な<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html?lang=ja" target="_blank">カスタムオブジェクト</a>の数を確認します。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html?lang=ja" target="_blank"> これらのカスタムオブジェクトを CRM に同期 </a> します。</li></td>
  </tr>
</tbody>
</table>

## 統合 {#integrations}

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM </td>
    <td><li>CRM へのアクセスに必要な権限を特定します。</li>
    <li>トラブルシューティング用の CRM 管理者を特定します。</li></td>
  </tr>
  <tr>
    <td>Web サービス</td>
    <td><li>インスタンス内で <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html?lang=ja" target="_blank">API 呼び出し</a>を実行できるユーザ／アプリを決定します。</li>
    <li>API 呼び出しを行うすべてのアプリを確認し、API 呼び出しの増減が必要かどうかを判断します。</li></td>
  </tr>
  <tr>
    <td>Launchpoint</td>
    <td><li>ビジネス向けに <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html?lang=ja" target="_blank">LaunchPoint</a> サービスを設定します。トラブルシューティングを支援するために、各 LaunchPoint と一意の API ユーザをペアにする必要があります。</li></td>
  </tr>
  <tr>
    <td>インタラクティブウェビナー（該当する場合）</td>
    <td><li>インタラクティブウェビナーを作成するには、Marketo Engageのビルトインウェビナー機能である <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management" target="_blank"> 「インタラクティブウェビナー」タブの「ユーザー」セクションにユーザーを追加 </a> します。</li>
    <p><img src="assets/note-icon.png" alt="メモアイコン"> メモ：インタラクティブウェビナーは、実稼動インスタンスにのみプロビジョニングされます。</td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat（該当する場合）</td>
    <td><li>Marketo Engage/管理者/Dynamic Chatとロールで、ユーザーを <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role" target="_blank"> アクセスのロール </a> に割り当てます。</li></td>
  </tr>
  <tr>
    <td>Sales Insight（該当する場合）</td>
    <td><li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account" target="_blank">Sales Insight アクションの設定</a>は、Sales Insight／アクション設定で行います。</li>
    <li>適切なユーザーに <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html?lang=ja#invite-individual-users-to-msi-actions" target="_blank"> 問題の席 </a> を割り当てます。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html?lang=ja" target="_blank">API を設定</a>します。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html?lang=ja" target="_blank"> リードスコア </a> をカスタマイズします。</li></td>
  </tr>
  <tr>
    <td>Sales Connect（該当する場合）</td>
    <td><li>適切なMarketo Engage管理者を <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance" target="_blank">Sales Connect インスタンス </a> に招待します。</li>
    <li>Sales Connect と Salesforce で<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins" target="_blank">追加の Sales Connect 管理者設定</a>を完了します。</li></td>
  </tr>
  <tr>
    <td>Web フック（該当する場合）</td>
    <td><li>ビジネスに<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html?lang=ja" target="_blank">必須の Web フックを作成</a>します。</li>
    </td>
  </tr>
</tbody>
</table>

## アイデアスペース {#treasure-chest}

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>アイデアスペース </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html?lang=ja" target="_blank">アイデアスペースを有効</a>にして、パイロット機能を実験します。</li>
    <li>オンまたはオフにする機能を決定します。</li></td>
  </tr>
  <tr>
    <td>キャンペーンインスペクター </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html?lang=ja" target="_blank"> キャンペーンインスペクターをオン </a> にすると、すべてのスマートキャンペーンが 1 か所で表示されます。</li></td>
  </tr>
</tbody>
</table>
