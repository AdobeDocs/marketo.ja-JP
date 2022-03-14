---
description: セールスアクティビティ用語集 - Marketo ドキュメント - 製品ドキュメント
title: セールスアクティビティ用語集
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
source-git-commit: d261da2a2784ab322ef78fe22ef3d6b4321fc806
workflow-type: ht
source-wordcount: '520'
ht-degree: 100%

---

# セールスアクティビティ用語集 {#sales-activity-glossary}

Sales Connect で、販売者がセールスケイデンスにリードを追加したり、メールを送信したり、通話をアクティビティに送信したりすると、Marketo のアクティビティ履歴に記録されます。さらに、リードがメールに関与した場合、開封数、クリック数、返信数もログに記録されます。

以下のアクティビティは、Sales Connect から Marketo に記録されます。

>[!NOTE]
>
>これらのアクティビティと属性は、アドビの REST および Bulk API から使用できます。

## アクティビティ {#activities}

<table>
 <tr>
  <th>セールスアクティビティ</th>
  <th>属性</th>
 </tr>
 <tr>
  <th rowspan="9">セールスメール送信</th>
  <td>送信者</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>テンプレート ID</td>
 </tr>
 <tr>
  <td>セールステンプレート URL</td>
 </tr>
 <tr>
  <td>セールスキャンペーン URL</td>
 </tr>
 <tr>
  <td>セールステンプレート名</td>
 </tr>
 <tr>
  <td>メールの件名</td>
 </tr>
 <tr>
  <td>セールスキャンペーン名</td>
 </tr>
 <tr>
  <td>Marketo「セールス担当者」ID</td>
 </tr>
 <tr>
  <th rowspan="9">セールスメール開封</th>
  <td>送信者</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>テンプレート ID</td>
 </tr>
 <tr>
  <td>セールステンプレート URL</td>
 </tr>
 <tr>
  <td>セールスキャンペーン URL</td>
 </tr>
 <tr>
  <td>セールステンプレート名</td>
 </tr>
 <tr>
  <td>メールの件名</td>
 </tr>
 <tr>
  <td>セールスキャンペーン名</td>
 </tr>
 <tr>
  <td>Marketo「セールス担当者」ID</td>
 </tr>
 <tr>
  <th rowspan="10">セールスメールをクリック済み</th>
  <td>リンク</td>
 </tr>
 <tr>
  <td>送信者</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>テンプレート ID</td>
 </tr>
 <tr>
  <td>セールステンプレート URL</td>
 </tr>
 <tr>
  <td>セールスキャンペーン URL</td>
 </tr>
 <tr>
  <td>セールステンプレート名</td>
 </tr>
 <tr>
  <td>メールの件名</td>
 </tr>
 <tr>
  <td>セールスキャンペーン名</td>
 </tr>
 <tr>
  <td>Marketo「セールス担当者」ID</td>
 </tr>
<tr>
  <th rowspan="3">セールスメールに返信済み</th>
  <td>受信者</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>Marketo「セールス担当者」ID</td>
 </tr>
 <tr>
  <th rowspan="11">セールス電話を受信</th>
  <td>セールス電話発信者</td>
 </tr>
 <tr>
  <td>セールス電話のステータス</td>
 </tr>
 <tr>
  <td>セールス電話の件名</td>
 </tr>
 <tr>
  <td>セールスキャンペーン名</td>
 </tr>
 <tr>
  <td>セールスキャンペーン URL</td>
 </tr>
 <tr>
  <td>セールス電話の発信先電話番号</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>セールス電話の長さ</td>
 </tr>
 <tr>
  <td>セールス電話録音 URL</td>
 </tr>
  <tr>
  <td>セールス電話対応者</td>
 </tr>
 <tr>
  <td>Marketo「セールス担当者」ID</td>
 </tr>
 <tr>
  <th rowspan="6">セールスキャンペーンに追加</th>
  <td>セールスキャンペーン名</td>
 </tr>
 <tr>
  <td>セールス電話のステータス</td>
 </tr>
 <tr>
  <td>セールスキャンペーン URL</td>
 </tr>
 <tr>
  <td>送信者</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>セールスキャンペーン ID</td>
 </tr>
 <tr>
  <th rowspan="6">セールスキャンペーンから削除</th>
  <td>セールスキャンペーン名</td>
 </tr>
 <tr>
  <td>セールス電話のステータス</td>
 </tr>
 <tr>
  <td>セールスキャンペーン URL</td>
 </tr>
 <tr>
  <td>送信者</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>セールスキャンペーン ID</td>
 </tr>
</table>

## 説明 {#descriptions}

<table> 
 <tr>
  <th>属性</th>
  <th>説明</th>
 </tr>
 <tbody> 
 <tr> 
   <td><strong>詳細</strong></td> 
   <td>バウンスエラーメッセージの詳細。</td> 
  </tr> 
  <tr> 
   <td><strong>メール</strong></td> 
   <td>バウンスしたメールアドレス。</td> 
  </tr> 
  <tr> 
   <td><strong>リンク</strong></td> 
   <td>クリックされた URL。</td> 
  </tr> 
  <tr> 
   <td><strong>Marketo「セールス担当者」ID</strong></td> 
   <td>Sales Connect の人物レコードの一意の ID。</td> 
  </tr> 
  <tr> 
   <td><strong>受信者</strong></td> 
   <td>メール送信者のメールアドレス。</td> 
  </tr>
  <tr> 
   <td><strong>セールス電話対応者</strong></td> 
   <td>電話に出た人の名前。</td> 
  </tr>
  <tr> 
   <td><strong>セールス電話の長さ</strong></td> 
   <td>電話の長さ（秒）。</td> 
  </tr>
  <tr> 
   <td><strong>セールス電話発信者</strong></td> 
   <td>電話をかけた人のメールアドレス。</td> 
  </tr>
  <tr> 
   <td><strong>セールス電話録音 URL</strong></td> 
   <td>通話記録の URL。</td> 
  </tr>
  <tr> 
   <td><strong>セールス電話のステータス</strong></td> 
   <td>電話の最終的な電話ステータスを保存します。このステータスには、完了、応答なし、キャンセル、失敗が含まれます。</td> 
  </tr>
  <tr> 
   <td><strong>セールス電話の件名</strong></td> 
   <td>ダイヤラー内でセールスユーザーによって選択された電話の結果。</td> 
  </tr>
  <tr> 
   <td><strong>セールスキャンペーン ID</strong></td> 
   <td>Sales Campaign のセールスキャンペーンアセットの一意の ID。</td> 
  </tr>
  <tr> 
   <td><strong>セールスキャンペーン名</strong></td> 
   <td>セールスキャンペーンの名前。</td> 
  </tr>
  <tr> 
   <td><strong>セールスキャンペーン URL</strong></td> 
   <td>セールスキャンペーンの Sales Campaign URL。</td> 
  </tr>
  <tr> 
   <td><strong>セールスメールの件名</strong></td> 
   <td>メールの件名行と一意の ID（例：件名（MSC-12345678）</td> 
  </tr>
  <tr> 
   <td><strong>セールス電話の発信先電話番号</strong></td> 
   <td>セールスが発信した電話番号。</td> 
  </tr>
  <tr> 
   <td><strong>セールステンプレート名</strong></td> 
   <td>Sales Connect のメールテンプレートの名前。</td> 
  </tr>
  <tr> 
   <td><strong>セールステンプレート URL</strong></td> 
   <td>メールテンプレートの Sales Connect. URL。</td> 
  </tr>
  <tr> 
   <td><strong>送信者</strong></td>
   <td>メール送信者のメールアドレス。</td> 
  </tr> 
  <tr> 
   <td><strong>ソース</strong></td> 
   <td>アクティビティのソース。2021 年 10 月のリリースより前では Sales Connect アクティビティは「Tout」に設定されます。2021 年 10 月のリリースより後では Sales Connect アクティビティは「Sales App」に設定されます。</td>
  </tr> 
  <tr> 
   <td><strong>テンプレート ID</strong></td> 
   <td>ソースが Tout の場合、テンプレート ID は Marketo Sales Connect テンプレート ID になります。複数のテンプレートに存在する可能性のある、件名の代わりに特定のテンプレートをターゲットにする場合に使用します。
</td> 
  </tr> 
 </tbody> 
</table>
