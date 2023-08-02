---
description: ドキュメントを継承 1 - Marketoドキュメント — 製品ドキュメント
title: ドキュメント 1 を継承
hide: true
hidefromtoc: true
source-git-commit: 93be928e540fd50d92bef4ead3ea23519de18cce
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 11%

---

# ドキュメント 1 を継承 {#inherit-doc-1}

継承されたインスタンスの監査は、

別の管理者から既存のMarketo Engageインスタンスを継承したか。 その場合は、この記事があなたのためのものです。

>[!TIP]
>
>新規のMarketo Engageユーザーで、多くの用語に精通していない場合は、 [Marketo用語集](/help/marketo/getting-started/marketo-glossary.md){target="_blank"}.

## ユーザ&amp;ロール {#users-and-roles}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>エリア</th> 
   <th>レビューフォーカス</th>
   <th>列 3</th>
  </tr> 
  <tr> 
   <td>ユーザ</td> 
   <td><li>ユーザー数は？</li>
<li>期限切れになるユーザーはいますか？</li>
<li>ユーザーの削除に関するポリシーが会社にあるか。</li> 
<li>管理者権限を持つユーザーの数は？</li>
<li>これらのユーザーの役割を他の役割に変更する必要はありますか？</li> 
<li>このインスタンスの API ユーザーは誰ですか？</li></td>
   <td>3.1</td>
  </tr>
  <tr> 
   <td>ロール</td> 
   <td><li>役割はいくつありますか？</li>  
<li>各役割にはどの権限/アクセス権がありますか？ 何か調整すべきではありませんか？</li>
<li>1 つのロールにつき何人のユーザーが存在しますか？</li>
<li>ユーザーがログインする頻度はどれくらいですか？</li>
<li>各 API ユーザーは独自のユーザー役割を持っていますか。 そうでない場合は、トラブルシューティングを容易にするために、これを実装することを検討してください。</li> 
<li>ユーザーの役割と権限は、企業のデータのプライバシーポリシーに合っていますか。</li></td>
   <td>3.2</td>
  </tr>
  <tr> 
   <td>内部ドキュメント</td> 
   <td><li>組織でユーザーと役割が明確に定義されているか。</li>
<li>新しいユーザー/管理者を追加するプロセスは何ですか？</li></td>
   <td>3.3</td>
  </tr>
  <tr> 
   <td>サンドボックス（該当する場合）</td> 
   <td><li>サンドボックスインスタンスを持っているか。 その場合は、お使いのサンドボックスで上記のカテゴリを確認してください。</li>
<li>プログラムのインポートはサンドボックスにリンクされていますか？</li></td>
   <td>3.4</td>
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
   <td><li>インスタンスで作業しているのは誰ですか？</li></td>
   <td>3.1</td>
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
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Marketo Sales Insight（該当する場合）</td> 
   <td><li>次の条件を満たす <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">MSI パッケージがインストールされました</a>?</li>
<li>あなたがいる <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">Sales Insight の最新バージョンにアップグレード済み</a>?</li>
<li>Sales Insight の構成は完了していますか？</li>
<li>あなたがいる <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">ユーザーに対するアクセス権を付与</a> 購入したシート数に基づいて</li></td>
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
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
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
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
 </tbody> 
</table>
