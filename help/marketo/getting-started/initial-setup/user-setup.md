---
description: 新しい Marketo Engage インスタンスに取り組む前に、継続して使用するための基本的な手順をいくつか完了する必要があります。これらの手順には、ユーザーアカウントの設定、サポート管理者の設定、進行中のシステムアップデートの購読が含まれます。
short-description: 初期設定手順を完了した後で、スムーズに継続使用するための基本的な要素を確立する方法について説明します。
title: ユーザー設定チェックリスト
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 471a777041361cfebdc8b7139b618ff4dc03e8a8
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 10%

---

# ユーザー設定チェックリスト {#user-setup-checklist}

[ 初期設定の手順 ](/help/marketo/getting-started/initial-setup/setup-steps.md){target="_blank"} がすべて完了したので、次は、継続的にスムーズに使用するための基本的な要素を確立します。 これにより、Marketo Engageを使用したジャーニーの基盤が構築され、その機能を最大限に活用できるようになります。 それでは始めましょう。

>[!NOTE]
>
>また、このチェックリストを [ ベストプラクティスのリストと共に ](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) 新しいインスタンスに対してダウンロードし、移動中に手順を確認することもできます。

## AdobeIdentity ManagementのMarketo Engage {#marketo-engage-on-adobe-identity-management}

新しいMarketo Engageのサブスクリプションは、[AdobeIdentity Management System （IMS） ](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=ja) に転送されます。 Adobe Admin Consoleで次の User Management レビューに進みます。

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
    <td><li>Adobe組織システム管理者から「Adobe製品管理者」の役割を付与されていることを確認します。</li> 
    <ul>
    <li>Adobeアカウントチーム（アカウントマネージャー）に問い合わせるか、<code>marketocares@marketo.com</code> にメールを送信して組織内で <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=ja">Adobe Admin Console システム管理者 </a> 権限を持っているユーザーを確認します。</li></ul>
    <li>「Marketo Engage製品管理者」の招待を受け入れて、Adobe IDをアクティブ化します。 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=ja#create-a-product-profile"> ようこそメール </a> は、Adobe Admin Consoleでロールが割り当てられると送信されます。</li></td>
  </tr>
  <tr>
    <td>製品プロファイル</td>
    <td><li>必要なユーザーをすべてAdobe Admin ConsoleのMarketo Engage<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile"> 製品プロファイル </a> に割り当てます。</li>
    <ul>
    <li>Marketo Engage/管理者/ユーザーと役割でユーザーの役割を割り当ててから、製品プロファイルに追加することはできません。</li>
    <li>各サブスクリプションは、スタンドアロンの製品プロファイルになります。 望ましくないユーザーが複数の製品プロファイル（実稼動サンドボックスやテスト用サンドボックスなど）に追加された場合は、すべての製品プロファイルからそのユーザーを削除する必要があります。 そうでない場合でも、Marketo Engageにアクセスできます。</li></ul></td>
  </tr>
  <tr>
    <td>ユーザ</td>
    <td><li>いつ <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html?lang=ja"> ユーザーを作成 </a> するかに関するポリシーを作成します。</li> <li>ユーザーを削除するタイミングに関するポリシーを作成します。</li>
    <p><img src="assets/note-icon.png" alt="メモアイコン"> メモ：ユーザーを削除するにはシステム管理者である必要があります。
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=ja">Adobeシステム管理者およびMarketo Engage製品管理者のアクセス許可を持つユーザーを決定します。</a> <li>目的の製品プロファイルに <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user"> ユーザーを追加 </a> します。</li>
    <li>API ユースケースごとに 1 つの API ユーザーを作成します。</li></td>
  </tr>
  <tr>
    <td>User Management API （該当する場合）</td>
    <td><li><a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html">User Management API</a> を使用して、Adobeを招待、更新、および削除します。</li>
    <li><a href="https://developer.adobe.com/umapi/">AdobeUser Management API</a> を使用して、役割を追加または削除します（管理者、サポート管理者、デベロッパーなど）。</li>
    </td>
  </tr>
  <tr>
    <td>製品サポート管理者</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html?lang=ja#create-a-support-ticket-with-admin-console">Adobe Admin Consoleでサポートチケットを送信 </a> するには、システム管理者が「製品サポート管理者」の役割を、管理するサブスクリプションに割り当てる必要があります。 組織のシステム管理者のみが <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html?lang=ja#assign-the-support-admin-role"> この役割に割り当てる </a> ことができます。</li>
    <li>Marketo Engage管理者から、システム購読のサポート管理者であることを示すメールを受け取った可能性があります。 その場合は、電子メールの <a href="https://experienceleague.adobe.com/ja/docs/customer-one/using/home#assign-the-support-admin-role"> 「開始 </a>」をクリックして、組織に参加します。</li>
    <li>適切な担当者（バックアップ担当者を 1 人以上含む）を決定し、それに応じて製品サポート管理者の役割を割り当てるようシステム管理者に依頼します。</li></td>
  </tr>
</tbody>
</table>

## AdobeIdentity Management設定のDynamic Chat {#dynamic-chat-on-adobe-identity-management}

Marketo Engageのネイティブなスレッド自動処理チャネルである [&#128279;](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html?lang=ja)0&rbrace;Dynamic Chat&rbrace; を使用するには、[Adobe Admin Console&rbrace; の以下の手順に従って、ユーザー権限設定に進み ](https://adminconsole.adobe.com/){target="_blank"} す。

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>購読およびDynamic Chat製品管理者（該当する場合）</td>
    <td><li>Adobe組織システム管理者から「Adobe製品管理者」の役割を付与されていることを確認します。</li> 
    <ul><li>Adobeアカウントチーム（アカウントマネージャー）に問い合わせるか、<code>marketocares@marketo.com</code> にメールを送信して組織内で <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=ja">Adobe Admin Console システム管理者 </a> 権限を持っているユーザーを確認します。</li></ul>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html?lang=ja"> のDynamic Chat製品管理者の招待を受け入 </a> ます。 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html?lang=ja"> ようこそメール </a> は、Marketo EngageインスタンスでDynamic Chatが有効になっており、システム管理者として指定されている場合に送信されます。</li></td>
  </tr>
  <tr>
    <td>製品プロファイル</td>
    <td><li>Adobe Admin Consoleで、必要なすべてのユーザーをDynamic Chatの製品プロファイルに割り当てます。</li> 
    <ul>
    <li>望ましくないユーザーが複数の製品プロファイルに追加された場合は、すべての製品プロファイルからそのユーザーを削除する必要があります。 それ以外の場合は、Dynamic Chat に引き続きアクセスできます。</li>
    <li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">Dynamic Chat内で製品プロファイルを編集 </a> し、カスタムセットの <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions"> サブスクリプション内で使用可能な権限 </a> を使用してカスタムプロファイルを作成できます。</li></td>
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
    <td>AdobeMarketoのステータス更新</td>
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">Adobe Marketo Engage ステータスのアップデートを購読する </a>。</li></td>
  </tr>
  <tr>
    <td>通知</td>
    <td><li>スマートキャンペーンのエラーや CRM 同期で見つかった重要な問題など、重要な問題に関する <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications"> 管理者通知への登録 </a>。</li></td>
  </tr>
</tbody>
</table>

<p>

Marketo Engageアカウントの準備が整ったので、アドビの [ 新しいMarketo Engageインスタンスのベストプラクティス ](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/where-to-start.md){target="_blank"} の節を確認して、投資を最大限に活用し、長期的な成功を収めるためのセットアップを行ってください。
