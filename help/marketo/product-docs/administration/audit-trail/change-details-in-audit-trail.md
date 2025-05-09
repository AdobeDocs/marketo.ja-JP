---
unique-page-id: 11379928
description: 監査記録の変更の詳細 — Marketo ドキュメント — 製品ドキュメント
title: 監査記録の詳細の変更
exl-id: 5583be62-46a6-42f9-b4b3-0df63a171b2d
feature: Audit Trail
source-git-commit: 1477b889f74597396b3467371229a511e4390f91
workflow-type: ht
source-wordcount: '1902'
ht-degree: 100%

---

# 監査記録の詳細の変更 {#change-details-in-audit-trail}

監査記録は、Marketo サブスクリプションで誰が何をおこなっているかに関する多くのインサイトを提供します。詳細は以下の通りです。

## アセット監査記録 {#asset-audit-trail}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th colspan="1">アセット／タイプ</th> 
   <th colspan="1">アクション</th> 
   <th colspan="1">変更の詳細</th> 
  </tr> 
  <tr> 
   <td rowspan="15"><strong>デフォルトのプログラム</strong><br><br><br><br><br><br><br><br><br><br><br></td> 
   <td>作成</td> 
   <td>チャネルタイプ「チャネルタイプ」<br>または<br>「プログラム名」から複製</td> 
  </tr> 
  <tr> 
   <td>名前変更</td> 
   <td>新しい名前「新しい名前」、古い名前「古い名前」</td> 
  </tr> 
  <tr> 
   <td>複製</td> 
   <td>ワークスペース「ワークスペース名」に複製<br>場所「キャンペーンフォルダー」または「エンゲージメントプログラム」<br>複製されたプログラム名「新しい名前」</td> 
  </tr> 
  <tr> 
   <td>削除</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>チャネルの編集</td> 
   <td>新しいチャネル「新しいチャネル名」、古いチャネル「古いチャネル名」 </td> 
  </tr> 
  <tr> 
   <td>プログラムトークンの修正</td> 
   <td>トークン「トークン名」、値「トークン値」を追加</td> 
  </tr> 
  <tr> 
   <td>プログラムトークンの修正</td> 
   <td>トークン「トークン名」を編集：新しい値「新しい値」、古い値「古い値」</td> 
  </tr> 
  <tr> 
   <td>プログラムトークンの修正</td> 
   <td>トークン「トークン名」を削除</td> 
  </tr> 
  <tr> 
   <td>プログラム設定の修正</td> 
   <td>分析動作「動作名」を追加</td> 
  </tr> 
  <tr> 
   <td>プログラム設定の修正</td> 
   <td><p>分析動作「動作名」を編集</p><p>古い動作「動作名」</p></td> 
  </tr> 
  <tr> 
   <td>プログラム設定の修正</td> 
   <td>分析動作「動作名」を削除</td> 
  </tr> 
  <tr> 
   <td colspan="1">プログラム設定の修正</td> 
   <td colspan="1">期間原価を追加：値「#」、プログラム対象月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">プログラム設定の修正</td> 
   <td colspan="1">期間原価を編集：新しいコスト値「#」、新しいプログラム対象月「yyyy-mm」、古いコスト値「#」、古いプログラム対象月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">プログラム設定の修正</td> 
   <td colspan="1">期間原価を削除。値「#」プログラム対象月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td>エクスポート</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td rowspan="19"><strong>メール</strong><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br></td> 
   <td>作成</td> 
   <td>テンプレート「テンプレート名」を使用して作成<br>または<br>「アセット名」から複製</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>「差出人名」を「新しい差出人名」に更新</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>「メールから」を「newemail@name.com」に更新</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>「返信先」を「newreplytoemail@name.com」に更新</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>「件名」を「新しい件名行」に更新</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>セグメント化「segmentation_name」を追加</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>セグメント化を削除</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>スニペット「snippet_name」を追加</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>スニペットを削除</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>編集によってテンプレート「template_name」かメールが壊れた（注意：これは、コードを直接編集した場合に発生します）。</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>新しい説明「新しい説明」、古い説明「古い説明」</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>モジュール <code>"&lt;module name&gt;" &lt;attribute&gt;</code> を「値」に編集</td> 
  </tr> 
  <tr> 
   <td>削除</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>名前変更</td> 
   <td>新しい名前「新しい名前」、古い名前「古い名前」</td> 
  </tr> 
  <tr> 
   <td>複製</td> 
   <td>「デザインスタジオ」のフォルダー「フォルダー名」に複製<br>アセット名「名前」を複製<br>または<br>「マーケティングアクティビティ」のプログラム「プログラム名」に複製<br>アセット名「名前」を複製</td> 
  </tr> 
  <tr> 
   <td>移動</td> 
   <td>「デザインスタジオ」のフォルダー「フォルダ名ー」に移動<br>または<br>「マーケティングアクティビティ」のプログラム「プログラム名」に移動</td> 
  </tr> 
  <tr> 
   <td>承認</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>承認取消</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>下書き</td> 
   <td>スニペット「スニペット名」が承認されたので、メールを下書き<br>または<br>テンプレート「テンプレート名」が承認されたので、メールを下書き</td> 
  </tr> 
   <td rowspan="17">メールプログラム</td> 
   <td>作成</td> 
   <td>チャネルタイプ「チャネルタイプ」<br>または<br>「プログラム名」から複製</td> 
  </tr> 
  <tr> 
   <td colspan="1">名前変更</td> 
   <td colspan="1">新しい名前「新しい名前」、古い名前「古い名前」</td> 
  </tr> 
  <tr> 
   <td>複製</td> 
   <td>ワークスペース「ワークスペース名」に複製<br>場所「キャンペーンフォルダーまたはエンゲージメントプログラム」<br>プログラム名「新しい名前」を複製</td> 
  </tr> 
  <tr> 
   <td>削除</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>中止</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>チャネルの編集</td> 
   <td>新しいチャネル「新しいチャネル」、古いチャネル「古いチャネル」</td> 
  </tr> 
  <tr> 
   <td>プログラムトークンの修正</td> 
   <td>トークン「トークン名」、値「トークン値」を追加</td> 
  </tr> 
  <tr> 
   <td>プログラムトークンの修正</td> 
   <td>トークン「トークン名」を編集：新しい値「新しい値」、古い値「古い値」</td> 
  </tr> 
  <tr> 
   <td>プログラムトークンの修正</td> 
   <td>トークン「トークン名」を削除</td> 
  </tr> 
  <tr> 
   <td>プログラムスケジュールの修正</td> 
   <td>「開始日、開始時刻」に開始して「終了日、終了時刻」に終了するようにスケジュールを設定</td> 
  </tr> 
  <tr> 
   <td>プログラムスケジュールの修正</td> 
   <td>スケジュールを「新しい日付、新しい時刻」に変更</td> 
  </tr> 
  <tr> 
   <td>プログラム設定の修正</td> 
   <td>分析動作「動作名」を追加</td> 
  </tr> 
  <tr> 
   <td>プログラム設定の修正</td> 
   <td>分析動作「動作名」を編集<br>古い動作「動作名」</td> 
  </tr> 
  <tr> 
   <td>プログラム設定の修正</td> 
   <td>分析動作「動作名」を削除</td> 
  </tr> 
  <tr> 
   <td colspan="1">プログラム設定の修正</td> 
   <td colspan="1">期間原価を追加：値「#」、プログラム対象月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">プログラム設定の修正</td> 
   <td colspan="1">期間原価を編集：新しいコスト値「#」、新しいプログラム対象月「yyyy-mm」、古いコスト値「#」、古いプログラム対象月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">プログラム設定の修正</td> 
   <td colspan="1">期間原価を削除。値「#」プログラム対象月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td rowspan="8">メールテンプレート</td> 
   <td>作成</td> 
   <td>空白または「テンプレート名」から複製</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>新しい説明「新しい説明」、古い説明「古い説明」</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>HTML 編集済み</td> 
  </tr> 
  <tr> 
   <td>削除</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>名前変更</td> 
   <td>新しい名前「新しい名前」、古い名前「古い名前」</td> 
  </tr> 
  <tr> 
   <td>複製</td> 
   <td>「フォルダー名」に複製<br>アセット名「名前」を複製</td> 
  </tr> 
  <tr> 
   <td>承認</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>承認取消</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td rowspan="23">エンゲージメントプログラム</td> 
   <td>作成</td> 
   <td>チャネルタイプ「チャネルタイプ」<br>または<br>「プログラム名」から複製</td> 
  </tr> 
  <tr> 
   <td>名前変更</td> 
   <td>新しい名前「新しい名前」、古い名前「古い名前」</td> 
  </tr> 
  <tr> 
   <td>複製</td> 
   <td>ワークスペース「ワークスペース名」に複製<br>場所「キャンペーンフォルダーまたはエンゲージメントプログラム」<br>プログラム名「新しい名前」を複製</td> 
  </tr> 
  <tr> 
   <td>削除</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>チャネルの編集</td> 
   <td>新しいチャネル「新しいチャネル」、古いチャネル「古いチャネル」</td> 
  </tr> 
  <tr> 
   <td>プログラムストリームの修正</td> 
   <td><p>ストリームを追加</p><p>名前「名前」、配置「#」</p></td> 
  </tr> 
  <tr> 
   <td>プログラムストリームの修正</td> 
   <td><p>ストリームを編集</p><p>新しいストリーム名「新しい名前」、古いストリーム名「古い名前」</p><p>新しい配置「新しい#」、古い配置「古い#」</p></td> 
  </tr> 
  <tr> 
   <td>プログラムストリームの修正</td> 
   <td>ストリーム名「名前」を削除</td> 
  </tr> 
  <tr> 
   <td>プログラムストリームの修正</td> 
   <td>コンテンツを追加<br>ストリーム名「ストリーム名」<br>タイプ「メール」または「プログラム」<br>名前「メール名」または「プログラム名」<br>スマートキャンペーン「スマートキャンペーン名」</td> 
  </tr> 
  <tr> 
   <td>プログラムストリームの修正</td> 
   <td>コンテンツを有効化<br>ストリーム名「ストリーム名」<br>コンテンツ名「メール名」または「プログラム名」</td> 
  </tr> 
  <tr> 
   <td>プログラムストリームの修正</td> 
   <td>コンテンツを非アクティブ化<br>ストリーム名「ストリーム名」<br>コンテンツ名「メール名」または「プログラム名」</td> 
  </tr> 
  <tr> 
   <td>プログラムストリームの修正</td> 
   <td>コンテンツを削除<br>ストリーム名「ストリーム名」<br>コンテンツ名「メール名」または「プログラム名」</td> 
  </tr> 
  <tr> 
   <td>プログラムトークンの修正</td> 
   <td>トークン「トークン名」、値「トークン値」を追加</td> 
  </tr> 
  <tr> 
   <td>プログラムトークンの修正</td> 
   <td>トークン「トークン名」を編集：新しい値「新しい値」、古い値「古い値」</td> 
  </tr> 
  <tr> 
   <td>プログラムトークンの修正</td> 
   <td>トークン「トークン名」を削除</td> 
  </tr> 
  <tr> 
   <td>プログラム設定の修正</td> 
   <td>分析動作「動作名」を追加</td> 
  </tr> 
  <tr> 
   <td>プログラム設定の修正</td> 
   <td>分析動作「動作名」を編集<br>古い動作「動作名」</td> 
  </tr> 
  <tr> 
   <td>プログラム設定の修正</td> 
   <td>分析動作「動作名」を削除</td> 
  </tr> 
  <tr> 
   <td>プログラム設定の修正</td> 
   <td>プログラムをステータスを変更：新しい値「オン／オフ」、古い値「オフ／オン」</td> 
  </tr> 
  <tr> 
   <td colspan="1">プログラム設定の修正</td> 
   <td colspan="1">期間原価を追加：値「#」、プログラム対象月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">プログラム設定の修正</td> 
   <td colspan="1">期間原価を編集：新しいコスト値「#」、新しいプログラム対象月「yyyy-mm」、古いコスト値「#」、古いプログラム対象月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">プログラム設定の修正</td> 
   <td colspan="1">期間原価を削除。値「#」プログラム対象月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td>エクスポート</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td rowspan="18">イベントプログラム</td> 
   <td>作成</td> 
   <td>チャネルタイプ「チャネルタイプ」<br>または<br>「プログラム名」から複製</td> 
  </tr> 
  <tr> 
   <td>名前変更</td> 
   <td>新しい名前「新しい名前」、古い名前「古い名前」</td> 
  </tr> 
  <tr> 
   <td>削除</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>複製</td> 
   <td>ワークスペース「ワークスペース名」に複製<br>場所「キャンペーンフォルダー」または「エンゲージメントプログラム」<br>複製されたプログラム名「新しい名前」</td> 
  </tr> 
  <tr> 
   <td>チャネルの編集</td> 
   <td>新しいチャネル「新しいチャネル」、古いチャネル「古いチャネル」 </td> 
  </tr> 
  <tr> 
   <td>プログラムトークンの修正</td> 
   <td>トークン「トークン名」、値「トークン値」を追加</td> 
  </tr> 
  <tr> 
   <td>プログラムトークンの修正</td> 
   <td>トークン「トークン名」を編集：新しい値「新しい値」、古い値「古い値」</td> 
  </tr> 
  <tr> 
   <td>プログラムトークンの修正</td> 
   <td>トークン「トークン名」を削除</td> 
  </tr> 
  <tr> 
   <td>プログラムスケジュールの修正</td> 
   <td>「開始日、開始時刻」に開始して「終了日、終了時刻」に終了するようにスケジュールを設定</td> 
  </tr> 
  <tr> 
   <td>プログラムスケジュールの修正</td> 
   <td>スケジュールを「新しい日付、新しい時刻」に変更</td> 
  </tr> 
  <tr> 
   <td>プログラム設定の修正</td> 
   <td>分析動作「動作名」を追加</td> 
  </tr> 
  <tr> 
   <td>プログラム設定の修正</td> 
   <td>分析動作「動作名」を編集<br>古い動作「動作名」</td> 
  </tr> 
  <tr> 
   <td>プログラム設定の修正</td> 
   <td>分析動作「動作名」を削除</td> 
  </tr> 
  <tr> 
   <td colspan="1">プログラム設定の修正</td> 
   <td colspan="1">期間原価を追加：値「#」、プログラム対象月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">プログラム設定の修正</td> 
   <td colspan="1">期間原価を編集：新しいコスト値「#」、新しいプログラム対象月「yyyy-mm」、古いコスト値「#」、古いプログラム対象月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">プログラム設定の修正</td> 
   <td colspan="1">期間原価を削除。値「#」プログラム対象月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">プログラム設定の修正</td> 
   <td colspan="1">イベントパートナー「パートナー名」を追加</td> 
  </tr> 
  <tr> 
   <td>エクスポート</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td rowspan="5">フォルダー</td> 
   <td>作成</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>削除</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>トークン「token_name」、値「値」を追加</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>トークン「token_name」を編集：新しい値「token_value」、古い値「old_token_value」</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>トークン「token_name」を削除</td> 
  </tr> 
  <tr> 
   <td rowspan="8">フォーム</td> 
   <td>作成</td> 
   <td>近日開始。詳細を表示または「フォーム名」から複製</td> 
  </tr> 
  <tr> 
   <td>削除</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>名前変更</td> 
   <td>新しい名前「新しい名前」、古い名前「古い名前」</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>新しい説明「新しい説明」、古い説明「古い説明」</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>フォーム設定を編集済み </td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>フィールド詳細を編集済み</td> 
  </tr> 
  <tr> 
   <td>複製</td> 
   <td>「デザインスタジオ」のフォルダー「フォルダー名」に複製<br>アセット名「名前」を複製<br>または<br>「マーケティングアクティビティ」のプログラム「プログラム名」に複製<br>アセット名「名前」を複製</td> 
  </tr> 
  <tr> 
   <td>移動</td> 
   <td>「デザインスタジオ」のフォルダー「フォルダ名ー」に移動<br>または<br>「マーケティングアクティビティ」のプログラム「プログラム名」に移動</td> 
  </tr> 
  <tr> 
   <td>フォーム</td> 
   <td>承認</td> 
   <td># アセットで使用 </td> 
  </tr> 
  <tr> 
   <td rowspan="9">ランディングページ</td> 
   <td>作成</td> 
   <td>テンプレート「テンプレート名」を使用して作成<br>または<br>「アセット名」から複製</td> 
  </tr> 
  <tr> 
   <td>削除</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>名前変更</td> 
   <td>新しい名前「新しい名前」、古い名前「古い名前」</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>新しい説明「新しい説明」、古い説明「古い説明」</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>「画像」を追加、「画像」を削除、画像コンポーネントを編集</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>「リッチテキスト」を追加、「リッチテキスト」を削除、リッチテキストコンポーネントを編集</td> 
  </tr> 
  <tr> 
   <td>複製</td> 
   <td>「デザインスタジオ」のフォルダー「フォルダー名」に複製<br>アセット名「名前」を複製<br>アセット URL 「www.url.com」を複製<br>または<br>「マーケティングアクティビティ」のプログラム「プログラム名」に複製<br>アセット名「名前」を複製<br>アセット URL 「www.url.com」を複製</td> 
  </tr> 
  <tr> 
   <td>移動</td> 
   <td>「デザインスタジオ」のフォルダー「フォルダー名」に移動<br>または<br>「マーケティングアクティビティ」のプログラム「プログラム名」に移動</td> 
  </tr> 
  <tr> 
   <td>承認</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>下書き</td> 
   <td>テンプレート「テンプレート名」が承認されたため、ランディングページを下書き</td> 
  </tr> 
  <tr> 
   <td>承認取消</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td rowspan="8">ランディングページテンプレート</td> 
   <td>作成</td> 
   <td><p>空白<br>または<br>「アセット名」から複製</p></td> 
  </tr> 
  <tr> 
   <td>削除</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>名前変更</td> 
   <td>新しい名前「新しい名前」、古い名前「古い名前」</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>新しい説明「新しい説明」、古い説明「古い説明」</td> 
  </tr> 
  <tr> 
   <td>複製</td> 
   <td>「フォルダー名」に複製<br>アセット名「名前」を複製</td> 
  </tr> 
  <tr> 
   <td>エクスポート</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>承認</td> 
   <td># アセットで使用 </td> 
  </tr> 
  <tr> 
   <td>承認取消</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td rowspan="5">リスト（静的）</td> 
   <td>作成</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>エクスポート</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>複製</td> 
   <td>「ユーザーデータベース」のフォルダー「フォルダー名」に複製<br>アセット名「名前」を複製<br>または<br>「マーケティングアクティビティ」のプログラム「プログラム名」に複製<br>アセット名「名前」を複製</td> 
  </tr> 
  <tr> 
   <td>削除</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>名前変更</td> 
   <td>新しい名前「新しい名前」、古い名前「古い名前」</td> 
  </tr> 
  <tr> 
   <td rowspan="12">スマートキャンペーン</td> 
   <td>作成</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>有効化</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>無効化</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>中止</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>移動</td> 
   <td>「プログラム」の「プログラム名」に移動<br>または<br>「フォルダー」の「フォルダー名」に移動</td> 
  </tr> 
  <tr> 
   <td>名前変更</td> 
   <td>新しい名前「新しい名前」、古い名前「古い名前」</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>新しい説明「新しい説明」、古い説明「古い説明」</td> 
  </tr> 
  <tr> 
   <td>削除</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>複製</td> 
   <td>「プログラム」のプログラム「プログラム名」に複製<br>アセット名「名前」を複製<br>または<br>「フォルダー」のフォルダー「フォルダー名」に複製<br>アセット名「名前」を複製</td> 
  </tr> 
  <tr> 
   <td>スマートリスト設定の修正</td> 
   <td>フィルターとトリガーの名前と値を含む、現在の状態のスナップショットを表示</td> 
  </tr> 
  <tr> 
   <td>キャンペーンスケジュールの修正</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>フローステップアクションの変更</td> 
   <td>各フローステップの名前と値を含む、現在の状態のスナップショットを表示</td> 
  </tr> 
  <tr> 
   <td rowspan="7">スマートリスト</td> 
   <td>作成</td> 
   <td>「スマートリスト名」から複製</td> 
  </tr> 
  <tr> 
   <td>エクスポート</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>名前変更</td> 
   <td>新しい名前「新しい名前」、古い名前「古い名前」</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>新しい説明「新しい説明」、古い説明「古い説明」</td> 
  </tr> 
  <tr> 
   <td>削除</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>複製</td> 
   <td>「担当者データベース」のフォルダー「フォルダー名」に複製<br>アセット名「名前」を複製<br>または<br>「マーケティングアクティビティ」のプログラム「プログラム名」に複製<br>アセット名「名前」を複製</td> 
  </tr> 
  <tr> 
   <td>スマートリスト設定の修正</td> 
   <td>フィルターとトリガーの名前と値を含む、現在の状態のスナップショットを表示 </td> 
  </tr> 
  <tr> 
   <td rowspan="11">スニペット</td> 
   <td>作成</td> 
   <td><p>空白<br>または<br>「スニペット名」から複製</p></td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>セグメント化「segmentation_name」を追加</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>セグメント化を削除</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>編集済み</td> 
  </tr> 
  <tr> 
   <td>削除</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>名前変更</td> 
   <td>新しい名前「新しい名前」、古い名前「古い名前」</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>新しい説明「新しい説明」、古い説明「古い説明」</td> 
  </tr> 
  <tr> 
   <td>複製</td> 
   <td>「フォルダー名」に複製<br>スニペット名「スニペット名」を複製</td> 
  </tr> 
  <tr> 
   <td>承認</td> 
   <td># アセットで使用</td> 
  </tr> 
  <tr> 
   <td>下書きなしで承認</td> 
   <td>なし</td> 
  </tr> 
  <tr> 
   <td>承認取消</td> 
   <td><p>なし</p></td> 
  </tr> 
 </tbody> 
</table>

## 管理監査記録 {#admin-audit-trail}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>管理エリア</th> 
   <th>アクション</th> 
   <th>変更の詳細</th> 
  </tr> 
  <tr> 
   <td>IP 制限</td> 
   <td>編集</td> 
   <td>IP 制限の編集：許可／ブロック「ブロック」、IP アドレス「#」、IP 制限無効化「」</td> 
  </tr> 
  <tr> 
   <td rowspan="2">パーティション</td> 
   <td>作成</td> 
   <td>名前「パーティション名」のパーティションを作成</td> 
  </tr> 
  <tr> 
   <td>削除</td> 
   <td>「パーティション名」パーティションを削除</td> 
  </tr> 
  <tr> 
   <td>パスワード強度</td> 
   <td>編集</td> 
   <td>パスワードのセキュリティがテンプレートに変更：標準セキュリティ、min length：「#」、lower-upper：「#」、number：「#」、mixed case：「#」、expiration：「#」、session timeout：「#」</td> 
  </tr> 
  <tr> 
   <td rowspan="3">役割<br><br></td> 
   <td>作成</td> 
   <td>役割「役割名」を作成（注意：追加された権限に関する詳細が必要な場合は、サポートにお問い合わせください）- <br>役割に割り当てられた権限のスナップショットを表示</td> 
  </tr> 
  <tr> 
   <td>削除</td> 
   <td>役割「役割名」を削除</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>役割を「以前の名前」から「新しい名前」に編集（注意：権限の編集について詳しくは、サポートにお問い合わせください）- <br>役割に割り当てられた権限のスナップショットを表示<br></td> 
  </tr> 
  <tr> 
   <td>スマートリストレポート</td> 
   <td>編集</td> 
   <td>スマートリストをダウンロード用に編集</td> 
  </tr> 
  <tr> 
   <td rowspan="7">ユーザー<br><br><br><br></td> 
   <td>作成（招待）</td> 
   <td>次でユーザーを招待：メール「メールアドレス」、名前「氏名」、アクセス有効期限「空白または日付」、API ユーザー「True または False」 - <br>ユーザーに割り当てられた役割とワークスペースのスナップショットを表示</td> 
  </tr> 
  <tr> 
   <td colspan="1">削除</td> 
   <td colspan="1">ユーザー「ユーザー名」を削除</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>ユーザー名を「古い名前」から「新しい名前」に変更：メール「メール」、apiUser「true または false」、アクセス有効期限「空白または日付」</td> 
  </tr> 
  <tr> 
   <td>編集</td> 
   <td>メール「メール」、apiUser「true または false」、アクセス有効期限「空白または日付」のユーザーを編集</td> 
  </tr> 
  <tr> 
   <td colspan="1">編集</td> 
   <td colspan="1">ユーザーに割り当てられた役割やワークスペースを含む、現在の状態のスナップショットを表示</td> 
  </tr> 
  <tr> 
   <td>問題</td> 
   <td>カレンダーライセンスをメール「ユーザーのメール」、名前「ユーザー名」に発行</td> 
  </tr> 
  <tr> 
   <td>リセット</td> 
   <td>名前「名前」、メール「メール」のパスワードをリセット</td> 
  </tr> 
  <tr> 
   <td rowspan="2">ワークスペース</td> 
   <td>作成</td> 
   <td>「ワークスペース名」ワークスペースを作成</td> 
  </tr> 
  <tr> 
   <td>削除</td> 
   <td>「ワークスペース名」ワークスペースを削除</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[監査記録でのフィルタリング](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)
