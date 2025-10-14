---
description: 新しい Marketo Engage インスタンスに取り組む前に、継続して使用するための基本的な手順をいくつか完了する必要があります。これらの手順には、ユーザーアカウントの設定、サポート管理者の設定、進行中のシステムアップデートの購読が含まれます。
short-description: 初期設定手順を完了した後で、スムーズに継続使用するための基本的な要素を確立する方法について説明します。
title: ユーザー設定チェックリスト
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 11%

---

# ユーザー設定チェックリスト {#user-setup-checklist}

[&#x200B; 初期設定の手順 &#x200B;](/help/marketo/getting-started/initial-setup/setup-steps.md){target="_blank"} がすべて完了したので、次は、継続的にスムーズに使用するための基本的な要素を確立します。 これにより、Marketo Engageを使用したジャーニーの基盤が構築され、その機能を最大限に活用できるようになります。 それでは始めましょう。

>[!NOTE]
>
>また、このチェックリストを [&#x200B; ベストプラクティスのリストと共に &#x200B;](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) 新しいインスタンスに対してダウンロードし、移動中に手順を確認することもできます。

## Adobe Identity ManagementのMarketo Engage {#marketo-engage-on-adobe-identity-management}

新しいMarketo Engage サブスクリプションは、[Adobe Identity Management System （IMS） &#x200B;](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=ja) に転送されます。 Adobe Admin Consoleで次の User Management レビューに進みます。

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>サブスクリプションおよび Marketo Engage 製品管理者</td>
    <td><li>Adobe組織システム管理者からAdobe製品管理者の役割を付与されたことを確認します。</li>
    <ul>
    <li>Adobe アカウントチーム（アカウントマネージャー）に問い合わせるか、<code>marketocares@marketo.com</code> にメールを送信して組織内で <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=ja">Adobe Admin Console システム管理者 </a> 権限を持っているユーザーを確認します。</li></ul>
    <li>「Marketo Engage製品管理者」のへの招待を受け入れて、Adobe IDをアクティベートします。 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=ja#create-a-product-profile"> ようこそメール </a> は、Adobe Admin Consoleでロールが割り当てられると送信されます。</li></td>
  </tr>
  <tr>
    <td>製品プロファイル</td>
    <td><li>必要なユーザーをすべてAdobe Admin ConsoleのMarketo Engage<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile"> 製品プロファイル </a> に割り当てます。</li>
    <ul>
    <li>Marketo Engage /管理者/ ユーザーと役割でユーザーの役割を割り当ててから、製品プロファイルに追加することはできません。</li>
    <li>各サブスクリプションは、スタンドアロンの製品プロファイルになります。 望ましくないユーザーが複数の製品プロファイル（実稼動サンドボックスやテスト用サンドボックスなど）に追加された場合は、すべての製品プロファイルからそのユーザーを削除する必要があります。 それ以外の場合は、引き続きMarketo Engageにアクセスできます。</li></ul></td>
  </tr>
  <tr>
    <td>ユーザ</td>
    <td><li>いつ <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html?lang=ja"> ユーザーを作成 </a> するかに関するポリシーを作成します。</li> <li>ユーザーを削除するタイミングに関するポリシーを作成します。</li>
    <p><img src="assets/note-icon.png" alt="メモアイコン"> メモ：ユーザーを削除するにはシステム管理者である必要があります。
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=ja">Adobe システム管理者およびMarketo Engage製品管理者権限を持つユーザーを決定します。</a> <li>目的の製品プロファイルに <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user"> ユーザーを追加 </a> します。</li>
    <li>API ユースケースごとに 1 つの API ユーザーを作成します。</li></td>
  </tr>
  <tr>
    <td>User Management API （該当する場合）</td>
    <td><li><a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html">Adobe User Management API</a> を使用して、ユーザーを招待、更新、削除します。</li>
    <li><a href="https://developer.adobe.com/umapi/">Adobe User Management API</a> を使用して、役割を追加または削除します（管理者、サポート管理者、デベロッパーなど）。</li>
    </td>
  </tr>
  <tr>
    <td>製品サポート管理者</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html?lang=ja#create-a-support-ticket-with-admin-console">Adobe Admin Consoleでサポートチケットを送信 </a> するには、システム管理者が「製品サポート管理者」の役割を、管理するサブスクリプションに割り当てる必要があります。 組織のシステム管理者のみが <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html?lang=ja#assign-the-support-admin-role"> この役割に割り当てる </a> ことができます。</li>
    <li>システム管理者から、Marketo Engage サブスクリプションのサポート管理者であることを示すメールを受け取った可能性があります。 その場合は、電子メールの <a href="https://experienceleague.adobe.com/ja/docs/customer-one/using/home#assign-the-support-admin-role"> 「開始 </a>」をクリックして、組織に参加します。</li>
    <li>適切な担当者（バックアップ担当者を 1 人以上含む）を決定し、それに応じて製品サポート管理者の役割を割り当てるようシステム管理者に依頼します。</li></td>
  </tr>
</tbody>
</table>

## Adobe Identity ManagementでのDynamic Chatの設定 {#dynamic-chat-on-adobe-identity-management}

Marketo Engageのネイティブなスレッド自動処理チャネルである [0&rbrace;Dynamic Chat&rbrace; を使用するには、](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html?lang=ja)Adobe Admin Console[&#x200B; の以下の手順に従って、ユーザー権限の設定を行います。](https://adminconsole.adobe.com/){target="_blank"}

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Subscription &amp; Dynamic Chat製品管理者（該当する場合）</td>
    <td><li>Adobe組織システム管理者からAdobe製品管理者の役割を付与されたことを確認します。</li>
    <ul><li>Adobe アカウントチーム（アカウントマネージャー）に問い合わせるか、<code>marketocares@marketo.com</code> にメールを送信して組織内で <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=ja">Adobe Admin Console システム管理者 </a> 権限を持っているユーザーを確認します。</li></ul>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html?lang=ja"> のDynamic Chat製品管理者の招待を受け入 </a> ます。 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html?lang=ja"> ようこそメール </a> は、Marketo Engage インスタンスでDynamic Chatが有効になっており、システム管理者として指定されている場合に送信されます。</li></td>
  </tr>
  <tr>
    <td>製品プロファイル</td>
    <td><li>必要なユーザーをすべてAdobe Admin Consoleの Dynamic Chat 製品プロファイルに割り当てます。</li>
    <ul>
    <li>望ましくないユーザーが複数の製品プロファイルに追加された場合は、すべての製品プロファイルからそのユーザーを削除する必要があります。 それ以外の場合は、Dynamic Chat に引き続きアクセスできます。</li>
    <li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">Dynamic Chatで製品プロファイルを編集 </a> し、カスタムセットのカスタムプロファイルを作成 <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions"> サブスクリプション内で使用可能な権限 </a> できます。</li></td>
  </tr>
  <tr>
    <td>ユーザ</td>
    <td><li>チャットユーザーを追加および削除するタイミングに関するポリシーを作成します。</li>
    <li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">Adobe Dynamic Chat製品管理者権限が必要なユーザーのポリシーを作成します。</a></li>
    <li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user"> 目的の製品プロファイルにユーザーを追加します </a>。</li></td>
  </tr>
</tbody>
</table>

## 継続的なシステム更新と通信の設定 {#system-updates}

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Adobe Marketoのステータス更新</td>
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">Adobe Marketo Engage ステータスのアップデートを購読する </a>。</li></td>
  </tr>
  <tr>
    <td>通知</td>
    <td><li>スマートキャンペーンのエラーや CRM 同期で見つかった重要な問題など、重要な問題に関する <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications"> 管理者通知への登録 </a>。</li></td>
  </tr>
</tbody>
</table>

<p>

Marketo Engage アカウントの準備が整ったので、アドビの [&#x200B; 新しいMarketo Engage インスタンスのベストプラクティス &#x200B;](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/where-to-start.md){target="_blank"} の節を確認して、投資を最大限に活用し、長期的な成功を収めるためのセットアップを行ってください。
