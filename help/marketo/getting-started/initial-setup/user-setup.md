---
description: 新しい Marketo Engage インスタンスに取り組む前に、継続して使用するための基本的な手順をいくつか完了する必要があります。 これらの手順には、ユーザーアカウントの設定、サポート管理者の設定、進行中のシステムアップデートの購読が含まれます。
short-description: 初期設定手順を完了した後で、スムーズに継続使用するための基本的な要素を確立する方法について説明します。
title: ユーザー設定チェックリスト
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 240b78561db11e169188698880d4707a5c1f64de
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 15%

---

# ユーザー設定チェックリスト {#user-setup-checklist}

[初期セットアップ手順](/help/marketo/getting-started/initial-setup/setup-steps.md){target="_blank"}がすべて完了したので、次は、スムーズに継続的に使用できるように、いくつかの基本要素を確立します。 それにより、Marketo Engageを導入する基礎が築かれ、その機能を最大限に活用することができます。 それでは始めましょう。

>[!NOTE]
>
>このチェックリスト、[および新しいインスタンスのベストプラクティスのリスト &#x200B;](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx)をダウンロードして、手順を確認することもできます。

## Adobe Identity Management上のMarketo Engage {#marketo-engage-on-adobe-identity-management}

新しいMarketo Engage サブスクリプションは、[Adobe Identity Management System （IMS） &#x200B;](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=ja)にオンボーディングされます。 Adobe Admin Consoleで次のユーザー管理レビューに進みます。

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
    <td><li>Adobe組織システム管理者からAdobe Product Admin ロールが付与されていることを確認します。</li>
    <ul>
    <li>Adobe アカウントチーム（アカウントマネージャー）に連絡するか、<code>marketocares@marketo.com</code>にメールを送信して、組織の<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=ja">Adobe Admin Console System Admin</a>権限を持つユーザーを確認します。</li></ul>
    <li>「Marketo Engage Product Admin」招待に同意して、Adobe IDをアクティブ化します。 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=ja#create-a-product-profile"> ウェルカムメール </a>は、ロールがAdobe Admin Consoleで割り当てられたときに送信されます。</li></td>
  </tr>
  <tr>
    <td>製品プロファイル</td>
    <td><li>Adobe Admin ConsoleのMarketo Engage <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">Product Profile</a>に、必要なすべてのユーザーを割り当てます。</li>
    <ul>
    <li>製品プロファイルにユーザーを追加する前に、Marketo Engage/管理者/ユーザーと役割でユーザーの役割を割り当てることはできません。</li>
    <li>各サブスクリプションは、スタンドアロンの製品プロファイルになります。 望ましくないユーザーが複数の製品プロファイル（実稼動用サンドボックスやテスト用サンドボックスなど）に追加された場合は、そのユーザーをすべての製品プロファイルから削除する必要があります。 そうでない場合は、Marketo Engageにアクセスできます。</li></ul></td>
  </tr>
  <tr>
    <td>ユーザ</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html"> ユーザーを作成する</a> タイミングのポリシーを作成します。</li> <li>ユーザーを削除するタイミングに関するポリシーを作成します。</li>
    <p><img src="assets/note-icon.png" alt="メモアイコン"> メモ：ユーザーを削除するには、システム管理者である必要があります。
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=ja">Adobe システム管理者とMarketo Engage製品管理者の権限を持つユーザーを決定します。</a> <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user"> ユーザー</a>を目的の製品プロファイルに追加します。</li>
    <li>APIのユースケースごとに1人のAPI ユーザーを作成します。</li></td>
  </tr>
  <tr>
    <td>User Management API （該当する場合）</td>
    <td><li><a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html">Adobe User Management API</a>を使用して、ユーザーを招待、更新、削除します。</li>
    <li><a href="https://developer.adobe.com/umapi/">Adobe User Management API</a>を使用して、役割（管理者、サポート管理者、開発者など）を追加または削除します。</li>
    </td>
  </tr>
  <tr>
    <td>製品サポート管理者</td>
    <td><li>Adobe Admin Console</a>でサポートチケットを<a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html?lang=ja#create-a-support-ticket-with-admin-console">送信するには、管理するサブスクリプションにシステム管理者が「Product Support Administrator」ロールを割り当てる必要があります。 組織のシステム管理者のみが<a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html?lang=ja#assign-the-support-admin-role">この役割に割り当てることができます</a>。</li>
    <li>Marketo Engage サブスクリプションのサポート管理者であることを示すメールがシステム管理者から送信された可能性があります。 その場合は、メール内の<a href="https://experienceleague.adobe.com/ja/docs/customer-one/using/home#assign-the-support-admin-role">'開始'</a>をクリックして組織に参加してください。</li>
    <li>（少なくとも1人のバックアップ担当者を含む）適切な連絡先を決定し、それに応じてシステム管理者が製品サポート管理者の役割を割り当てるようにします。</li></td>
  </tr>
</tbody>
</table>

## Adobe Identity Management版Dynamic Chatの設定 {#dynamic-chat-on-adobe-identity-management}

Marketo Engageのネイティブ会話オートメーションチャネルである[Dynamic Chat](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html?lang=ja)を使用するには、[Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}の次の手順に従って、ユーザー権限の設定に進みます。

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>サブスクリプションとDynamic Chat製品管理者（該当する場合）</td>
    <td><li>Adobe組織システム管理者からAdobe Product Admin ロールが付与されていることを確認します。</li>
    <ul><li>Adobe アカウントチーム（アカウントマネージャー）に連絡するか、<code>marketocares@marketo.com</code>にメールを送信して、組織の<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=ja">Adobe Admin Console System Admin</a>権限を持つユーザーを確認します。</li></ul>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html?lang=ja">'Dynamic Chat Product Admin'</a>の招待に同意します。 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html?lang=ja"> ウェルカムメール </a>は、Marketo Engage インスタンスでDynamic Chatが有効になっていて、システム管理者として指定されている場合に送信されます。</li></td>
  </tr>
  <tr>
    <td>製品プロファイル</td>
    <td><li>Adobe Admin ConsoleのDynamic Chat製品プロファイルに、必要なユーザーをすべて割り当てます。</li>
    <ul>
    <li>不要なユーザーが複数の製品プロファイルに追加された場合は、すべての製品プロファイルからユーザーを削除する必要があります。 それ以外の場合は、Dynamic Chat に引き続きアクセスできます。</li>
    <li>Dynamic Chat</a>で製品プロファイルを<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">編集し、サブスクリプション </a>内で利用可能な<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">権限のカスタムセットを使用してカスタムプロファイルを作成できます。</li></td>
  </tr>
  <tr>
    <td>ユーザ</td>
    <td><li>チャットユーザーを追加および削除するタイミングに関するポリシーを作成します。</li>
    <li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">Adobe Dynamic Chat Product Admin権限を持つユーザーに関するポリシーを作成します。</a></li>
    <li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">目的の製品プロファイルにユーザーを追加</a>。</li></td>
  </tr>
</tbody>
</table>

## 継続的なシステム更新とコミュニケーションの設定 {#system-updates}

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
    <td><li><a href="https://status.adobe.com/ja-jp/cloud/experience_cloud">Adobe Marketo Engageのステータス更新を購読する</a>。</li></td>
  </tr>
  <tr>
    <td>通知</td>
    <td><li>スマートキャンペーンのエラーや、CRM同期で見つかった重大な問題などの重要な問題については、<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">管理者通知</a>を購読します。</li></td>
  </tr>
</tbody>
</table>

<p>

Marketo Engage アカウントの準備が整ったら、[新しいMarketo Engage インスタンスのベストプラクティス &#x200B;](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/where-to-start.md){target="_blank"}のセクションを確認して、投資を最大限に活用し、長期的な成功に向けて準備してください。
