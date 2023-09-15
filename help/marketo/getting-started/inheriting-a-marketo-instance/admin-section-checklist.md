---
description: 継承インスタンス管理チェックリスト — Marketoドキュメント — 製品ドキュメント
title: 継承されたインスタンスの管理者チェックリスト
hide: true
hidefromtoc: true
source-git-commit: d3a35d669eb54d020228ffdbdd7606a86abd18af
workflow-type: tm+mt
source-wordcount: '1566'
ht-degree: 6%

---

# 継承されたインスタンス：管理セクションのチェックリスト {#inherited-instance-admin-section-checklist}

以下のチェックリスト（各記事の下部にリンクされている後続のチェックリスト）は、Marketo Champions の入力を得てAdobe Professional Servicesでまとめられ、迅速に作業を進めるのに役立ちます。 また、チェックリストをダウンロードして、進行状況を追跡することもできます。

>[!TIP]
>
>新規のMarketo Engageユーザーで、多くの用語に精通していない場合は、 [Marketo Engage用語集](/help/marketo/getting-started/marketo-engage-glossary.md){target="_blank"}.

## Adobe Identity Management {#adobe-identity-management}

>[!NOTE]
>
>これは、にオンボーディングされたサブスクリプションにのみ適用されます [AdobeIdentity Managementシステム (IMS)](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"}. If your Marketo Engage subscription has not onboarded Adobe IMS yet, proceed with the [legacy user roles and permissions experience](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"} (Marketo Engage/管理者/ユーザーとロール )。

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">エリア</th> 
   <th>レビューフォーカス</th>
  </tr> 
  <tr> 
   <td>サブスクリプション</td> 
   <td><li>Marketo Engage配信登録がに移行されているか。 <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md" target="_blank">Adobe IMS</a> まだ？ 
<br/>     その場合、「Adobe Admin Console System Admin」の役割が「Adobe Admin Console」に付与されていますか。 組織内で誰がコンソールの管理者権限を持っているかが不明な場合は、<a href="https://helpx.adobe.com/contact.html" target="_blank">アドビカスタマーケア</a>にお問い合わせください。</li>
<li>「製品管理者のMarketo Engage」招待を受け入れましたか？ 役割がAdobe Admin Consoleで割り当てられると、電子メールが送信されます。
<br/>     そうでない場合は、を探します。 <a href="//help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md#" target="_blank">お知らせメール</a> を受信トレイに入れ、招待を受け入れてAdobe IDをアクティベートします。</li></td>
  </tr>
  <tr> 
   <td>製品プロファイル</td> 
   <td><li>すべての適切なユーザーがAdobe Admin ConsoleのMarketo Engageの製品プロファイルに割り当てられていますか。
<br/>     そうでない場合は、必ず <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md" target="_blank">ユーザーの追加/削除</a> Adobe Admin ConsoleのMarketo Engage製品プロファイルから。 製品プロファイルに追加されている場合、Marketo Engage/管理者/ユーザーとロールで、ユーザーの役割を割り当てることはできません。</li>
<p><img src="assets/note-icon.png" alt="メモアイコン"> 注意：望ましくないユーザーが複数の製品プロファイルに追加された場合は、すべての製品プロファイルからそのユーザーを削除する必要があります。 そうしないと、Marketo Engageにアクセスできます。</td>
  </tr>
  <tr> 
   <td>ユーザー管理 API</td> 
   <td><li>サブスクリプションでMarketo User Management API を使用しているか。
<br/>     その場合は、 <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html" target="_blank">Adobe IMSAPI</a> をクリックして、今後のユーザーの招待、更新、削除を行います。</li>
<p><img src="assets/note-icon.png" alt="メモアイコン"> 注意： 「役割の管理」はMarketo Engageのままです。Marketo User Management API は引き続き役割の管理に使用できます。</td>
  </tr>
 </tbody> 
</table>

## ユーザ&amp;ロール {#users-and-roles}

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">エリア</th>
   <th>レビューフォーカス</th>
  </tr> 
  <tr> 
   <td>ユーザ</td> 
   <td><img src="assets/note-icon.png" alt="メモアイコン"> 注意：サブスクリプションが既にAdobe IMSになっている場合は、Adobe Admin Consoleで次のユーザー管理レビューに進んでください。 それ以外の場合は、管理者/ユーザーとロール/Marketo Engageのユーザーに移動します。
   <p>
   <li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">ユーザー数</a> いるの？</li>
<li>以下の条件を満たす必要があるユーザーがいるか <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md#remove-a-user" target="_blank">削除済み</a>?</li>
<li>ユーザーの削除に関するポリシーが会社にあるか。</li> 
<li>ユーザーの数 <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">管理者権限</a>?</li>
<li>これらのユーザーのいずれかが <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">他の役割？</a></li> 
<li>誰が <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md" target="_blank">API ユーザー</a> このインスタンスで</li></td>
  </tr>
  <tr> 
   <td>ロール</td> 
   <td><img src="assets/note-icon.png" alt="メモアイコン"> 注意： MarketoをAdobeID と共に使用しているかどうかに関わらず、管理者/ユーザーとロール/ロールで、Marketo Engageのロール権限の確認に進みます。
   <p><li>役割はいくつありますか？</li>  
<li>What <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">permissions/access</a> 各役割には何がありますか？ 何か調整すべきではありませんか？</li>
<li>1 つのロールにつき何人のユーザーが存在しますか？</li>
<li>ユーザーの頻度 <a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">ログイン</a>?</li>
<li>各 API ユーザーが <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">独自のユーザーロール</a>? そうでない場合は、トラブルシューティングを容易にするために、これを実装することを検討してください。</li> 
<li>ユーザーの役割と権限は、規制への準拠 ( <a href="https://gdpr-info.eu/" target="_blank">GDPR</a>)? 企業データを実行 <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">プライバシーポリシー</a> ユーザーがMarketo Engageのユーザーデータをダウンロードして共有することを許可しますか？ 許可業務は必要ですか？</li></td>
  </tr>
  <tr> 
   <td>サポートユーザー</td> 
   <td><li>適切な <a href="/help/marketo/getting-started/setup/setup-steps.md#set-up-your-authorized-support-contacts" target="_blank">認証済み連絡先</a> 」がサポートポータルに表示される問題を修正しました。</li></td>
  </tr>
  <tr> 
   <td>内部ドキュメント</td> 
   <td><li>組織でユーザーと役割が明確に定義されているか。</li>
<li>新しいユーザー/管理者を追加するプロセスは何ですか？</li></td>
  </tr>
  <tr> 
   <td>サンドボックス（該当する場合）</td> 
   <td><li>次をお持ちですか： <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">サンドボックスインスタンス</a>?
   <br/>     その場合は、お使いのサンドボックスで上記のカテゴリを確認してください。</li>
<li>次に該当 <a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">プログラムの読み込み</a> サンドボックスにリンクされているか</li></td>
  </tr>
 </tbody> 
</table>

## 監査証跡 {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">エリア</th>
   <th>レビューフォーカス</th>
  </tr> 
  <tr> 
   <td>監査証跡</td> 
   <td><li><a href="/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md" target="_blank">作業中のユーザー</a> インスタンス内？</li></td>
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
   <td><li>数 <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md" target="_blank">ワークスペースおよび/またはパーティション</a> 持ってる？</li>
<li>各ワークスペースとパーティションの主な目的は何ですか。</li>
<li>次のいずれかを実行します。 <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-a-workspace.md" target="_blank">Workspaces</a> または <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-an-existing-person-partition.md" target="_blank">区分</a> 監査/変更が必要ですか？</li>
<li>ワークスペースとパーティションの関係は何ですか？</li>
<li>ユーザー数 <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.md" target="_blank">アクセス権を持つ</a> を各ワークスペースに追加しますか？</li></td>
  </tr>
  <tr> 
   <td>内部ドキュメント</td> 
   <td><li>ワークスペースとパーティションの定義方法</li>
<li>ワークスペースをインスタンスに追加したり、ユーザーをワークスペースに追加したりするには、どのようなプロセスを実行しますか？</li></td>
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
   <td>スマートキャンペーン設定</td> 
   <td><li><a href="/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md" target="_blank">制限があるか</a> スマートキャンペーンのサイズ 
   <br/>     そうでない場合は、追加することを検討します。 ワークフローでの過剰通信やデータベース全体の処理を避けるために、スマートキャンペーンの制限をデータベースの 25%に制限することをお勧めします。これは、ブランドを保護するだけでなく、インスタンスのパフォーマンスを保護します。</li></td>
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
   <td><li>あるか <a href="/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md" target="_blank">通信制限</a> その場で？ お客様のビジネスには、通信制限が必要なポリシーがありますか？</li>
<p><img src="assets/note-icon.png" alt="メモアイコン"> 注意：では、1 日に 1 回、7 日に 3 回のみ、通信を制限することをお勧めします。 <b>non</b>-<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md" target="_blank">操作</a> ブロックされたメール。</td>
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
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags.md" target="_blank">タグの数</a> いるの？ 使用中のタグの数 追加が必要な場合は、</li>
<li>プログラム内にタグは必要ですか？</li></td>
  </tr>
  <tr> 
   <td>チャネル</td> 
   <td><li><a href="/help/marketo/product-docs/administration/tags/create-a-program-channel.md" target="_blank">チャネル数</a> いるの？ 使用中のユーザー数</li>
<li>すべて <a href="/help/marketo/product-docs/administration/tags/hide-unhide-a-program-channel.md" target="_blank">チャネルプログラムのステータスに適したもの</a>? プログラム内の進行状況は表示されますか？</li>
<li>チャネルは特定のプログラムタイプに関連していますか？</li>
<li>各チャネルで成功と見なされるステータスはどれですか？ それらはマーケティング目標に合っていますか？</li>
<li>オペレーショナルチャネルは適切に使用されていますか？</li>
<li>高度なReport Builder（収益サイクルエクスプローラー/RCE）の場合、チャネル分析の動作は、期間原価を組み込んだプログラムプラクティスに合わせて設定されますか？</li></td>
  </tr>
  <tr> 
   <td>マーケティングカレンダー（該当する場合）</td> 
   <td><li>数 <a href="/help/marketo/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.md" target="_blank">カレンダーエントリタイプ</a> いるの？ まだ関連性があるのか？</li></td>
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
   <td><li>フィールドの数は？ 
   <br/>     クリック <a href="/help/marketo/product-docs/administration/field-management/export-a-list-of-all-marketo-api-field-names.md" target="_blank">フィールド名をエクスポート</a> をクリックして、フィールド、カスタムフィールドおよび API 名のリストを確認します。</li>
<li>数 <a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">カスタムフィールド</a> いるの？</li>
<li>使用されているフィールドの数 
<br/>     選択 <a href="/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md" target="_blank">エクスポート使用者</a> フィールドアクションドロップダウンで、フィールドの関連アセットを確認します。</li>
<li>Marketo Engageと CRM の間で同期されるフィールドの数</li>
<li>CRM フィールドは適切なオブジェクトに同期されていますか？</li>
<li>次の項目がありますか？ <a href="/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md" target="_blank">カスタムビューセット</a> 担当者の詳細について あるべきか？</li>
<li>ソースに基づいてフィールドの命名規則を設定しているか。 
<br/>     そうでない場合は、この実装を検討してください。</li>
<li>フィールドがありますか？ <a href="/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md" target="_blank">ブロック</a>? 
<br/>     その場合は、その理由を必ず理解してください。</li></td>
  </tr>
  <tr> 
   <td>カスタムアクティビティ</td> 
   <td><li>何かあるか <a href="/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md" target="_blank">カスタムアクティビティ</a>?
<br/>     その場合は、クリックスルーして、Marketoのフォーム、E メール、ランディングページに関連しないアクティビティを理解します。</li></td>
  </tr>
  <tr> 
   <td>カスタムオブジェクト</td> 
   <td><li>数 <a href="/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md" target="_blank">カスタムオブジェクト</a> いるの？ CRM と同期する方法を教えてください。</li>
<li>これらのカスタムオブジェクトは、プログラムやリストクエリでどのように利用されていますか？</li></td>
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
   <td><li>どの CRM と同期しますか？ Salesforce? MS Dynamics? Veeva?</li>
<li>を使用しているか <a href="https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758" target="_blank">カスタム同期</a>?</li>
<li>[Salesforce のみ ] インスタンスにカスタム同期フィルターが実装されているか。 
<p><img src="assets/note-icon.png" alt="メモアイコン"> 注意： Marketoサポートに連絡して、カスタム同期フィルターを特定するか、カスタム同期ルールの実装をリクエストしてください。</li></td>
  </tr>
  <tr> 
   <td>ランディングページ</td> 
   <td><li>とは <a href="/help/marketo/product-docs/administration/settings/edit-landing-page-settings.md" target="_blank">ドメインセット：</a>?</li>
   <li>ホームページは何として設定されますか。</li>
<li>とは <a href="/help/marketo/product-docs/administration/settings/set-a-fallback-page.md" target="_blank">フォールバックセット：</a>?</li>
<li>フォームの事前入力は有効になっていますか？</li>
<li>次に該当 <a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/enable-personalized-urls-for-your-account.md" target="_blank">パーソナライズ URL</a> 有効？</li>
<li>次のようにルールが設定されているか <a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-actions/redirect-a-marketo-landing-page-to-another-page.md" target="_blank">リダイレクト</a>?</li>
<li>ドメインエイリアスが存在するか。 ドメインエイリアスの利用方法を追跡していますか？</li>
<li>次に該当 <a href="https://nation.marketo.com/t5/knowledgebase/setting-up-secured-domains-for-marketo-landing-pages-first-time/ta-p/250370" target="_blank">ランディングページのセキュリティ保護されたドメイン</a> 有効？ 
<br/>     ランディングページアセットに「http」URL が含まれているかどうかを確認します。</li></td>
  </tr>
  <tr> 
   <td>Munchkin</td> 
   <td><li>Is your <a href="/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md" target="_blank">Munchkin トラッキングコード</a> を (Marketo以外の )Web サイトに追加した場合、</li>
<li>Is a <a href="/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md" target="_blank">追跡しない</a> ブラウザーリクエストが有効ですか？</li>
<li>Is your <a href="https://developers.marketo.com/javascript-api/lead-tracking/" target="_blank">Munchkin API</a> 設定済み？ 
<p><img src="assets/tip-icon.png" alt="ヒントアイコン">ヒント：Munchkin コードが Web サイト上にある場所に関するドキュメントが見つからない場合は、 <a href="/help/marketo/product-docs/reporting/basic-reporting/report-types/web-page-activity-report.md" target="_blank">ウェブページアクティビティレポート</a>.</li></td>
  </tr>
  <tr> 
   <td>Web サービス</td> 
   <td><li>次に該当 <a href="/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md" target="_blank">IP 制限</a> 有効？ そうなるべきか？</li>
<li>インスタンスで API 呼び出しをおこなっているのは、どのユーザー/アプリですか？</li>
<li>API 制限に達したか、それとも近いか。 
<br/>     その場合は、API 呼び出しを増やすか、インスタンスを監査して、API 呼び出しを停止することを検討してください。</li></td>
  </tr>
  <tr> 
   <td>Marketo Sales Insight（該当する場合）</td> 
   <td><li>次の条件を満たす <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">MSI パッケージがインストールされました</a>?</li>
<li>あなたがいる <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">Sales Insight の最新バージョンにアップグレード済み</a>?</li>
<li>Sales Insight の構成は完了していますか？ <br/>     Enterprise/Unlimited ユーザー <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">ここをクリック</a>、Professional ユーザー <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">ここをクリック</a>.</li>
<li>あなたがいる <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">ユーザーに対するアクセス権を付与</a> 購入したシート数に基づいて</li>
<li>次に該当 <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md" target="_blank">星と炎</a> カスタマイズ済み？</li></td>
  </tr>
  <tr> 
   <td>Launchpoint（該当する場合）</td> 
   <td><li>設定済みのサービス ( 例： <a href="/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md" target="_blank">BrightTALK</a>, <a href="/help/marketo/product-docs/administration/additional-integrations/connect-brighttalk-to-marketo.md" target="_blank">ズーム</a>など )? 彼らの有効期限が近いものはありますか？</li>
<li><a href="https://nation.marketo.com/t5/knowledgebase/viewing-your-number-of-api-calls-to-marketo/ta-p/254256" target="_blank">API 呼び出し数</a> 統合ではを使用していますか？</li>
<li>使用例に適した統合を実施しているか。</li></td>
  </tr>
  <tr> 
   <td>ウェブフック（該当する場合）</td> 
   <td><li><a href="/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md" target="_blank">接続</a> 準備は？</li>
<li>使用されなくなったものはありますか？</li></td>
  </tr>
  <tr> 
   <td>モバイルアプリ（該当する場合）</td> 
   <td><li>対象 <a href="/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md" target="_blank">モバイルアプリ</a> 持ってる？</li>
<li>次のいずれかを持つ <a href="/help/marketo/product-docs/mobile-marketing/push-notifications/adding-a-new-test-device.md" target="_blank">デバイスをテスト</a>  追加された？</li></td>
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
   <td><li>での表示 <a href="/help/marketo/product-docs/administration/settings/enable-or-disable-treasure-chest-features.md" target="_blank">宝箱</a>?</li>
<li>オンまたはオフにする必要がある機能はありますか？</li></td>
  </tr>
  <tr> 
   <td>キャンペーンインスペクター</td> 
   <td><li>次に該当 <a href="/help/marketo/product-docs/administration/settings/campaign-inspector.md" target="_blank">キャンペーンインスペクター</a> オン？
<br/>そうでない場合は、有効にして、アクティブなキャンペーン、CRM との同期、レコードの削除など、どのキャンペーンかを簡単に識別することを検討してください。</li></td>
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
   <td>Marketo Engageステータスの更新</td> 
   <td><li>インスタンスが次を購読しているか。 <a href="https://nation.marketo.com/t5/knowledgebase/how-to-subscribe-to-status-page-notifications/ta-p/296749" target="_blank">Marketo Engageステータスの更新</a>?</li></td>
  </tr>
  <tr> 
   <td>アラート</td> 
   <td><li>何かあるか <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md" target="_blank">アクティブなアラート</a> Marketo Engageから内部チームに送信された場合</li>
<li>該当する場合、これらのアラートは適切に機能していますか。</li></td>
  </tr>
  <tr> 
   <td>通知</td> 
   <td><li>適切な管理者を購読していますか？ <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md" target="_blank">通知</a>?</li></td>
  </tr>
 </tbody> 
</table>

<br> 

[継承されたインスタンスの監査：データベース►](/help/marketo/getting-started/inheriting-a-marketo-instance/database-checklist.md)
