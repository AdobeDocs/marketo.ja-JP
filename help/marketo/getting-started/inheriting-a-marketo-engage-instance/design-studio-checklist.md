---
description: 継承インスタンスデザインスタジオのチェックリスト - Marketo ドキュメント - 製品ドキュメント
title: 継承インスタンスデザインスタジオのチェックリスト
feature: Getting Started
exl-id: 41e89120-4ac0-4e70-bed0-da4e5c5542ff
source-git-commit: 2c74c71c9311312f7e0991ed5598ccb09a9b1f15
workflow-type: ht
source-wordcount: '561'
ht-degree: 100%

---

# 継承インスタンス：デザインスタジオのチェックリスト {#inherited-instance-design-studio-checklist}

テンプレートを構造化し、グローバルフォーム、スニペット、画像およびファイルを作成すると、データエラーを最小限に抑えながら、プログラムの作成ワークフローを合理化できます。忘れずに[チェックリストをダウンロード](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx)し、進捗状況を追跡してください。

## ランディングページ {#landing-pages}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">エリア</th> 
   <th>レビューフォーカス</th>
  </tr> 
  <tr> 
   <td>グローバルランディングページ</td> 
   <td><li>グローバル<a href="/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/understanding-free-form-vs-guided-landing-pages.md" target="_blank">ランディングページ</a>はいくつありますか？プログラムで使われていますか？</li>
   <li><a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/subscription-center-learn.html?lang=ja" target="_blank">サブスクリプションセンター</a>を設定していますか？
   <br/>     設定していない場合は、新たに設定することを検討してください。</li></td>
  </tr>
  <tr> 
   <td>テンプレート</td> 
   <td><li><a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-templates/edit-a-marketo-landing-page-template.md" target="_blank">ランディングページテンプレート</a>はいくつありますか？活用されていますか？</li></td>
  </tr>
  <tr> 
   <td>テストグループ</td> 
   <td><li><a href="/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-test-groups.md" target="_blank">ランディングページのテストグループ</a>はいくつありますか？それらはすべて今でも関連性がありますか？</li></td>
  </tr>
   <tr> 
   <td>プライバシーとコンプライアンス</td> 
   <td><li>すべてのランディングページに適切なフッターがありますか？</li></td>
  </tr>
 </tbody> 
</table>

## 画像とファイル {#images-and-files}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">エリア</th> 
   <th>レビューフォーカス</th>
  </tr> 
  <tr> 
   <td>命名規則</td> 
   <td><li><a href="/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md" target="_blank">画像やファイル</a>には一貫性のある命名規則が使用されていますか？</li></td>
  </tr>
  <tr> 
   <td>フォルダー構造</td> 
   <td><li>画像やファイルは<a href="/help/marketo/product-docs/demand-generation/images-and-files/organize-your-images-and-files-using-folders.md" target="_blank">適切に整理され</a>ており、簡単に検索できますか？</li></td>
  </tr>
  <tr> 
   <td>画像とファイル</td> 
   <td><li><a href="/help/marketo/product-docs/demand-generation/images-and-files/find-the-url-of-an-uploaded-image-or-file.md" target="_blank">Web ページで参照されている</a>画像やファイルは更新が必要ですか？ 
   <p>例：<code>http://na-sj01.marketo.com/rs/123-ABC-456/images/puppy.png</code> など、ハードコードされた URL 構造の<a href="https://nation.marketo.com/t5/product-documents/upcoming-changes-to-design-studio-urls/ta-p/306632#_Toc54870361" target="_blank">更新が必要になる場合があります</a>。 
   <p>Web 開発者と協力して、更新が必要な場所を判断してください。</li></td>
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
   <td><li>グローバル<a href="/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md" target="_blank">フォーム</a>はいくつありますか？</li>
<li>ほとんどのプログラムでグローバルフォームとローカルフォームのどちらを使用しますか？</li>
<li>すべてのフォームがマーケティングおよびセールスに適したデータを収集していますか？</li>
<li>非表示の値は適切に活用されていますか？</li>
<li>任意の Marketo Engage フォームが Marketo Engage 以外のランディングページで使用されていますか？どのように参照されていますか？</li>
<p><img src="assets/tip-icon.png" alt="ヒントアイコン">ヒント：導入された新しい埋め込みコードを使用して、Marketo Engage フォームを埋め込むページを更新します（セキュリティで保護されたランディングページが必要です）。
<p><a href="/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/design-studio-checklist-2.png" target="_blank"><img src="assets/design-studio-checklist-1.png" alt="コードサムネール"></a>
</td>
  </tr>
  <tr> 
   <td>データの標準化</td> 
   <td><li>使用している<a href="/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md" target="_blank">フォームフィールド</a>は主に選択リストですか、それともオープンテキストフィールドですか？</li>
<p><img src="assets/tip-icon.png" alt="ヒントアイコン">ヒント：オープンテキストフィールドの場合は、データが乱雑にならないように、選択リストに切り替えることを検討してください。</td>
  </tr>
  <tr> 
   <td>プライバシーとコンプライアンス</td> 
   <td><li>現在のフォーム戦略は、企業のデータプライバシーおよびオプトインの要件を満たしていますか？
   <br/>     <a href="https://business.adobe.com/resources/ebooks/the-gdpr-and-the-marketer.html" target="_blank">EU 一般データ保護規則（GDPR）</a>、カナダのスパム対策法（CASL）、2003 年の迷惑ポルノグラフィーおよびマーケティングの攻撃に対する規制法（CAN-SPAM）、カリフォルニア州消費者プライバシー法（CCPA）などの規制への準拠を考慮してください。</li>
<p><img src="assets/tip-icon.png" alt="ヒントアイコン">ヒント：これらの問題については、必ず法務部門に相談してください。変更を行う前に、コンプライアンスを維持するためのこれまでの取り組みについてチームに確認してください。</td>
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
   <td><li>グローバル<a href="/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md" target="_blank">メール</a>は何件ありますか？プログラムで使われていますか？</li></td>
  </tr>
  <tr> 
   <td>テンプレート</td> 
   <td><li><a href="/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md" target="_blank">メールテンプレート</a>はいくつありますか？活用されていますか？</li></td>
  </tr>
  <tr> 
   <td>メールテスト</td> 
   <td><li><a href="/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/understanding-email-testing-options.md" target="_blank">メールテスト</a>をどのように使用していますか？その使用方法はまだ効果的ですか？</li></td>
  </tr>
  </tr>
  <tr> 
   <td>プライバシーとコンプライアンス</td> 
   <td><li>すべてのメールに適切なフッターがありますか？コンプライアンスへの影響については、GDPR、CASL、CAN-SPAM、CCPA などを検討してください。</li>
<p><img src="assets/tip-icon.png" alt="ヒントアイコン">ヒント：コンプライアンスに関する問題については、常に法務チームに相談してください。変更を行う前に、コンプライアンスを維持するためのこれまでの取り組みについてチームに確認してください。</td>
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
   <td><li><a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md" target="_blank">スニペット</a>はいくつありますか？現在使用していますか？
   <br/>     使用していない場合は、<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md" target="_blank">メール</a>や<a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/add-a-snippet-to-a-landing-page.md" target="_blank">ランディングページ</a>のフッターコンテンツ、ロゴなどに使用することを検討してください。</li></td>
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
   <td>アセットのステータス</td> 
   <td><li><i>ドラフト</i>ステータスと<i>ドラフトで承認済み</i>ステータスのアセット（<a href="/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md" target="_blank">メール</a>、<a href="/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md#approve-a-landing-page" target="_blank">ランディングページ</a>、<a href="/help/marketo/product-docs/demand-generation/forms/creating-a-form/approve-a-form.md" target="_blank">フォーム</a>、<a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/approve-a-snippet.md" target="_blank">スニペット</a>など）はいくつありますか？
   <br/>     多数ある場合は、削除または承認を検討してください。</li></td>
  </tr>
  <tr> 
   <td>アセットの共有</td> 
   <td><li>どのアセットが<a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md#sharing-across-workspaces" target="_blank">ワークスペース全体で共有</a>されていますか？</li>
   <p><img src="assets/note-icon.png" alt="メモアイコン"> メモ：あるワークスペースで実行されたアクションによって、別のユーザーが別のワークスペースでアセットにアクセスできなくなる可能性があることを理解しておいてください。</td>
  </tr>
 </tbody> 
</table>
