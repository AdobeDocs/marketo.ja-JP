---
description: セールス活動用語集 — Marketoドキュメント — 製品ドキュメント
title: セールス活動用語集
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
source-git-commit: d261da2a2784ab322ef78fe22ef3d6b4321fc806
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 11%

---

# セールス活動用語集 {#sales-activity-glossary}

セールスコネクトで、販売者が以下を実行したとき：セールスケイデンスにリードを追加したり、メールを送信したり、通話をアクティビティに送信したりすると、Marketoのアクティビティ履歴に記録されます。 さらに、リードがメールに関与した場合、開封数、クリック数、返信数もログに記録されます。

以下のアクティビティは、セールスコネクトからMarketoに記録されます。

>[!NOTE]
>
>これらのアクティビティと属性は、アドビの REST および Bulk API から使用できます。

## アクティビティ {#activities}

<table>
 <tr>
  <th>セールス活動</th>
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
  <td>電子メールの件名</td>
 </tr>
 <tr>
  <td>セールスキャンペーン名</td>
 </tr>
 <tr>
  <td>Marketoセールス担当者 ID</td>
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
  <td>電子メールの件名</td>
 </tr>
 <tr>
  <td>セールスキャンペーン名</td>
 </tr>
 <tr>
  <td>Marketoセールス担当者 ID</td>
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
  <td>電子メールの件名</td>
 </tr>
 <tr>
  <td>セールスキャンペーン名</td>
 </tr>
 <tr>
  <td>Marketoセールス担当者 ID</td>
 </tr>
<tr>
  <th rowspan="3">セールスメールに返信済み</th>
  <td>受信者</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>Marketoセールス担当者 ID</td>
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
  <td>電話番号の受信</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>営業電話の期間</td>
 </tr>
 <tr>
  <td>セールス電話録音 URL</td>
 </tr>
  <tr>
  <td>セールス電話対応者</td>
 </tr>
 <tr>
  <td>Marketoセールス担当者 ID</td>
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
   <td>バウンスした電子メールアドレス。</td> 
  </tr> 
  <tr> 
   <td><strong>リンク</strong></td> 
   <td>クリックされた URL。</td> 
  </tr> 
  <tr> 
   <td><strong>Marketoセールス担当者 ID</strong></td> 
   <td>セールスコネクトの人物レコードの一意の ID。</td> 
  </tr> 
  <tr> 
   <td><strong>受信者</strong></td> 
   <td>電子メールを送信した人の電子メールアドレス。</td> 
  </tr>
  <tr> 
   <td><strong>セールス電話対応者</strong></td> 
   <td>電話に出た人の名前。</td> 
  </tr>
  <tr> 
   <td><strong>営業電話の期間</strong></td> 
   <td>呼び出しの長さ（秒）。</td> 
  </tr>
  <tr> 
   <td><strong>セールス電話発信者</strong></td> 
   <td>電話をした販売担当者のメールアドレス。</td> 
  </tr>
  <tr> 
   <td><strong>セールス電話録音 URL</strong></td> 
   <td>通話記録の URL。</td> 
  </tr>
  <tr> 
   <td><strong>セールス電話のステータス</strong></td> 
   <td>呼び出しの最終的な呼び出しステータスを保存します。このステータスには次が含まれます。完了、回答なし、キャンセル、失敗。</td> 
  </tr>
  <tr> 
   <td><strong>セールス電話の件名</strong></td> 
   <td>ダイヤラ内のセールスユーザーによって選択されたコールの結果。</td> 
  </tr>
  <tr> 
   <td><strong>セールスキャンペーン ID</strong></td> 
   <td>セールスコネクトのセールスキャンペーンアセットの一意の ID。</td> 
  </tr>
  <tr> 
   <td><strong>セールスキャンペーン名</strong></td> 
   <td>セールスキャンペーンの名前。</td> 
  </tr>
  <tr> 
   <td><strong>セールスキャンペーン URL</strong></td> 
   <td>セールスキャンペーンのセールスコネクト URL。</td> 
  </tr>
  <tr> 
   <td><strong>セールスメールの件名</strong></td> 
   <td>電子メールの件名行に一意の ID を付ける ( 例：件名 (MSC-12345678)</td> 
  </tr>
  <tr> 
   <td><strong>電話番号の受信</strong></td> 
   <td>セールスから呼び出された電話番号。</td> 
  </tr>
  <tr> 
   <td><strong>セールステンプレート名</strong></td> 
   <td>セールスコネクトのメールテンプレートの名前。</td> 
  </tr>
  <tr> 
   <td><strong>セールステンプレート URL</strong></td> 
   <td>メールテンプレートのセールスコネクト URL。</td> 
  </tr>
  <tr> 
   <td><strong>送信者</strong></td>
   <td>電子メールを送信した人の電子メールアドレス。</td> 
  </tr> 
  <tr> 
   <td><strong>ソース</strong></td> 
   <td>アクティビティのソース。 2021 年 10 月のリリースより前に、セールスコネクトアクティビティの「Tout」に設定されます。 2021 年 10 月のリリース以降、セールスコネクトアクティビティの「セールスアプリ」になります。</td>
  </tr> 
  <tr> 
   <td><strong>テンプレート ID</strong></td> 
   <td>ソースが Tout の場合、テンプレート ID はMarketoセールスコネクトテンプレート ID になります。 複数のテンプレートに存在する可能性のある、件名の代わりに特定のテンプレートをターゲットにする場合に使用します。
</td> 
  </tr> 
 </tbody> 
</table>
