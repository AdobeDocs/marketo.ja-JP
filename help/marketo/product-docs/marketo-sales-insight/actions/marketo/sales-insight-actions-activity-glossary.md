---
description: Sales Insight Actions アクティビティ用語集 - Marketo ドキュメント - 製品ドキュメント
title: Sales Insight Actions アクティビティ用語集
exl-id: fd0f632c-6f0d-49f9-a805-0730595c81fd
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 100%

---

# Sales Insight Actions アクティビティ用語集 {#sales-insight-actions-activity-glossary}

Sales Insight Actions で、販売者がセールスキャンペーンにリードを追加したり、セールスメールを送信したり、セールス通話発信を行ったりすると、そのリードのアクティビティ履歴が Marketo に記録されます。さらに、リードがメールに関与した場合、開封数、クリック数、返信数もログに記録されます。

以下のアクティビティは、Sales Insight Actions から Marketo に記録されます。

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
  <th rowspan="9">セールスメールを送信</th>
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
  <th rowspan="10">セールスメールをクリック</th>
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
  <th rowspan="3">セールスメールに返信</th>
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
   <td>Sales Insight Actions の人物レコードの一意の ID。</td> 
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
   <td>ダイヤラー内でセールスユーザによって選択された電話の結果。</td> 
  </tr>
  <tr> 
   <td><strong>セールスキャンペーン ID</strong></td> 
   <td>Sales Insight Actions のセールスキャンペーンアセットの一意の ID。</td> 
  </tr>
  <tr> 
   <td><strong>セールスキャンペーン名</strong></td> 
   <td>セールスキャンペーンの名前。</td> 
  </tr>
  <tr> 
   <td><strong>セールスキャンペーン URL</strong></td> 
   <td>セールスキャンペーンの Sales Insight Actions の URL。</td> 
  </tr>
  <tr> 
   <td><strong>セールスメールの件名</strong></td> 
   <td>メールの件名行と一意の ID（例：件名（SIA-12345678）</td> 
  </tr>
  <tr> 
   <td><strong>セールス電話の発信先電話番号</strong></td> 
   <td>セールスが発信した電話番号。</td> 
  </tr>
  <tr> 
   <td><strong>セールステンプレート名</strong></td> 
   <td>Sales Insight Actions のメールテンプレートの名前。</td> 
  </tr>
  <tr> 
   <td><strong>セールステンプレート URL</strong></td> 
   <td>メールテンプレートの Sales Insight Actions の URL。</td> 
  </tr>
  <tr> 
   <td><strong>送信者</strong></td>
   <td>メール送信者のメールアドレス。</td> 
  </tr> 
  <tr> 
   <td><strong>ソース</strong></td> 
   <td>アクティビティのソース。2021年10月のリリースより前では Sales Insight Actions のアクティビティは「Tout」に設定されます。2021年10月のリリースより後では Sales Insight Actions のアクティビティは「Sales App」に設定されます。</td>
  </tr> 
  <tr> 
   <td><strong>テンプレート ID</strong></td> 
   <td>ソースが Tout の場合、テンプレート ID は Marketo Sales Insight Actions のテンプレート ID になります。複数のテンプレートに存在する可能性のある件名の代わりに、特定のテンプレートをターゲットにする場合に使用します。
</td> 
  </tr> 
 </tbody> 
</table>
