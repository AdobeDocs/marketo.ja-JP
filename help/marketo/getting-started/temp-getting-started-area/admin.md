---
description: 新しい領域 - Marketo ドキュメント - 製品ドキュメント
title: 新しい領域
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 9f442b64f2e6d012207f79d06298583655db86b7
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 61%

---

# 新しい領域：管理者チェックリスト {#new-area-admin-checklist}

概要テキスト。

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
    <li>組織のニーズとユーザのログイン頻度に基づいて、<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=ja#create-a-new-role" target="_blank">新しいロールを作成</a>するか、<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=ja#edit-a-role" target="_blank">ロールを編集</a>します。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html%22%20/l%20%22assign-roles-to-a-user" target="_blank">ユーザーを適切な役割に割り当てる</a>. ユーザーは、役割で役割を付与する前に、Adobe Admin Consoleの購読に追加される必要があります。 「初期設定」チェックリスト [LINK] の「ユーザー」の節を参照してください。</li>
    <li>ユーザにロールを割り当てた後、ロールごとのユーザ数を確認します。<br>トラブルシューティングを容易にするために、各 API ユーザーに固有の役割を実装します。</td>
  </tr>
  <tr>
    <td>ドキュメント</td>
    <td><li>組織のユーザーと役割を定義します。</li>
    <li>新しいユーザー/管理者を追加するためのプロセスを定義します。</li></td>
  </tr>
  <tr>
    <td>サンドボックス（該当する場合）</td>
    <td><li>サンドボックスがある場合は、上記のカテゴリを確認します。</li></td>
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
    <li>各ワークスペースとパーティションの主な目的を定義します。<br>ワークスペースとパーティション間の関係を定義します。</li></td>
  </tr>
  <tr>
    <td>ドキュメント</td>
    <td><li>ワークスペースの定義方法と、データベースパーティションへの関連付け（つまり、すべてのユーザとビジネスセクターとの比較が表示されるグローバルワークスペース）をドキュメント化します。</li>
    <li>適切なパーティションに新しいレコードを読み込みます。</li>
    <li>適切なパーティションにユーザを配置する値を CRM で定義します。</li></td>
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
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html?lang=ja" target="_blank">スマートキャンペーンのサイズに関する制限</a>を追加して、データベース全体に誤ってメールを送信することを防ぎます。</li></td>
  </tr>
  <tr>
    <td>ドキュメント</td>
    <td><li>ワークスペースの定義方法と、データベースパーティションへの関連付け（つまり、すべてのユーザとビジネスセクターとの比較が表示されるグローバルワークスペース）をドキュメント化します。</li>
    <li>適切なパーティションに新しいレコードを読み込みます。</li>
    <li>適切なパーティションにユーザを配置する値を CRM で定義します。</li></td>
  </tr>
</tbody>
</table>

## メール設定 {#email-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>メールのデフォルト</td>
    <td><li>ブランディングドメインでドメインを選択し、メールの CNAME を追加します。これは次の形式で記述します。[EmailTrackingCNAME].[CompanyDomain].com</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console" target="_blank">Marketo サポートに連絡</a> SSL 証明書のプロビジョニングで保護します。 プロセスが完了するまでに最大で 3 営業日かかります。</li></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li>メール配信用に <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html?lang=ja" target="_blank">SPF と DKIM の設定</a></li></td>
  </tr>
  <tr>
  </tr>
  <tr>
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
    <td><li>「<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html?lang=ja" target="_blank" rel="noopener noreferrer">通信制限</a>」を配置します。</li>
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
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html?lang=ja" target="_blank" rel="noopener noreferrer">チャネル</a>の使用方法を定義します。</li></td>
  </tr>
  <tr>
    <td>タグ</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html?lang=ja" target="_blank" rel="noopener noreferrer">タグ</a>の使用方法を定義します。</li></td>
  </tr>
  <tr>
    <td>カレンダー（該当する場合）</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html?lang=ja" target="_blank" rel="noopener noreferrer">問題のマーケティング カレンダーの席</a> アクセスが必要なユーザーに送信されます。 <br>の設定 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html" target="_blank" rel="noopener noreferrer">カレンダー。</a></li></td>
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
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html?lang=ja" target="_blank" rel="noopener noreferrer">カスタムフィールドの命名規則を実装します。</a> 例えば、「MKTO」で始めます。</li>
    <li>同期するフィールドについては慎重に選択してください。同期するフィールドが多いほど、同期サイクルが遅くなります。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html?lang=ja" target="_blank" rel="noopener noreferrer">フィールドの更新をブロック</a> 1 回だけ書き込む（元のリードソース、元のリードソースの詳細、ファーストタッチ UTM フィールドなど）</li></td>
  </tr>
  <tr>
  </tr>
  <tr>
    <td>カスタムアクティビティ</td>
    <td><li>ビジネスに固有の<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html?lang=ja">カスタムアクティビティ</a>を定義します。</li></td>
  </tr>
  <tr>
    <td>カスタムオブジェクト</td>
    <td><li>必要な<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html?lang=ja">カスタムオブジェクト</a>の数を確認します。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html?lang=ja">これらのカスタムオブジェクトを CRM に同期</a>。</li></td>
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
    <td><li>CRM 同期を開始します。会社で使用している CRM に応じて、次の中 <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html?lang=ja">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html?lang=ja">Microsoft Dynamics</a> から選択します。</li>
    <li>CRM にアクセスするのに必要なアクセスのタイプを特定します。</li>
    <li>トラブルシューティング用の CRM 管理者を特定します。</li></td>
  </tr>
  <tr>
    <td>ランディングページ</td>
    <td>メモ：Launch Pack をご利用の場合は、この手順をスキップできます。初回コール時に、担当のコンサルタントが IT セットアップ手順書を提供します。<br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html?lang=ja">CNAME</a>を使用してランディングページのドメインを設定し、<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html?lang=ja">ドメインとページの情報を入力</a>します。これは次の形式で記述します。[LandingPageCNAME].[CompanyDomain].com <br>ランディングページの CNAME を選択します。次に例を示します。<br>* **go**.[CompanyDomain].com <br>* **www2**.[CompanyDomain].com <br>* **lp**.[CompanyDomain].com <br><a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console">Marketo サポートに連絡</a> ssl 証明書のプロビジョニングのプロセスを開始します。 このプロセスが完了するまでに最大 3 営業日かかる場合があります。 <br>ヒント：短くしてください。 URL は短いほど覚えやすくなります。ドメインには「go」を指定することをお勧めします。<br>分析トラッキングコード（Google Analytics や Adobe Analytics など）をランディングページテンプレートに追加します。 </td>
  </tr>
  <tr>
    <td>Munchkin</td>
    <td>メモ：Launch Pack をご利用場合は、この手順をスキップしてください。担当のコンサルタントが、IT セットアップ手順ドキュメントに Munchkin コード手順を提供します。Web サイトに <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.html?lang=ja">Munchkin トラッキングコードを追加</a>します。Munchkin コードは、<a href="https://developers.marketo.com/javascript-api/lead-tracking/">ハードコード</a>することも、Google タグマネージャー経由でデプロイすることもできます。  </td>
  </tr>
  <tr>
    <td>Web サービス</td>
    <td><li>実行できるユーザー/アプリの決定 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html?lang=ja">API 呼び出し</a> インスタンス内。</li>
    <li>API 呼び出しを行うすべてのアプリを確認し、API 呼び出しに増加と削減のどちらが必要かを判断します。</li></td>
  </tr>
  <tr>
    <td>Launchpoint</td>
    <td><li>必須の設定 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html?lang=ja">LaunchPoint</a> お客様のビジネスに対応するサービス。 各 LaunchPoint は、トラブルシューティングに役立つように一意の API ユーザーとペアにする必要があります。</li></td>
  </tr>
  <tr>
    <td>インタラクティブウェビナー（該当する場合）</td>
    <td>メモ：インタラクティブウェビナーは、実稼動インスタンスにのみプロビジョニングされます。
    <li>インタラクティブウェビナーの作成のために、組み込みのウェビナー機能 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management">「ユーザー」セクションにユーザーを追加</a> 「インタラクティブウェビナー」タブで、次の操作を行います。</li></td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat（該当する場合）</td>
    <td>使用する場合 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html?lang=ja">Dynamic Chat</a>は、Marketo Engageのネイティブなコンバージョン自動処理チャネルです。次の手順に従って、ユーザー権限の設定を行います <a href="https://adminconsole.adobe.com/">Adobe Admin Console</a>. <br>Adobe組織システム管理者から「Adobe製品管理者」ロールを付与されているかどうかを確認します。 連絡先 <a href="https://helpx.adobe.com/contact.html">Adobeカスタマーケア</a> をクリックして、コンソールで管理者権限を持つ組織のユーザーを確認します。 <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html?lang=ja">「Dynamic Chat 製品管理者」の招待</a>を承認します。この<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html?lang=ja">ウェルカムメール</a>は、Marketo Engage インスタンスで Dynamic Chat が有効になっており、ご自身をシステム管理者として指定している場合に送信されます。<br>Adobe Admin Consoleで、Dynamic Chatの製品プロファイルに適切なユーザーをすべて割り当てます。 <br>望ましくないユーザーが複数の製品プロファイルに追加された場合は、すべての製品プロファイルからそのユーザーを削除する必要があります。 そうでない場合でも、Dynamic Chatにアクセスできます。 <br>次のことができます <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">Dynamic Chatでの製品プロファイルの編集</a> 次のカスタムセットを使用してカスタムプロファイルを作成します <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">サブスクリプション内で使用可能な権限</a>. <br>ユーザー割り当て先 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role">「Dynamic Chatにアクセス」の役割</a> Marketo Engage/管理者/ユーザーと役割 </td>
  </tr>
  <tr>
    <td>Sales Insight（該当する場合）</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account">販売インサイト アクションの設定</a> [Sales Insight]&gt;[Actions Config] の順にクリックします。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html?lang=ja#invite-individual-users-to-msi-actions">適切なユーザにシートを発行します。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html?lang=ja">API を設定</a>します。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html?lang=ja">リードスコアをカスタマイズします。</a></li></td>
  </tr>
  <tr>
    <td>Sales Connect （該当する場合）</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance">Sales Connect インスタンスに適切なMarketo Engage管理者を招待します。</a>.</li>
    <li>を完了する <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins">追加の Sales Connect 管理者設定</a> （Sales Connect および Salesforce の場合）。</li></td>
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
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html?lang=ja">宝箱を有効にする</a> パイロット機能を試してみる。</li>
    <li>オンまたはオフにする機能を決定します。</li></td>
  </tr>
  <tr>
    <td>キャンペーンインスペクター </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html?lang=ja">キャンペーンインスペクターをオンに</a>すると、すべてのスマートキャンペーンを一度に表示できます。</li></td>
  </tr>
</tbody>
</table>
