---
description: Marketo LP に関する内容 — Marketoドキュメント — 製品ドキュメント
title: Marketo LP のコンテンツ
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 661a41eb0c5c43541a63a36c31837b35f516d827
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 12%

---

# Marketo LP のコンテンツ {#content-on-marketo-lp}

プログラム名： CT-YYYY-MM-Content on Marketo LP

このサンプルリファレンスは、Marketoのデフォルトプログラムを利用するMarketoフォームを使用したMarketoランディングページを活用するコンテンツプログラムであるように設計されています。 フォームは、コンテンツ/オファーにアクセスするためのものです。 オファーへのリンクは、「ありがとうございます」ページに表示したり、「ありがとうございます」E メールに送信したり、両方に送信したりできます。 戦略に関するサポートやプログラムのカスタマイズについては、Adobeアカウントチームにお問い合わせいただくか、 [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) ページに貼り付けます。

**チャネルサマリ**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>チャネル</th> 
   <th>メンバーシップステータス</th>
   <th>アナリティクス動作</th>
   <th>プログラムのタイプ</th>
  </tr> 
  <tr> 
   <td>Web コンテンツ</td> 
   <td>01 — メンバー 
<br/>02-Engaged-Success</td>
   <td>包含</td>
   <td>デフォルト</td>
  </tr>
 </tbody> 
</table>

**プログラムには次のアセットが含まれています：**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>タイプ</th> 
   <th>テンプレート名</th>
   <th>アセット名</th>
  </tr> 
  <tr> 
   <td>メール</td> 
   <td>クイックスタートメールテンプレート</td>
   <td>01-Email-Thank You</td>
  </tr>
  <tr> 
   <td>ランディングページ</td> 
   <td>クイックスタート LP テンプレート</td>
   <td>01 - LP — 登録</td>
  </tr>
  <tr> 
   <td>ランディングページ</td> 
   <td>クイックスタート LP テンプレート</td>
   <td>02 - LP — ありがとうございます</td>
  </tr>
  <tr> 
   <td>フォーム</td> 
   <td> </td>
   <td>コンテンツ登録フォーム</td>
  </tr>
  <tr> 
   <td>ローカルレポート</td> 
   <td> </td>
   <td>メールの効果</td>
  </tr>
  <tr> 
   <td>ローカルレポート</td> 
   <td> </td>
   <td>ランディングページの効果</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>01 入力済みフォーム</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>02 — エンゲージ済み（プログラム成功）</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>アセット — すべてのクリエイティブアセットを格納します。 
<br/>（メールおよびランディングページのサブフォルダー）  </td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>キャンペーン — すべてのスマートキャンペーンを格納</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>レポート</td>
  </tr>
 </tbody> 
</table>

SCREENSHOT — プログラムの画像

**含まれるマイトークン：**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>トークンのタイプ</th> 
   <th>トークン名</th>
   <th>値</th>
  </tr> 
  <tr> 
   <td>リッチテキスト</td> 
   <td><code>{{my.Content-Description}}</code></td>
   <td>ダブルクリックして詳細を表示  
<br/><code><--My Content Description Here--></code> 
<br/>このコンテンツの説明は、プログラムレベルの「マイトークン」タブで編集します。 
<br/>学習内容： 
<li>箇条書き 1</li>
<li>箇条書き 2</li>
<li>箇条書き 3</li></td>
  </tr>
  <tr> 
   <td>テキスト</td> 
   <td><code>{{my.Content-Title}}</code></td>
   <td><code><--My Content Title Here--></code></td>
  </tr>
  <tr> 
   <td>テキスト</td> 
   <td><code>{{my.Content-Type}}</code></td>
   <td><code><--My Content Type Here--></code></td>
  </tr>
  <tr> 
   <td>テキスト</td> 
   <td><code>{{my.Content-URL}}</code></td>
   <td>my.ContentURL?without=http://</td>
  </tr>
  <tr> 
   <td>テキスト</td> 
   <td><code>{{my.Email-FromAddress}}</code></td>
   <td>PlaceholderFrom.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>テキスト</td> 
   <td><code>{{my.Email-FromName}}</code></td>
   <td><code><--My From Name Here--></code></td>
  </tr>
  <tr> 
   <td>テキスト</td> 
   <td><code>{{my. Email-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>テキスト</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>My.ThankYouPageURL?http://</td>
  </tr>
 </tbody> 
</table>

>[!CAUTION]
>
>デフォルトの競合規則に関するプログラムのインポート手順を参照してください。

**インポートに推奨されるデフォルトの競合規則：**

* プログラムタグ
   * この配信登録におけるタグを作成 （デフォルト） — 推奨
   * 無視する

* 同じ名前のランディングページテンプレート
   * 元のテンプレートをコピー（デフォルト）
   * 宛先テンプレートを使用 — 推奨

* 同じ名前の画像
   * どちらのファイルも保持する  (デフォルト)
   * この配信登録の項目を置換 — 推奨

* 同じ名前のメールテンプレート
   * 両方のテンプレートを保持（デフォルト）
   * 既存のテンプレートを置き換え — 推奨

SCREENSHOT — デフォルトの競合ルールの画像

**推奨ベストプラクティス：**

* Marketoコンサルティングのベストプラクティスでは、コンテンツプログラムの読み込み後に、フォームをローカルアセットからMarketo Engageの Design Studio にあるグローバルアセットに移動することをお勧めします。
   * フォームの数を減らし、Design Studio からより多くのグローバルアセットを利用することで、プログラムのデザインと管理ガバナンスにおけるスケーラビリティを高めることができます。 また、フィールド、オプトイン言語などに対する定期的なコンプライアンス更新を柔軟におこなうこともできます。

* 現在ブランド化されているテンプレートを利用するには、読み込んだプログラムでテンプレートを更新するか、スニペットや適切なロゴおよびフッター情報を追加して、新しく読み込んだテンプレートをブランドに合わせて更新します。

* 必要に応じて、命名規則に合わせて、このプログラムテンプレートの命名規則を更新することを検討してください。

* 必要に応じて、プログラムテンプレートのマイトークン値と、プログラムを使用するたびに、必要に応じて値を更新します。

* 戦略に関するサポートやプログラムのカスタマイズについては、Adobeのアカウントチームにお問い合わせいただくか、 [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) ページに貼り付けます。

>[!TIP]
>
>成功を追跡するための「02-Engaged」キャンペーンを忘れずに有効化してください。 これは、フォームがライブになり、電子メールが送信される前に行います。

>[!NOTE]
>
>URL を参照する My Tokens にhttp://やhttps://を含めることはできません。含めないと、リンクがアセット内で適切に機能しません。
