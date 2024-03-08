---
description: 新しい領域 — Marketoドキュメント — 製品ドキュメント
title: 新しい領域
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: d65903d64d068a6f919df78258654414f3b76426
workflow-type: tm+mt
source-wordcount: '985'
ht-degree: 9%

---

# 新しい領域：管理チェックリスト {#new-area-admin-checklist}

概要テキスト。

## ロール {#roles}

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
    <td>ロール</td>
    <td><li>事前に作成された役割を確認し、各役割に割り当てられている権限/アクセスを確認します。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role">新しいロールを作成</a> または <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role">役割の編集</a> 組織のニーズとユーザーのログイン頻度に応じて異なります。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#assign-roles-to-a-user">適切な役割へのユーザーの割り当て</a>.</li>
    <li>ユーザーの役割を割り当てた後で、役割ごとのユーザー数を確認します。</li>  <li>トラブルシューティングを容易におこなえるよう、各 API ユーザーに固有の役割を実装します。</li></td>
    <td></td>
  </tr>
  <tr>
    <td>ドキュメント</td>
    <td>組織のユーザーと役割を定義します。 <br>新しいユーザー/管理者を追加するプロセスを定義します。</td>
    <td></td>
  </tr>
  <tr>
    <td>サンドボックス（該当する場合）</td>
    <td>サンドボックスにカテゴリがある場合は、そのカテゴリを確認します。</td>
    <td></td>
  </tr>
</tbody>
</table>

## ワークスペースとパーティション {#workspaces-partitions}

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
    <td>ワークスペースとパーティション </td>
    <td><li>次の数を決定：<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html"> workspaces</a> 組織が必要とするおよび/またはパーティション <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html">各ワークスペースにアクセスできるユーザーの数。</a></li>
    <li>各ワークスペースとパーティションの主な目的を定義します。</li>
    <li>ワークスペースとパーティション間の関係を定義します。</li></td>
    <td></td>
  </tr>
  <tr>
    <td>ドキュメント</td>
    <td><li>ワークスペースの定義方法と、それがデータベースパーティション（すなわち全員を表示するグローバルワークスペースとビジネスセクター）にどのように関連しているかを文書化します。</li>
    <li>適切なパーティションに新しいレコードをインポートします。</li>
    <li>ユーザーを適切なパーティションに配置する CRM で値を定義します。</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## スマートキャンペーン設定 {#smart-campaign-settings}

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
    <td>スマートキャンペーン設定 </td>
    <td><li>を追加します。 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html">スマートキャンペーンサイズの制限</a>：データベース全体に誤って電子メールを送信するのを防ぎます。</li>
    <li>スマートキャンペーンの担当者制限の有効化</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## メール設定 {#email-settings}

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
    <td>電子メールのデフォルト</td>
    <td><li>「ブランディングドメイン」で、ドメインを選択し、E メール CNAME を追加します。 これは、[EmailTrackingCNAME] の形式で記述する必要があります。[CompanyDomain].com</li></td>
    <td></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html">SPF および DKIM の設定</a> （e メールの配信品質）。</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## 通信制限 {#communication-limits}

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
    <td>通信制限</td>
    <td><li>場所 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html">通信制限</a>.</li>
    <li>ビジネスで通信制限に関するポリシーが必要かどうかを判断します。</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## タグ {#tags}

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
    <td>チャネル</td>
    <td><li>使用方法の定義 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html">channels</a>.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>タグ </td>
    <td><li>使用方法の定義 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">タグ</a>.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>カレンダー（該当する場合） </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html">マーケティングカレンダーシートの発行</a> アクセスを必要とするユーザーに対して</li> 
    <li>設定 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">カレンダー</a>.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## データベース管理 {#database-management}

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
    <td>フィールド管理</td>
    <td><li>の命名規則を実装します。 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank">カスタムフィールド。</a> 例えば、「MKTO」で始まります。</li>
    <li>同期するフィールドを選択してください。 同期するフィールドが多いほど、同期サイクルが遅くなります。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank">フィールドの更新をブロックする</a> 1 回だけ書き込む（元のリードソース、元のリードソースの詳細、ファーストタッチ UTM フィールドなど）</li></td>
    <td></td>
  </tr>
  <tr>
    <td>カスタムアクティビティ </td>
    <td><li>定義 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html" target="_blank">カスタムアクティビティ</a> お客様のビジネスに固有の</li></td>
    <td></td>
  </tr>
  <tr>
    <td>カスタムオブジェクト </td>
    <td><li>レビューする数 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html" target="_blank">カスタムオブジェクト</a> 必要です。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html" target="_blank">これらのカスタムオブジェクトを CRM に同期</a>.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## 統合 {#integrations}

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
    <td>CRM</td>
    <td><li>CRM 同期を開始します。 会社が使用している CRM に応じて、次の中から選択します。 <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html" target="_blank">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html" target="_blank">Microsoft Dynamics</a>.</li>
    <li>CRM にアクセスするために必要なアクセスのタイプを特定します。</li>
    <li>トラブルシューティング用の CRM 管理者を特定します。</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Sales Insight（該当する場合）</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html" target="_blank">Sales Insight を設定します。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions" target="_blank">適切なユーザーにシートを発行します。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html" target="_blank">API の設定</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html" target="_blank">リードスコアをカスタマイズします。</a></li></td>
    <td></td>
  </tr>
  <tr>
    <td>ランディングページ </td>
    <td>注意： Launch Pack をお使いですか？ この手順をスキップできます。キックオフコール中に、IT セットアップ手順書が担当のコンサルタントから提供されます。 <br>ランディングページドメインを <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html" target="_blank">CNAME</a> および <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html" target="_blank">ドメインとページの情報を入力</a>. これは、[LandingPageCNAME] の形式で記述する必要があります。[CompanyDomain].com <br>ランディングページの CNAME を選択します。 次に例を示します。 <br>* **go**.[CompanyDomain].com <br>* **www2**.[CompanyDomain].com <br>* **lp**.[CompanyDomain].com <br>ヒント：短くしてください。 URL は短いほど覚えやすくなります。ドメインには「go」を指定することをお勧めします。 <br>ランディングページテンプレートに Analytics トラッキングコード (Google Analytics、Adobe Analyticsなど ) を追加します。 </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Edit+Landing+Page+Settings">ランディングページ設定の編集</a></td>
  </tr>
  <tr>
    <td rowspan="2">Munchkin </td>
    <td rowspan="2">注意： Launch Pack をご利用のお客様は、この手順をスキップしてください。 担当のコンサルタントが、IT セットアップ手順ドキュメントに Munchkin のコード手順を提供します。 <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.html" target="_blank">Munchkin トラッキングコードの追加</a> を web サイトに追加します。 Munchkin コードは、 <a href="https://developers.marketo.com/javascript-api/lead-tracking/" target="_blank">ハードコードされた</a> またはGoogle Tag Manager を使用してデプロイされます。</td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Add+Munchkin+Tracking+Code+to+Your+Website">Web サイトへの Munchkin 追跡コードの追加</a> </td>
  </tr>
  <tr>
    <td><a href="https://developers.marketo.com/javascript-api/lead-tracking/">リードトラッキング</a> </td>
  </tr>
  <tr>
    <td>Web サービス </td>
    <td>有効にする <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html" target="_blank">IP 制限</a> 該当する場合は。 <br>作成可能なユーザー/アプリを決定 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html" target="_blank">API 呼び出し</a> インスタンス内で使用できます。 <br>API 呼び出しをおこなうすべてのアプリを確認し、API 呼び出しに増やしや切り取りが必要かどうかを判断します。</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html#product-docs">IP ベー許可リストに加えるスの API アクセス用のの作成 </a> </td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat（該当する場合） </td>
    <td>を使用する場合 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html" target="_blank">Dynamic Chat</a>、Marketo Engageのネイティブ対話型エンゲージメントチャネル、次の手順に従って、ユーザー権限の設定に進みます： <a href="https://adminconsole.adobe.com/" target="_blank">Adobe Admin Console</a>. <br> <br>Adobe組織システム管理者からAdobe製品管理者の役割が付与されているかどうかを確認します。 連絡先 <a href="https://helpx.adobe.com/contact.html" target="_blank">Adobeカスタマーケア</a><a href="https://helpx.adobe.com/contact.html)." target="_blank">https://helpx.adobe.com/contact.html</a> をクリックして、組織内で誰がコンソールの管理者権限を持っているかを確認します。 <br>確定 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html" target="_blank">「Dynamic Chat製品管理者」招待</a>. The <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html" target="_blank">お知らせメール</a> は、Marketo EngageインスタンスでDynamic Chatが有効になっていて、システム管理者に指定されている場合に送信されます。  <br>Adobe Admin Consoleの製品プロファイルに、すべての適切なMarketo Engageを割り当てます。 <br>製品プロファイルに追加する前に、Marketo Engage/管理者/ユーザーとロールでユーザーのロールを割り当てることはできません。  <br>望ましくないユーザーが複数の製品プロファイルに追加された場合は、すべての製品プロファイルからそのユーザーを削除する必要があります。 そうしないと、ユーザーは引き続きDynamic Chatにアクセスできます。 </td>
    <td> </td>
  </tr>
  <tr>
    <td>Launchpoint（該当する場合） </td>
    <td>必要に応じてを設定 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html" target="_blank">LaunchPoint</a> お客様のビジネスに適したサービスです。  <br>注意：インタラクティブウェビナーは、Adobe Connectとネイティブに統合された組み込みのウェビナー機能です。 追加の統合は必要ありませんが、インスタンスで必要になるのは <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html" target="_blank">Adobe Connect as a LaunchPoint Service に同期します。</a>  </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Additional+Integrations">その他の統合</a> </td>
  </tr>
  <tr>
    <td>ウェブフック（該当する場合）</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html" target="_blank">必要なウェブフックを作成する</a> あなたのビジネスのために。  </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Create+a+Webhook">Web フックの作成</a> </td>
  </tr>
</tbody>
</table>

## アイデアスペース {#treasure-chest}

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
    <td>アイデアスペース</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html" target="_blank">宝箱を有効にする</a> を使用して、パイロット機能を試すことができます。  <br>オンまたはオフにする機能を決定します。</td>
    <td>テキスト</td>
  </tr>
  <tr>
    <td>キャンペーンインスペクター </td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html" target="_blank">キャンペーンインスペクターをオンにする</a> すべてのスマートキャンペーンを一度に表示できます。</td>
    <td>テキスト</td>
  </tr>
</tbody>
</table>
