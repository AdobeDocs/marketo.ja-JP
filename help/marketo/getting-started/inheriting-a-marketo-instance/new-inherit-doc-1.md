---
description: ドキュメントを継承 1 - Marketoドキュメント — 製品ドキュメント
title: ドキュメント 1 を継承
hide: true
hidefromtoc: true
source-git-commit: 3c7eb2fc2e64898e12f08743225c0b802bf97474
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 22%

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
   <td><li>制限が設けられているか。 お客様のビジネスには、通信制限が必要なポリシーがありますか？</li>
<li>Adobeでは、非オペレーショナル E メールをブロックして、1 日に 1 件、7 日に 3 件の通信を制限することをお勧めします。</li></td>
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

## タグ {#tags}

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

## データベース管理 {#database-management}

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

## 統合 {#integrations}

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
