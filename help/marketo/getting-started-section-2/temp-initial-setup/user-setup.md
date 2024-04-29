---
description: 早期設定チェックリスト - Marketo ドキュメント – 製品ドキュメント
title: 早期設定チェックリスト
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 8473c4d59210bb18c3968a56883034febf00c320
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 6%

---

# 新しい領域：早期設定チェックリスト {#early-setup-checklist}

概要テキスト。

## AdobeIdentity ManagementのMarketo Engage {#marketo-engage-on-adobe-identity-management}

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>サブスクリプションおよび Marketo Engage 製品管理者 </td>
    <td><li>Adobe組織システム管理者から「Adobe製品管理者」ロールを付与されていることを確認します。</li>  
    <ul>
    <li>連絡先 <a href="https://helpx.adobe.com/contact.html">Adobeカスタマーケア</a> 組織の担当者を確認する場合 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobe Admin Console System Admin</a> 権限。</li></ul>
    <li>「Marketo Engage製品管理者」の招待を受け入れて、Adobe IDをアクティブ化します。 この <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=en#create-a-product-profile">お知らせメール</a> は、Adobe Admin Consoleで役割が割り当てられると送信されます。</li></td>
  </tr>
  <tr>
    <td>製品プロファイル</td>
    <td><li>該当するすべてのユーザーをMarketo Engageに割り当てます。 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">製品プロファイル</a> Adobe Admin Consoleで。</li>
    <ul>
    <li>ユーザーのロールを製品プロファイルに追加する前に、「Marketo Engage」/「管理者」/「ユーザーとロール」で割り当てることはできません。</li>
    <li>各サブスクリプションは、スタンドアロンの製品プロファイルになります。 望ましくないユーザーが複数の製品プロファイル（実稼動サンドボックスやテスト用サンドボックスなど）に追加された場合は、すべての製品プロファイルからそのユーザーを削除する必要があります。 そうでない場合でも、Marketo Engageにアクセスできます。</li></ul></td>
  </tr>
  <tr>
    <td>ユーザ</td>
    <td><li>実行するタイミングに関するポリシーの作成 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html">ユーザーの作成</a>.</li> <li>ユーザーを削除するタイミングに関するポリシーを作成します。</li>
    <li>誰に権限を付与すべきかを判断する <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobeシステム管理者およびMarketo Engage製品管理者の権限。</a> <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user">ユーザーを追加</a> を目的の製品プロファイルに追加します。</li>
    <li>API ユースケースごとに 1 つの API ユーザーを作成します。</li></td>
  </tr>
  <tr>
    <td>製品サポート管理者 </td>
    <td><li>終了 <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#create-a-support-ticket-with-admin-console">Adobe Admin Consoleでサポートチケットを送信</a>を使用するには、システム管理者から「製品サポート管理者」の役割を、ユーザーが管理する購読に割り当てられている必要があります。 組織内のシステム管理者のみが、 <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#assign-the-support-admin-role">割り当て先：この役割</a>.</li>
    <li>Marketo Engage管理者から、システム購読のサポート管理者であることを示すメールを受け取った可能性があります。 該当する場合は、 <a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#assign-the-support-admin-role">電子メールでの「基本を学ぶ」</a> 組織に参加します。</li>
    <li>適切な担当者（バックアップ担当者 1 人以上）を決定し、システム管理者に、事前に製品サポート管理者の役割を割り当ててもらいます。</li></td>
  </tr>
</tbody>
</table>

## AdobeIdentity Management設定のDynamic Chat {#dynamic-chat-on-adobe-identity-management}

テキスト

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>購読およびDynamic Chat製品管理者（該当する場合） </td>
    <td><li>Adobe組織システム管理者から「Adobe製品管理者」ロールを付与されているかどうかを確認します。 連絡先 <a href="https://helpx.adobe.com/contact.html">Adobeカスタマーケア</a> をクリックして、コンソールで管理者権限を持つ組織のユーザーを確認します。</li>
    <li>承諾 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html?lang=ja">「Dynamic Chat製品管理者」の招待</a>. この <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html?lang=ja">お知らせメール</a> は、Marketo EngageインスタンスでDynamic Chatが有効になっており、システム管理者に指定されている場合に送信されます。</li></td>
  </tr>
  <tr>
    <td>製品プロファイル </td>
    <td><li>Adobe Admin Consoleで、Dynamic Chatの製品プロファイルに適切なユーザーをすべて割り当てます。</li> 
    <ul>
    <li>望ましくないユーザーが複数の製品プロファイルに追加された場合は、すべての製品プロファイルからそのユーザーを削除する必要があります。 それ以外の場合は、Dynamic Chat に引き続きアクセスできます。</li>
    <li>次のことができます <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">Dynamic Chatでの製品プロファイルの編集</a> 次のカスタムセットを使用してカスタムプロファイルを作成します <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">サブスクリプション内で使用可能な権限</a>.</li></td>
  </tr>
  <tr>
    <td>ユーザ </td>
    <td><li>チャットユーザーを追加および削除するタイミングに関するポリシーを作成します。</li>
    <li>誰に権限を付与すべきかについてポリシーを作成します <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">製品管理者権限をAdobe Dynamic Chatします。</a></li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">目的の製品プロファイルへのユーザーの追加</a>.</li></td>
  </tr>
</tbody>
</table>

## 継続的なシステムのアップデートと通信の設定

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>AdobeMarketoのステータス更新 </td>
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">Adobe Marketo Engage ステータスのアップデートを購読</a>.</li></td>
  </tr>
  <tr>
    <td>通知 </td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">管理者通知のサブスクライブ</a> スマートキャンペーンのエラーや CRM 同期で見つかった重要な問題など、重要な問題の場合。</li></td>
  </tr>
</tbody>
</table>
