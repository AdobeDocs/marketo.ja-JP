---
description: 継承されたインスタンスデザインスタジオのチェックリスト — Marketoドキュメント — 製品ドキュメント
title: 継承されたインスタンスデザインスタジオのチェックリスト
hide: true
hidefromtoc: true
source-git-commit: 30a7b16e20b6abdfe4f7c10000e64d556ba94116
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 4%

---

# 継承されたインスタンス：デザインスタジオチェックリスト {#inherited-instance-design-studio-checklist}

テンプレートを構造化し、グローバルフォーム、スニペット、画像およびファイルを作成すると、データエラーを最小限に抑えると共に、プログラムの作成ワークフローを合理化できます。

## ランディングページ {#landing-pages}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">エリア</th> 
   <th>レビューフォーカス</th>
  </tr> 
  <tr> 
   <td>グローバルランディングページ</td> 
   <td><li>グローバルな数 <a href="/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/understanding-free-form-vs-guided-landing-pages.md" target="_blank">ランディングページ</a> いるの？ プログラムで使われているのか？</li></td>
  </tr>
  <tr> 
   <td>テンプレート</td> 
   <td><li>数 <a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-templates/create-a-free-form-landing-page-template.md" target="_blank">ランディングページテンプレート</a> いるの？ 彼らは活用されているのですか？</li></td>
  </tr>
  <tr> 
   <td>テストグループ</td> 
   <td><li>数 <a href="/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-test-groups.md" target="_blank">ランディングページのテストグループ</a> 彼らは？ まだ関連性があるのか？</li></td>
  </tr>
   <tr> 
   <td>プライバシーとコンプライアンス</td> 
   <td><li>すべてのランディングページに適切なフッターがあるか。</li></td>
  </tr>
 </tbody> 
</table>

## 画像およびファイル {#images-and-files}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">エリア</th> 
   <th>レビューフォーカス</th>
  </tr> 
  <tr> 
   <td>命名規則</td> 
   <td><li>実行 <a href="/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md" target="_blank">画像とファイル</a> 一貫性のある命名規則を使用しますか？</li></td>
  </tr>
  <tr> 
   <td>フォルダー構造</td> 
   <td><li>画像とファイル <a href="/help/marketo/product-docs/demand-generation/images-and-files/organize-your-images-and-files-using-folders.md" target="_blank">適切に整理された</a> 簡単に検索できますか？</li></td>
  </tr>
  <tr> 
   <td>画像およびファイル</td> 
   <td><li>任意の画像またはファイルの実行 <a href="/help/marketo/product-docs/demand-generation/images-and-files/find-the-url-of-an-uploaded-image-or-file.md" target="_blank">web ページで参照されています</a> 更新が必要ですか？ 
   <p>例：ハードコードされた URL 構造 <a href="https://nation.marketo.com/t5/product-documents/upcoming-changes-to-design-studio-urls/ta-p/306632#_Toc54870361" target="_blank">の更新が必要な場合があります</a>、例： <code>http://na-sj01.marketo.com/rs/123-ABC-456/images/puppy.png</code>. 
   <p>Web 開発者と協力して、更新が必要になる場所を決定してください。</li></td>
  </tr>
 </tbody> 
</table>

## フォーム {#forms}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">エリア</th> 
   <th>レビューフォーカス</th>
  </tr> 
  <tr> 
   <td>グローバルフォーム</td> 
   <td><li>グローバルな数 <a href="/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md" target="_blank">フォーム</a> いるの？</li>
<li>ほとんどのプログラムでグローバルフォームとローカルフォームのどちらを使用しますか？</li>
<li>すべてのフォームがマーケティングおよびセールスに適したデータを収集していますか？</li>
<li>非表示の値は適切に利用されますか？</li>
<li>任意のMarketo Engageフォームが、非Marketo Engageのランディングページで使用されているか。 どのように参照されていますか？</li>
<p><img src="assets/tip-icon.png" alt="ヒントアイコン">ヒント：導入された新しい埋め込みコードを使用してMarketo Engageフォームを埋め込むページを更新します（セキュリティで保護されたランディングページが必要です）。
<br/><pre><script src="//example.marketo.com/js/forms2/js/forms2.min.js"></script></pre>
<br/><pre><form id="mktoForm_1"></form><script>MktoForms2.loadForm("//example.marketo.com", "123-ABC-456", 1);</script></pre>
</td>
  </tr>
  <tr> 
   <td>データの標準化</td> 
   <td><li>お使いの <a href="/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md" target="_blank">フォームフィールド</a> 主に候補リストを開くか、テキストフィールドを開くか。</li>
<p><img src="assets/tip-icon.png" alt="ヒントアイコン">ヒント：テキストフィールドが開いている場合は、データが乱雑にならないように、候補リストに切り替えることを検討してください。</td>
  </tr>
  <tr> 
   <td>プライバシーとコンプライアンス</td> 
   <td><li>フォーム戦略は、企業データのプライバシーやオプトインの要件に合っていますか？ 
   <br/>     検討 <a href="https://business.adobe.com/resources/ebooks/the-gdpr-and-the-marketer.html" target="_blank">一般データ保護規則 (GDPR)</a>，カナダのスパム対策法 (CASL)，規制コンプライアンスのための 2003 年の非迷惑ポルノおよびマーケティング法 (CAN-SPAM) の暴行の制御，カリフォルニア州消費者プライバシー法 (CCPA) など。</li>
<p><img src="assets/tip-icon.png" alt="ヒントアイコン">ヒント：これらの問題については、常に法務チームに相談してください。 変更を加える前に、コンプライアンスを維持するための以前の取り組みについてチームに問い合わせてください。</td>
  </tr>
 </tbody> 
</table>

## メール {#emails}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">エリア</th> 
   <th>レビューフォーカス</th>
  </tr> 
  <tr> 
   <td>グローバルメール</td> 
   <td><li>グローバルな数 <a href="/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md" target="_blank">電子メール</a> いるの？ プログラムで使われているのか？</li></td>
  </tr>
  <tr> 
   <td>テンプレート</td> 
   <td><li>数 <a href="/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md" target="_blank">電子メールテンプレート</a> いるの？ 彼らは活用されているのですか？</li></td>
  </tr>
  <tr> 
   <td>メールテスト</td> 
   <td><li>使用方法 <a href="/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/understanding-email-testing-options.md" target="_blank">メールテスト</a>? あなたの方法はまだ有効ですか？</li></td>
  </tr>
  </tr>
  <tr> 
   <td>プライバシーとコンプライアンス</td> 
   <td><li>すべてのメールに適切なフッターがありますか？ GDPR、CASL、CAN-SPAM、CCPA などを考慮します。 コンプライアンスに関する影響</li>
<p><img src="assets/tip-icon.png" alt="ヒントアイコン">ヒント：コンプライアンスに関する問題については、常に法務チームに相談してください。 変更を加える前に、コンプライアンスを維持するための以前の取り組みについてチームに問い合わせてください。</td>
  </tr>
 </tbody> 
</table>

## スニペット {#snippets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">エリア</th> 
   <th>レビューフォーカス</th>
  </tr> 
  <tr> 
   <td>スニペット</td> 
   <td><li>数 <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md" target="_blank">スニペット</a> いるの？ 使用されていますか？ 
   <br/>     そうでない場合は、 <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md" target="_blank">電子メール</a> および <a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/add-a-snippet-to-a-landing-page.md" target="_blank">ランディングページ</a> フッターコンテンツ、ロゴなど。</li></td>
  </tr>
 </tbody> 
</table>

## すべてのアセット {#all-assets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">エリア</th> 
   <th>レビューフォーカス</th>
  </tr> 
  <tr> 
   <td>アセットステータス</td> 
   <td><li>にあるアセットの数 <i>ドラフト</i> および <i>承認待ち下書きあり</i> ステータス ( 例： <a href="/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md" target="_blank">電子メール</a>, <a href="/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md#approve-a-landing-page" target="_blank">ランディングページ</a>, <a href="/help/marketo/product-docs/demand-generation/forms/creating-a-form/approve-a-form.md" target="_blank">フォーム</a>, <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/approve-a-snippet.md" target="_blank">スニペット</a>)?
   <br/>     多数の場合は、削除または承認することを検討してください。</li></td>
  </tr>
  <tr> 
   <td>アセットの共有</td> 
   <td><li>どのアセットが <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md#sharing-across-workspaces" target="_blank">ワークスペースで共有</a>?</li>
   <p><img src="assets/note-icon.png" alt="メモアイコン"> 注意：ある Workspace で実行されたアクションによって、別のユーザーの別の Workspace でアセットにアクセスできなくなる可能性があるので、これを把握することが重要です。</td>
  </tr>
 </tbody> 
</table>

<br> 

[◄継承されたインスタンスの監査：マーケティングアクティビティ](/help/marketo/getting-started/inheriting-a-marketo-instance/marketing-activities-checklist.md)

[継承されたインスタンスの監査：継承されたインスタンスの設定のドキュメント化►](/help/marketo/getting-started/inheriting-a-marketo-instance/document-your-setup.md)
