---
description: 継承インスタンス管理者チェックリスト - Marketo ドキュメント - 製品ドキュメント
title: 継承インスタンス管理者チェックリスト
feature: Getting Started
exl-id: 088f3ce9-bf3d-4323-9cde-c39fec06c20e
TQID: https://experienceleague.adobe.com/FCMSgPqv3eJh4Etqe3J7305tnfQbVrghY8nc2Im6Ww8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ea90ebee-5c84-42d9-8b21-006bdabc95a3
subfeature_v2: id: a8c137b3-8aa5-433e-bdc9-0a216c2a11c1id: c942e9f6-ed06-481a-abdd-1195363d1452id: e5d29014-8a81-4c0c-845b-2adc7a5d6258id: ea4e3ff5-e7b9-4b4c-a5a0-dc27cc3f4275id: efc9a24a-a6a4-449d-a3e6-44f6c74dfd46id: f5e85a9b-a883-40d0-8759-f3651efb32e9id: f7d2c504-7d5f-4a94-b77e-7fce7ef46c22id: fc5c4f1e-5467-43ac-94e9-0acfa71c517did: fc9b09fe-b844-4544-887b-e420c3b82065
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 1943
ht-degree: 89%

---

# 継承インスタンス：「管理者」セクションのチェックリスト {#inherited-instance-admin-section-checklist}

以下のチェックリスト（各記事の下部にリンクされている後続のチェックリスト）は、即座に理解できるように、Marketo Champions からの入力を基にして Adobe Professional Services によってまとめられたものです。 また、[チェックリストをダウンロード](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx)して、進捗を追跡することもできます。

>[!TIP]
>
>Marketo Engageの初心者で、多くの用語に精通していない場合は、[Marketo Engage用語集](/help/marketo/getting-started/things-to-know/marketo-engage-glossary.md){target="_blank"}を参照してください。

## Adobe Identity Management {#adobe-identity-management}

>[!NOTE]
>
>[Adobe Identity Management システム（IMS）](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"}にオンボードされた Marketo Engage サブスクリプションにのみ適用されます。 サブスクリプションに Adobe IMS がまだオンボードされていない場合は、Marketo Engage／管理者／ユーザ＆ロールで、[従来のユーザロールと権限のエクスペリエンス](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}に進みます。

<table>
 <tbody>
  <tr>
   <th style="width:20%">エリア</th>
   <th>レビューフォーカス</th>
  </tr>
  <tr>
   <td>サブスクリプションおよび Marketo Engage 製品管理者</td>
   <td><li>お使いのMarketo Engage サブスクリプションは、まだ<a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md" target="_blank">Adobe IMS</a>に移行されていますか？
<br/>     移行が完了している場合、「Adobe Admin Console システム管理者」から「Adobe Admin Console 製品管理者」ロールが付与されていますか？ 組織内の誰がコンソールで管理者権限を持っているかわからない場合は、<a href="https://helpx.adobe.com/jp/contact.html" target="_blank">Adobe カスタマーケア </a>にお問い合わせください。</li>
<li>「Marketo Engage 製品管理者」の招待を受け入れましたか？ Adobe Admin Console でロールが割り当てられると、メールが送信されます。
<br/>     そうでない場合は、インボックスで<a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md#initial-setup" target="_blank">ウェルカムメール</a>を探し、招待を受け入れて Adobe ID をアクティベートします。</li></td>
  </tr>
  <tr>
   <td>製品プロファイル</td>
   <td><li>すべての適切なユーザが Adobe Admin Console で Marketo Engage の製品プロファイルに割り当てられていますか？
<br/>     そうでない場合は、Adobe Admin Console の Marketo Engage 製品プロファイルから必ず<a href="/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-user.md" target="_blank">ユーザを追加または削除</a>してください。 ユーザが製品プロファイルに追加されている場合、Marketo Engage／管理者／ユーザ＆ロールでユーザのロールを割り当てることはできません。</li>
<p><img src="assets/note-icon.png" alt="メモアイコン"> メモ：望ましくないユーザが複数の製品プロファイルに追加された場合は、そのユーザをすべての製品プロファイルから削除する必要があります。 それ以外の場合は、Marketo Engage に引き続きアクセスできます。</td>
  </tr>
  <tr>
   <td>User Management API</td>
   <td><li>サブスクリプションで Marketo User Management API を使用していますか？
<br/>     その場合、今後は <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html" target="_blank">Adobe IMS API</a> を使用してユーザを招待、更新、削除する必要があります。</li>
<p><img src="assets/note-icon.png" alt="メモアイコン"> メモ：「ロール管理」は、Marketo Engage に残り、Marketo User Management API をロール管理に引き続き使用できます。</td>
  </tr>
 </tbody>
</table>

## ユーザ＆ロール {#users-and-roles}

<table>
 <tbody>
  <tr>
   <th style="width:20%">エリア</th>
   <th>レビューフォーカス</th>
  </tr>
  <tr>
   <td>ユーザ</td>
   <td><img src="assets/note-icon.png" alt="メモアイコン"> メモ：サブスクリプションが既に Adobe IMS にある場合は、Adobe Admin Console で次のユーザ管理の確認に進みます。 それ以外の場合は、Marketo Engage で管理者／ユーザ＆ロール／ユーザに移動します。
   <p>
   <li>ユーザー数は？</li>
<li><a href="/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-user.md#remove-a-user" target="_blank">削除</a>する必要があるユーザはいますか？</li>
<li>会社にはユーザの削除に関するポリシーがありますか？</li>
<li><a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">管理者権限</a>を持つユーザ数はいくつですか？</li>
<li>これらのユーザのいずれかを<a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">他のロール</a>に変更する必要がありますか？</li>
</td>
  </tr>
  <tr>
   <td>ロール</td>
   <td><img src="assets/note-icon.png" alt="メモアイコン"> メモ：Marketo を Adobe ID と共に使用するかどうかに関わらず、Marketo Engage の管理者／ユーザ＆ロール／ロールでロール権限の確認に進みます。
   <p><li>ロール数はいくつですか？</li>
<li>各ロールにはどのような<a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">権限／アクセス権</a>がありますか？ 調整する必要がありますか？</li>
<li>ロールごとにユーザは何人いますか？</li>
<li>ユーザはどのくらいの頻度で<a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">ログイン</a>していますか？</li>
<li>各 API ユーザは<a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">独自のユーザロール</a>を持っていますか？ そうでない場合は、トラブルシューティングを容易にするために、独自のユーザロールを実装することを検討してください。</li>
<li>ユーザのロールと権限は、規制遵守のために企業データプライバシーポリシー（例：<a href="https://gdpr-info.eu/" target="_blank">GDPR</a>）と一致していますか？ 企業データ<a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">プライバシーポリシー</a>では、ユーザが Marketo Engage ユーザのデータをダウンロードして共有することを許可していますか？ 許可業務は必要ですか？</li></td>
  </tr>
  <tr>
   <td>サポートユーザ</td>
   <td><li>サポートポータルで適切な<a href="/help/marketo/getting-started/initial-setup/setup-steps.md#set-up-your-authorized-support-contacts" target="_blank">承認済み取引先責任者</a>を設定しましたか？</li></td>
  </tr>
  <tr>
   <td>内部ドキュメント</td>
   <td><li>組織ではユーザとロールが明確に定義されていますか？</li>
<li>新しいユーザ／管理者を追加するプロセスを教えてください。</li></td>
  </tr>
  <tr>
   <td>サンドボックス（該当する場合）</td>
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">サンドボックスインスタンス</a>はありますか？
   <br/>     その場合は、お使いのサンドボックスで上記のカテゴリを確認してください。</li>
<li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">プログラムの読み込み</a>はサンドボックスにリンクされていますか？</li></td>
  </tr>
 </tbody>
</table>

## 監査記録 {#audit-trail}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">エリア</th>
   <th>レビューフォーカス</th>
  </tr>
  <tr>
   <td>監査記録</td>
   <td><li>インスタンスで<a href="/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md" target="_blank">作業しているユーザ</a>は誰ですか？</li></td>
  </tr>
 </tbody>
</table>

## ワークスペースとパーティション {#workspaces-and-partitions}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">エリア</th>
   <th>レビューフォーカス</th>
  </tr>
  <tr>
   <td>ワークスペースとパーティション</td>
   <td><li><a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md" target="_blank">ワークスペースやパーティション</a>はいくつありますか？</li>
<li>各ワークスペースとパーティションの主な目的は何ですか？</li>
<li><a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-a-workspace.md" target="_blank">ワークスペース</a>または<a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-an-existing-person-partition.md" target="_blank">パーティション</a>のいずれかを監査／変更する必要がありますか？</li>
<li>ワークスペースとパーティションの関係は何ですか？</li>
<li>各ワークスペースに<a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.md" target="_blank">アクセスできる</a>ユーザは何人ですか？</li></td>
  </tr>
  <tr>
   <td>内部ドキュメント</td>
   <td><li>ワークスペースとパーティションの定義方法を教えてください。</li>
<li>インスタンスにワークスペースを追加する、またはワークスペースにユーザを追加するプロセスを教えてください。</li></td>
  </tr>
 </tbody>
</table>

## スマートキャンペーン {#smart-campaigns}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">エリア</th>
   <th>レビューフォーカス</th>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td><li><a href="/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md" target="_blank"> スマートキャンペーンのサイズに制限</a>はありますか？
   <br/>     ない場合は、制限を追加することを検討してください。 ワークフローでの過剰通信やデータベース全体の処理を避けるために、スマートキャンペーンの制限をデータベースの 25％に制限することをお勧めします。これはブランドだけでなく、インスタンスのパフォーマンスを保護します。</li></td>
  </tr>
 </tbody>
</table>

## 通信制限 {#communication-limits}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">エリア</th>
   <th>レビューフォーカス</th>
  </tr>
  <tr>
   <td>通信制限</td>
   <td><li><a href="/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md" target="_blank">通信制限</a>はありますか？ 社内では、通信制限が必要なポリシーが導入されていますか？</li>
<p><img src="assets/note-icon.png" alt="メモアイコン"> メモ：通信を 1 日あたり 1 件、7 日間あたり 3 件に制限し、<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md" target="_blank">業務</a><b>以外</b>のメールはブロックすることをお勧めします。</td>
  </tr>
 </tbody>
</table>

## タグ {#tags}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">エリア</th>
   <th>レビューフォーカス</th>
  </tr>
  <tr>
   <td>タグ</td>
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags.md" target="_blank">タグはいくつ</a>ありますか？ 使用中のタグはいくつありますか？ 追加する必要はありますか？</li>
<li>プログラム内にタグは必要ですか？</li></td>
  </tr>
  <tr>
   <td>チャネル</td>
   <td><li><a href="/help/marketo/product-docs/administration/tags/create-a-program-channel.md" target="_blank">チャネルはいくつ</a>ありますか？ 使用中はいくつありますか？</li>
<li>すべての<a href="/help/marketo/product-docs/administration/tags/hide-unhide-a-program-channel.md" target="_blank">チャネルのプログラムのステータスは適切</a>ですか？ プログラム内の進行状況は表示されますか？</li>
<li>チャネルは特定のプログラムタイプに関連していますか？</li>
<li>各チャネルで成功と見なされるステータスはどれですか？ それらはマーケティング目標に合っていますか？</li>
<li>オペレーショナルチャネルは適切に使用されていますか？</li>
<li>高度な Report Builder（Revenue Cycle Explorer／RCE）の場合、チャネル分析の動作は、期間コストを組み込んだプログラムのプラクティスに合わせて設定されていますか？</li></td>
  </tr>
  <tr>
   <td>マーケティングカレンダー（該当する場合）</td>
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.md" target="_blank">カレンダーエントリ</a>のタイプはいくつありますか？ それらはすべて今でも関連性がありますか？</li></td>
  </tr>
 </tbody>
</table>

## データベース管理 {#database-management}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">エリア</th>
   <th>レビューフォーカス</th>
  </tr>
  <tr>
   <td>フィールド管理</td>
   <td><li>フィールド数は？
   <br/>     「<a href="/help/marketo/product-docs/administration/field-management/export-a-list-of-all-marketo-api-field-names.md" target="_blank">フィールド名を書き出し</a>」をクリックして、フィールド、カスタムフィールド、API の名前のリストを確認します。</li>
<li><a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">カスタムフィールド</a>はいくつありますか？</li>
<li>使用されているフィールドの数
<br/>     フィールドアクションドロップダウンで「<a href="/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md" target="_blank">使用者を書き出し</a>」を選択して、フィールドの関連アセットを確認します。</li>
<li>Marketo Engage と CRM の間で同期されるフィールドはいくつありますか？</li>
<li>CRM フィールドは適切なオブジェクトと同期されていますか？</li>
<li>個人の詳細に<a href="/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md" target="_blank">カスタムビューセット</a>はありますか？ 必要ありますか？</li>
<li>ソースにもとづくフィールドの命名規則はありますか？
<br/>     ない場合は、この実装を検討してください。</li>
<li>ブロックされている<a href="/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md" target="_blank"> フィールドはありますか？</a>
<br/>     ある場合は、この理由を必ず理解してください。</li></td>
  </tr>
  <tr>
   <td>カスタムアクティビティ</td>
   <td><li><a href="/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md" target="_blank">カスタムアクティビティ</a>はありますか？
<br/>     その場合は、クリックスルーして、Marketo のフォーム、メール、ランディングページに関連していないアクティビティを理解してください。</li></td>
  </tr>
  <tr>
   <td>カスタムオブジェクト</td>
   <td><li><a href="/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md" target="_blank">カスタムオブジェクト</a>はいくつありますか？ CRM とどのように同期しますか？</li>
<li>これらのカスタムオブジェクトは、プログラムやリストクエリでどのように利用されていますか？</li></td>
  </tr>
 </tbody>
</table>

## メール {#email}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">エリア</th>
   <th>レビューフォーカス</th>
  </tr>
  <tr>
   <td>メールのデフォルト設定</td>
   <td><li>管理者／メールで、デフォルト設定（例：<a href="/help/marketo/product-docs/administration/email-setup/change-the-default-from-email-and-from-label.md" target="_blank">「差出人」メール／ラベル</a>、<a href="/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md" target="_blank">ブランディングドメイン</a>、<a href="/help/marketo/product-docs/administration/email-setup/edit-the-unsubscribe-message.md" target="_blank">購読解除メッセージ</a>など）はすべて最新ですか？</li></td>
  </tr>
 </tbody>
</table>

## 統合 {#integrations}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">エリア</th>
   <th>レビューフォーカス</th>
  </tr>
  <tr>
   <td>CRM</td>
   <td><li>どの CRM と同期していますか （Salesforce、 MS Dynamics、 Veeva など）？</li>
<li><a href="https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758" target="_blank">カスタム同期</a>を利用していますか？</li>
<li>[Salesforce のみ] インスタンスにカスタム同期フィルターが実装されていますか？
<p><img src="assets/note-icon.png" alt="メモアイコン"> メモ：カスタム同期フィルターを特定したり、カスタム同期ルールの実装をリクエストする場合は、Adobe サポートにお問い合わせください。</li></td>
  </tr>
  <tr>
   <td>ランディングページ</td>
   <td><li><a href="/help/marketo/product-docs/administration/settings/edit-landing-page-settings.md" target="_blank">ドメインをどのように設定</a>していますか？</li>
   <li>ホームページをどのように設定していますか？</li>
<li><a href="/help/marketo/product-docs/administration/settings/set-a-fallback-page.md" target="_blank">フォールバックをどのように設定</a>していますか？</li>
<li>フォームの事前入力は有効になっていますか？</li>
<li><a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/enable-personalized-urls-for-your-account.md" target="_blank">パーソナライズされた URL</a> は有効になっていますか？</li>
<li><a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-actions/redirect-a-marketo-landing-page-to-another-page.md" target="_blank">リダイレクト</a>用のルールは設定されていますか？</li>
<li>ドメインエイリアスは設定されていますか？ ドメインエイリアスの利用方法を追跡していますか？</li>
<li>ランディングページ </a>の<a href="https://nation.marketo.com/t5/knowledgebase/setting-up-secured-domains-for-marketo-landing-pages-first-time/ta-p/250370" target="_blank"> セキュアドメインは有効ですか？
<br/>ランディングページアセットに「http」URL が含まれているかどうかを確認します。</li></td>
  </tr>
  <tr>
   <td>Munchkin</td>
   <td><li>Web サイト（Marketo Engage ランディングページ以外）に <a href="/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md" target="_blank">Munchkin トラッキングコード</a>は設置されていますか？</li>
<li>「<a href="/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md" target="_blank">トラックしない</a>」ブラウザーリクエストは有効になっていますか？</li>
<li><a href="https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking" target="_blank">Munchkin API</a> は設定されていますか？
<p><img src="assets/tip-icon.png" alt="ヒントアイコン">ヒント：munchkin コードがweb サイト上のどこにあるかに関するドキュメントがない場合は、<a href="/help/marketo/product-docs/reporting/basic-reporting/report-types/web-page-activity-report.md" target="_blank">Web ページ アクティビティレポート </a>を作成して、すべてのURLを表示できます。</li></td>
  </tr>
  <tr>
   <td>Web サービス</td>
   <td><li><a href="/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md" target="_blank">IP 制限</a>は有効になっていますか？ そうすべきでしょうか？</li>
<li>インスタンスで API 呼び出しを行っているのは、どのユーザ／アプリですか？</li>
<li>API 呼び出しの回数制限を超えていますか、それとも超えそうですか？
<br/>     その場合は、API 呼び出し回数を増やすか、インスタンスを監査して API 呼び出しを停止することを検討してください。</li></td>
  </tr>
  <tr>
   <td>Adobe Dynamic Chat（該当する場合）</td>
<td>次の手順を実行するには、<a href="https://adminconsole.adobe.com/" target="_blank">Adobe Admin Console</a> にアクセスする必要があります。 Adobe IDをまだ設定していない場合は、<a href="https://helpx.adobe.com/jp/manage-account/using/create-update-adobe-id.html" target="_blank">その方法については、こちらを参照してください</a>。
<br/>
<li><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.md" target="_blank">Dynamic Chat 製品管理者</a>の招待を受け入れましたか？ メールは、Marketo Engage インスタンスでDynamic Chatが有効になっていて、システム管理者として指定されたときに送信されます。
<br/>     そうでない場合は、インボックスでウェルカムメールを探し、Adobe ID を設定する招待を受け入れます。</li>
<li>Adobe Admin Console の Dynamic Chat 製品プロファイルに<a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user" target="_blank">必要なユーザ</a>を追加しましたか？
<li>対象となるユーザの Adobe ID に、Dynamic Chat 製品プロファイルが追加されていることを確認してください。 「Dynamic Chat にアクセス」ロールが製品プロファイルに追加されている場合、Marketo Engage／管理／ユーザ＆ロールでこのロールを割り当てることはできません。</li>
<li>「製品プロファイル」タブで、デフォルトのプロファイル権限は組織のニーズと一致していますか？<br/>
そうでない場合は、特定のプロファイルの権限を編集します。 </li>
<li>複数のサブスクリプションがある場合、ユーザは正しいサブスクリプションに追加されていますか？</li>
<br>
ユーザ＆ロール設定の監査が終了したら、Dynamic Chat にログインして監査を続行します。
<li>Dynamic Chat に <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md" target="_blank">Marketo Engage インスタンスを接続</a>しましたか？</li>
<li>定義済み権限を持つ 5 つのデフォルトプロファイルは組織に適用できますか？<br/>
     そうでない場合は、Dynamic Chat</a>で<a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#edit-existing-permissions" target="_blank">編集できます。 また、カスタムの権限セットを備えた<a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#create-a-profile" target="_blank">カスタムプロファイルを作成</a>することもできます。</li>
<li>ユーザに Dynamic Chat へのアクセス権を付与するには、管理／ユーザ＆ロール／ロールで該当する Marketo Engage ロールの「Dynamic Chat にアクセス」をオンにしましたか？
<br/><img src="assets/note-icon.png" alt="メモアイコン"> メモ：「管理者」および「マーケティングユーザ」のロールには、Dynamic Chat へのアクセス権が必要です。</li>
</td>
  </tr>
  <td>Marketo セールスインサイト（該当する場合）</td>
   <td><li><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">MSI パッケージはインストール</a>されていますか？</li>
<li><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">セールスインサイトの最新バージョンにアップグレード</a>しましたか？</li>
<li>セールスインサイトの設定は完了しましたか？ <br/>     エンタープライズ／無制限ユーザは<a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">こちらをクリック</a>、プロフェッショナルユーザは<a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">こちらをクリック</a>してください。</li>
<li>購入したシート数に基づいて<a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">ユーザにアクセス権を付与</a>しましたか？</li>
<li><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md" target="_blank">星と炎</a>はカスタマイズされていますか？</li></td>
  </tr>
  <tr>
   <td>Launchpoint（該当する場合）</td>
   <td><li>どのサービス（例：<a href="/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md" target="_blank">BrightTALK</a>、<a href="/help/marketo/product-docs/administration/additional-integrations/connect-brighttalk-to-marketo.md" target="_blank">Zoom</a> など）を設定しましたか？ 有効期限が近いものはありますか？</li>
<li>統合では <a href="https://nation.marketo.com/t5/knowledgebase/viewing-your-number-of-api-calls-to-marketo/ta-p/254256" target="_blank">API 呼び出しがいくつ</a>使用されていますか？</li>
<li>ユースケースに適した統合が行われていますか？</li></td>
  </tr>
  <tr>
   <td>Web フック（該当する場合）</td>
   <td><li><a href="/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md" target="_blank">どのような接続</a>を設定しましたか？</li>
<li>使用中でなくなったものはありますか？</li></td>
  </tr>
  <tr>
   <td>モバイルアプリ（該当する場合）</td>
   <td><li>どの<a href="/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md" target="_blank">モバイルアプリ</a>がありますか？</li>
<li><a href="/help/marketo/product-docs/mobile-marketing/push-notifications/adding-a-new-test-device.md" target="_blank">テストデバイス</a>を追加しましたか？</li></td>
  </tr>
 </tbody>
</table>

## アイデアスペース {#treasure-chest}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">エリア</th>
   <th>レビューフォーカス</th>
  </tr>
  <tr>
   <td>アイデアスペース</td>
   <td><li><a href="/help/marketo/product-docs/administration/settings/enable-or-disable-treasure-chest-features.md" target="_blank">アイデアスペース</a>の何がオンになっていますか？</li>
<li>オンまたはオフにする必要がある機能はありますか？</li></td>
  </tr>
  <tr>
   <td>キャンペーンインスペクター</td>
   <td><li><a href="/help/marketo/product-docs/administration/settings/campaign-inspector.md" target="_blank">キャンペーンインスペクター</a>はオンになっていますか？
<br/>アクティブなキャンペーン、CRM と同期しているキャンペーン、レコードを削除しているキャンペーンを簡単に識別できるようにすることを考慮してください。</li></td>
  </tr>
 </tbody>
</table>

## アラートと更新 {#alerts-and-updates}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">エリア</th>
   <th>レビューフォーカス</th>
  </tr>
  <tr>
   <td>Marketo Engage ステータスの更新</td>
   <td><li>インスタンスでは、<a href="https://nation.marketo.com/t5/knowledgebase/how-to-subscribe-to-status-page-notifications/ta-p/296749" target="_blank">Marketo Engage ステータスの更新</a>を購読していますか？</li></td>
  </tr>
  <tr>
   <td>アラート</td>
   <td><li>Marketo Engage から内部チームに<a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md" target="_blank">アクティブなアラート</a>が送信されていますか？</li>
<li>「はい」の場合、これらのアラートは適切に機能していますか？</li></td>
  </tr>
  <tr>
   <td>通知</td>
   <td><li>適切な管理者<a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md" target="_blank">通知</a>を購読していますか？</li></td>
  </tr>
 </tbody>
</table>
