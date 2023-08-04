---
description: ドキュメントを継承 1 - Marketoドキュメント — 製品ドキュメント
title: ドキュメント 1 を継承
hide: true
hidefromtoc: true
source-git-commit: b06d1d0f8101895ebefeb821150090aac3044870
workflow-type: tm+mt
source-wordcount: '1220'
ht-degree: 7%

---

# ドキュメント 1 を継承 {#inherit-doc-1}

継承されたインスタンスの監査は、次のように見える場合があります。

別の管理者から既存のMarketo Engageインスタンスを継承したか。 その場合、この記事はあなたのために…

継承されたインスタンスで迅速に習得できるよう、以下のチェックリストがMarketo Champions の入力と共に追加されました。

>[!TIP]
>
>新規のMarketo Engageユーザーで、多くの用語に精通していない場合は、 [Marketo用語集](/help/marketo/getting-started/marketo-glossary.md){target="_blank"}.

## ユーザ&amp;ロール {#users-and-roles}

<table> 
 <tbody> 
  <tr> 
   <th>エリア</th> 
   <th>レビューフォーカス</th>
   <th>列 3</th>
  </tr> 
  <tr> 
   <td>ユーザ</td> 
   <td><li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">ユーザー数</a> いるの？</li>
<li>期限切れになるユーザーはいますか？</li>
<li>ユーザーの削除に関するポリシーが会社にあるか。</li> 
<li>ユーザーの数 <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">管理者権限</a>?</li>
<li>これらのユーザーのいずれかが <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">他の役割？</a></li> 
<li>このインスタンスの API ユーザーは誰ですか？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>ロール</td> 
   <td><li>役割はいくつありますか？</li>  
<li>What <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">permissions/access</a> 各役割には何がありますか？ 何か調整すべきではありませんか？</li>
<li>1 つのロールにつき何人のユーザーが存在しますか？</li>
<li>ユーザーの頻度 <a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">ログイン</a>?</li>
<li>各 API ユーザーが <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">独自のユーザーロール</a>? そうでない場合は、トラブルシューティングを容易にするために、これを実装することを検討してください。</li> 
<li>ユーザーの役割と権限を企業データに合わせて調整する <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">プライバシーポリシー</a>?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>内部ドキュメント</td> 
   <td><li>組織でユーザーと役割が明確に定義されているか。</li>
<li>新しいユーザー/管理者を追加するプロセスは何ですか？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>サンドボックス（該当する場合）</td> 
   <td><li>次をお持ちですか： <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">サンドボックスインスタンス</a>? その場合は、お使いのサンドボックスで上記のカテゴリを確認してください。</li>
<li>次に該当 <a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">プログラムの読み込み</a> サンドボックスにリンクされているか</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## 監査証跡 {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>エリア</th> 
   <th>レビューフォーカス</th>
   <th>列 3</th>
  </tr> 
  <tr> 
   <td>監査証跡</td> 
   <td><li><a href="/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md" target="_blank">作業中のユーザー</a> インスタンス内？</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## ワークスペースとパーティション {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>エリア</th> 
   <th>レビューフォーカス</th>
   <th>列 3</th>
  </tr> 
  <tr> 
   <td>ワークスペースとパーティション</td> 
   <td><li>ワークスペースやパーティションの数は？</li>
<li>各ワークスペースとパーティションの主な目的は何ですか。</li>
<li>監査または変更が必要か</li>
<li>ワークスペースとパーティションの関係は何ですか？</li>
<li>各ワークスペースにアクセスできるユーザーの数</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>内部ドキュメント</td> 
   <td><li>ワークスペースとパーティションの定義方法</li>
<li>インスタンスにワークスペースを追加したり、ワークスペースにユーザーを追加したりするプロセスは何ですか？</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## スマートキャンペーン {#smart-campaigns}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>エリア</th> 
   <th>レビューフォーカス</th>
   <th>列 3</th>
  </tr> 
  <tr> 
   <td>スマートキャンペーン設定</td> 
   <td><li>スマートキャンペーンのサイズに制限はありますか？</li>
<li>そうでない場合は、追加することを検討します。 過剰な通信を避けたり、ワークフローでデータベース全体を処理したりするのを防ぐため、スマートキャンペーンの制限をデータベースの 25%に制限することは、ブランドを保護するだけでなく、インスタンスのパフォーマンスを保護するのに役立ちます。</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## 通信制限 {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>エリア</th> 
   <th>レビューフォーカス</th>
   <th>列 3</th>
  </tr> 
  <tr> 
   <td>通信制限</td> 
   <td><li>制限が設けられているか。 お客様のビジネスには、通信制限が必要なポリシーがありますか？</li>
<li>Adobeでは、1 日に 1 件、7 日に 3 件に制限することをお勧めします。非運用 E メールはブロックされます。</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## タグ {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>エリア</th> 
   <th>レビューフォーカス</th>
   <th>列 3</th>
  </tr> 
  <tr> 
   <td>タグ</td> 
   <td><li>タグの数は？ 使用中のタグの数 追加が必要な場合は、</li>
<li>プログラム内にタグは必要ですか？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>チャネル</td> 
   <td><li>チャネルはいくつありますか？ 使用中のユーザー数</li>
<li>すべてのチャネルプログラムのステータスは適切ですか？ プログラム内の進行状況は表示されますか？</li>
<li>チャネルは特定のプログラムタイプに関連していますか？</li>
<li>各チャネルで成功と見なされるステータスはどれですか？ それらはマーケティング目標に合っていますか？</li>
<li>オペレーショナルチャネルは適切に使用されていますか？</li>
<li>高度なReport Builder（収益サイクルエクスプローラー\RCE）の場合、チャネル分析の動作は、期間原価を組み込んだプログラムプラクティスに合わせて設定されていますか？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>マーケティングカレンダー（該当する場合）</td> 
   <td><li>カレンダーエントリの種類はいくつありますか？ まだ関連性があるのか？</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## データベース管理 {#database-management}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>エリア</th> 
   <th>レビューフォーカス</th>
   <th>列 3</th>
  </tr> 
  <tr> 
   <td>フィールド管理</td> 
   <td><li>フィールドの数は？ [ フィールド名の書き出し ] をクリックして、フィールド、カスタムフィールド、および API 名のリストを確認します。</li>
<li>カスタムフィールドはいくつありますか？</li>
<li>使用されているフィールドの数 「フィールドアクション」ドロップダウンで「エクスポート実行者」を選択して、フィールドの関連アセットを確認します。</li>
<li>Marketo Engageと CRM の間で同期されるのはいくつですか？</li>
<li>CRM フィールドは適切なオブジェクトに同期されていますか？</li>
<li>担当者詳細に対して設定されたカスタムビューはありますか？ あるべきか？</li>
<li>ソースに基づいてフィールドの命名規則を設定しているか。 そうでない場合は、この実装を検討してください。</li>
<li>ブロックされているフィールドはありますか？ その理由を必ず理解してください。</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>カスタムアクティビティ</td> 
   <td><li>カスタムアクティビティはありますか？</li>
<li>その場合は、クリックスルーして、Marketoのフォーム、E メール、ランディングページに関連しないアクティビティを理解します。</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>カスタムオブジェクト</td> 
   <td><li>カスタムオブジェクトはいくつありますか？ CRM と同期する方法を教えてください。</li>
<li>これらのカスタムオブジェクトは、プログラムやリストクエリでどのように利用されていますか？</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## 統合 {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>エリア</th> 
   <th>レビューフォーカス</th>
   <th>列 3</th>
  </tr> 
  <tr> 
   <td>CRM</td> 
   <td><li>どの CRM と同期しますか？ Salesforce? MS Dynamics? Veeva?</li>
<li>カスタム同期と双方向のどちらですか。 （KG：文法を固定し、重要度をチェック）</li>
<li>[Salesforce のみ ] インスタンスにカスタム同期フィルターが実装されているか。 Marketoサポートに連絡して、カスタム同期フィルターを特定するか、カスタム同期ルールの実装をリクエストします。</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>ランディングページ</td> 
   <td><li>ドメインセットの形式を教えてください。</li>
<li>フォールバックセットは何ですか？</li>
<li>ホームページは何として設定されますか。</li>
<li>フォームの事前入力は有効になっていますか？</li>
<li>パーソナライズされた URL は有効になっていますか？</li>
<li>リダイレクト用のルールは設定されていますか？</li>
<li>ドメインエイリアスが存在するか。 ドメインエイリアスの活用方法について説明していますか。</li>
<li>ランディングページのセキュリティ保護されたドメインは有効になっていますか？ ランディングページアセットに「http」URL が含まれているかどうかを確認します。</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Munchkin</td> 
   <td><li>Web サイト上の Munchkin トラッキングコード (Marketo以外 )。</li>
<li>「トラッキング拒否」ブラウザーリクエストは有効になっていますか？</li>
<li>Munchkin API は設定されていますか？ Munchkin コードが Web サイト上のどこにあるかに関するドキュメントが見つからない場合は、基本的な「Analytics」の「Web 分析レポート」を使用して、Munchkin コードが Web サイト上で配置されている場所を把握し、クイックビューを開始します。</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Web サービス</td> 
   <td><li>IP 制限は有効になっていますか？ そうなるべきか？</li>
<li>インスタンスで API 呼び出しをおこなっているのは、どのユーザー/アプリですか？</li>
<li>API 制限に達したか、それとも近いか。 その場合は、API 呼び出しを増やすか、インスタンスを監査して、API 呼び出しを停止することを検討してください。</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Marketo Sales Insight（該当する場合）</td> 
   <td><li>次の条件を満たす <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">MSI パッケージがインストールされました</a>?</li>
<li>あなたがいる <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">Sales Insight の最新バージョンにアップグレード済み</a>?</li>
<li>Sales Insight の構成は完了していますか？ Enterprise/Unlimited ユーザー <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">ここをクリック</a>、Professional ユーザー <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">ここをクリック</a>.</li>
<li>あなたがいる <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">ユーザーに対するアクセス権を付与</a> 購入したシート数に基づいて</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Launchpoint（該当する場合）</td> 
   <td><li>設定したサービス（ウェビナー、広告など）を教えてください。 彼らの有効期限が近いものはありますか？</li>
<li>統合では何回の API 呼び出しを使用しますか？</li>
<li>使用例に適した統合を実施しているか。</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>ウェブフック（該当する場合）</td> 
   <td><li>設定した接続は何ですか？</li>
<li>使用されなくなったものはありますか？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>モバイルアプリ（該当する場合）</td> 
   <td><li>どのモバイルアプリをお持ちですか？</li>
<li>追加されたテストデバイスはどれですか？</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## アイデアスペース {#treasure-chest}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>エリア</th> 
   <th>レビューフォーカス</th>
   <th>列 3</th>
  </tr> 
  <tr> 
   <td>アイデアスペース</td> 
   <td><li>宝箱の中で何が起こってる？</li>
<li>オンまたはオフにする必要がある機能はありますか？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>キャンペーンインスペクター</td> 
   <td><li>キャンペーンインスペクターはオンになっていますか？</li>
<li>そうでない場合は、有効にして、アクティブなキャンペーン、CRM との同期、レコードの削除を簡単に識別することを検討してください。</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## その他 {#miscellaneous}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>エリア</th> 
   <th>レビューフォーカス</th>
   <th>列 3</th>
  </tr> 
  <tr> 
   <td>Marketo Engageステータスの更新</td> 
   <td><li>インスタンスはMarketo Engageステータスの更新にサインアップしていますか？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>認証済み連絡先</td> 
   <td><li>サポートポータルで、許可された適切な連絡先を設定していますか？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>アラート</td> 
   <td><li>Marketo Engageから内部チームに送信されるアクティブなアラートはありますか？</li>
<li>該当する場合、これらのアラートは適切に機能していますか。</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>通知</td> 
   <td><li>適切な管理者通知を購読しているか。</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>
