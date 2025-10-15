---
description: NUR-YYYY-MM-Advanced Nurture - Marketo ドキュメント – 製品ドキュメント
title: NUR-YYYY-MM-高度な育成
feature: Programs
exl-id: bd9c6605-a13f-4c73-aaa8-eca43cfcc950
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 16%

---

# NUR-YYYY-MM-高度な育成 {#nur-yyyy-mm-advanced-nurture}

Marketo Engageエンゲージメントプログラムを活用した高度人材育成プログラムの一例です。 ネストされたメールプログラムは、既に消費したコンテンツをユーザーが受信するのを防いだり、各ストリームで消費するコンテンツのタイプを制御したりできます。 アトリビューションレポートは、ネストされた電子メールプログラムごとに実行できます。 チャネル：「ナーチャー」と、ネストされたメールプログラム用の専用「ナーチャー E メール」チャネルが、Marketo Engageのメールプログラムを利用して 1 通のニュースレターメールを送信します。 メールには、A/B テストを含めることも、含めないこともできます。

詳細な方法に関するサポートや、プログラムのカスタマイズに関するヘルプについては、Adobe アカウントチームに問い合わせるか、[Adobe Professional Services](https://business.adobe.com/jp/customers/consulting-services/main.html){target="_blank"} のページを参照してください。

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
   <td>ナーチャリング</td>
   <td>01 - メンバー
<br/>02 - エンゲージメント – 成功</td>
   <td>包含</td>
   <td>エンゲージメント</td>
  </tr>
  <tr>
   <td>Nurture Email</td>
   <td>01 - スキップ
<br/>02 – 送信済み
<br/>03 - エンゲージメント – 成功</td>
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
   <td>ネストされたプログラム</td>
   <td> </td>
   <td>01 - トピック X</td>
  </tr>
  <tr>
   <td>ネストされたプログラム</td>
   <td> </td>
   <td>02 - トピック Y</td>
  </tr>
  <tr>
   <td>ネストされたプログラム</td>
   <td> </td>
   <td>03 - トピック Z</td>
  </tr>
  <tr>
   <td>メール</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">クイックスタートメールテンプレート</a></td>
   <td>01 - メール（ネストされたプログラム内でライブ）</td>
  </tr>
   <tr>
   <td>メール</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">クイックスタートメールテンプレート</a></td>
   <td>02 - メール（ネストされたプログラム内でライブ）</td>
  </tr>
   <tr>
   <td>メール</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">クイックスタートメールテンプレート</a></td>
   <td>03 - メール（ネストされたプログラム内でライブ）</td>
  </tr>
  <tr>
   <td>ローカル報告書</td>
   <td> </td>
   <td>メールの効果</td>
  </tr>
  <tr>
   <td>ローカル報告書</td>
   <td> </td>
   <td>メールリンクの効果</td>
  </tr>
  <tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>01 - ナーチャリングに追加</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>02 – 育成の一時停止</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>03 – 育成の再開</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>04 - エンゲージ済み（プログラム成功）</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>00 - メールをスキップ（ネストされた各プログラム内にあります）</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>01 - メールの送信（ネストされた各プログラム内にあります）</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>02 - Engaged-Success （ネストされた各プログラム内に存在）</td>
  </tr>
  <tr>
   <td>フォルダー</td>
   <td> </td>
   <td>Assets（ネストされたプログラムを含む）およびアセットフォルダーは、メールを含むネストされたプログラムにも存在します）</td>
  </tr>
  <tr>
   <td>フォルダー</td>
   <td> </td>
   <td>ネストされたプログラム（Assets フォルダーに存在）</td>
  </tr>
  <tr>
   <td>フォルダー</td>
   <td> </td>
   <td>キャンペーン – すべてのスマートキャンペーンを親育成プログラムに格納します。キャンペーンフォルダーもネストされた各プログラムに配置されます</td>
  </tr>
  <tr>
   <td>フォルダー</td>
   <td> </td>
   <td>レポート</td>
  </tr>
 </tbody>
</table>

![](assets/nur-yyyy-mm-advanced-nurture-1.png)

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
   <td><code>{{my.Email-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
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

* 読み込んだプログラムでテンプレートを更新して現在のブランドのテンプレートを利用するか、スニペットまたは適切なロゴ/フッター情報を追加して、新しく読み込んだテンプレートを更新し、ブランドを反映させることを検討してください。

* 命名規則に合わせて、このプログラムの例の命名規則を更新することを検討してください。

* ナーチャリング頻度を一時停止および再開するためのルールが整っていることを確認します。 これらのスマートキャンペーンは、エンゲージメントプログラムがアクティブ化される前にアクティブ化またはスケジュールされる必要があります。

>[!NOTE]
>
>必要に応じて、プログラムテンプレートとプログラムを使用するたびにマイトークン値を必ず更新してください。

>[!TIP]
>
>成功をトラッキングするには、「04 - エンゲージメント済み（プログラム成功）」キャンペーンを必ずアクティブ化してください。 メールを送信する前に _こ_ を行います。
