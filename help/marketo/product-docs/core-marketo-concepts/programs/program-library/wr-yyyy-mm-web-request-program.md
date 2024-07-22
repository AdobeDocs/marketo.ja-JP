---
description: WR-YYYY-MM-Web リクエストプログラム - Marketo ドキュメント – 製品ドキュメント
title: WR-YYYY-MM-web リクエストプログラム
feature: Programs
exl-id: 4acaa2d0-3329-4027-acbd-ae2e0ec6f7c5
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 16%

---

# WR-YYYY-MM-web リクエストプログラム {#wr-yyyy-mm-web-request-program}

これは、Marketo Engageのデフォルトプログラムを使用した、連絡先リクエスト、見積もりリクエスト、デモリクエスト、体験版リクエストフォームに最適なプログラムの例です。 Marketoのランディングページで使用することも、Marketo以外のランディングページに埋め込まれたフォームとして使用することもできます。 フォームの送信時に、指定した個人にアラートメールが送信されます。

詳細な手順に関するサポートやプログラムのカスタマイズについては、Adobeアカウントチームに問い合わせるか、[Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} のページを参照してください。

## チャネルサマリ {#channel-summary}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>チャネル</th> 
   <th>メンバーシップのステータス</th>
   <th>アナリティクス動作</th>
   <th>プログラムのタイプ</th>
  </tr> 
  <tr> 
   <td>ウェブリクエスト</td> 
   <td>01 - エンゲージメント – 成功</td>
   <td>包含</td>
   <td>デフォルト</td>
  </tr>
 </tbody> 
</table>

## プログラムには、次のAssetsが含まれています {#program-contains-the-following-assets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>タイプ</th> 
   <th>テンプレート名</th>
   <th>アセット名</th>
  </tr>
  <tr> 
   <td>フォーム</td> 
   <td> </td>
   <td>FM-WebRequestForm</td>
  </tr>
  <tr> 
   <td>メール</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">クイックスタートメールテンプレート</a></td>
   <td>Alert-WebRequest</td>
  </tr>
  <tr> 
   <td>ランディングページ</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">クイックスタート LP テンプレート</a></td>
   <td>01 - LP - リクエスト</td>
  </tr>
  <tr> 
   <td>ランディングページ</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">クイックスタート LP テンプレート</a></td>
   <td>02 - LP – ありがとうございました</td>
  </tr>
  <tr> 
   <td>ローカル報告書</td> 
   <td> </td>
   <td>ランディングページの効果</td>
  </tr>
   <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>Web リクエストからの新しいユーザー</td>
  </tr>
   <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>ウェビナーの新しいユーザー</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>Assets – すべてのクリエイティブアセットが格納されています 
<br/> （アラートとランディングページのサブフォルダー）</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>キャンペーン – すべてのスマートキャンペーンを格納します。</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>レポート</td>
  </tr>
 </tbody> 
</table>

![](assets/wr-yyyy-mm-web-request-program-1.png)

## 含まれるマイトークン {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>トークンのタイプ</th> 
   <th>トークン名</th>
   <th>値</th>
  </tr>
  <tr> 
   <td>テキスト</td> 
   <td><code>{{my.Request-Type}}</code></td>
   <td>お問い合わせ</td>
  </tr>
  <tr> 
   <td>テキスト</td> 
   <td><code>{{my.ALERT-FromAddress}}</code></td>
   <td>PlaceholderFrom.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>テキスト</td> 
   <td><code>{{my.ALERT-FromName}}</code></td>
   <td><code><--My From Name Here--></code></td>
  </tr>
  <tr> 
   <td>テキスト</td> 
   <td><code>{{my.ALERT-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>テキスト</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>My.ThankYouPageURL?http://なし</td>
  </tr>
 </tbody> 
</table>

## 競合ルール {#conflict-rules}

* **プログラムタグ**
   * このサブスクリプションにタグを作成 – _推奨_
   * 無視

* **同じ名前のランディングページテンプレート**
   * 元のテンプレートのコピー
   * 宛先テンプレートの使用 – _推奨_

* **同じ名前の画像**
   * どちらのファイルも保持する
   * このサブスクリプションの項目を置き換える – _推奨_

* **同じ名前のメールテンプレート**
   * どちらのテンプレートも保持する
   * 既存のテンプレートを置換 – _推奨_

## ベストプラクティス {#best-practices}

* ウェビナープログラムを読み込んだ後、フォームをローカルアセットから Design Studio にあるグローバルアセットに移動します。
   * フォームの数を減らし、Design Studio からより多くのグローバルアセットを利用することで、プログラムの設計と管理ガバナンスの拡張性が向上します。 また、フィールド、オプトイン言語など、定期的にコンプライアンスを更新する柔軟性も備えています。

* 読み込んだプログラムでテンプレートを更新して現在のブランドのテンプレートを利用するか、スニペットまたは適切なロゴ/フッター情報を追加して、新しく読み込んだテンプレートを更新し、ブランドを反映させることを検討してください。

* 命名規則に合わせるために、このプログラムの例の命名規則を更新することを検討してください。

>[!NOTE]
>
>必要に応じて、プログラムテンプレートとプログラムを使用するたびにマイトークン値を必ず更新してください。

>[!IMPORTANT]
>
>URL を参照するマイトークンにhttp://またはhttps://を含めることはできません。含めない場合、リンクがアセット内で適切に機能しません。
