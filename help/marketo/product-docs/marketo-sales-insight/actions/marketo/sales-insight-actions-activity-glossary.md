---
description: Sales Insight アクションアクティビティの用語集 — Marketoドキュメント — 製品ドキュメント
title: Sales Insight アクションアクティビティの用語集
hide: true
hidefromtoc: true
source-git-commit: a0cfc190e00ea6f8a9f5ef717566651423638b7d
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 66%

---

# Sales Insight アクションアクティビティの用語集 {#sales-insight-actions-activity-glossary}

Sales Insight アクションで、販売者が次の操作を実行したとき：リードをセールスキャンペーンに追加したり、セールスメールを送信したり、アウトバウンドのセールス電話をかけたりすると、そのリードのMarketoアクティビティ履歴に記録されます。 また、リードがメール、開封、クリック、返信に関与した場合も、ログに記録されます。

以下のアクティビティは、Sales Insight アクションからMarketoに記録されます。

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
   <td>Sales Insight アクションの担当者レコードの一意の ID。</td> 
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
   <td>Sales Insight アクションの Sales Campaign アセットの一意の ID。</td> 
  </tr>
  <tr> 
   <td><strong>セールスキャンペーン名</strong></td> 
   <td>セールスキャンペーンの名前。</td> 
  </tr>
  <tr> 
   <td><strong>セールスキャンペーン URL</strong></td> 
   <td>Sales Insight アクション URL （セールスキャンペーン用）。</td> 
  </tr>
  <tr> 
   <td><strong>セールスメールの件名</strong></td> 
   <td>電子メールの件名行に一意の ID を付ける ( 例：私の件名 (SIA-12345678)</td> 
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
   <td>Sales Insight アクション URL （メールテンプレート用）。</td> 
  </tr>
  <tr> 
   <td><strong>送信者</strong></td>
   <td>メール送信者のメールアドレス。</td> 
  </tr> 
  <tr> 
   <td><strong>ソース</strong></td> 
   <td>アクティビティのソース。2021 年 10 月のリリースより前の Sales Insight Actions アクティビティでは、「Tout」に設定されます。 2021 年 10 月のリリース以降、Sales Insight Actions アクティビティの「Sales App」になります。</td>
  </tr> 
  <tr> 
   <td><strong>テンプレート ID</strong></td> 
   <td>ソースが Tout の場合、テンプレート ID はMarketo Sales Insight Actions Template ID になります。 複数のテンプレートに存在する可能性のある、件名の代わりに特定のテンプレートをターゲットにする場合に使用します。
</td> 
  </tr> 
 </tbody> 
</table>
