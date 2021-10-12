---
description: 販売活動の用語集 — Marketoドキュメント — 製品ドキュメント
title: 販売活動の用語集
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
source-git-commit: 9677c26004a567bb53fef452304665eb73855568
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 12%

---

# 販売活動の用語集 {#sales-activity-glossary}

Sales Connect で、販売者が次の操作を実行したとき。リードを販売サイクルに追加したり、E メールを送信したり、呼び出しをアクティビティにしたりすると、Marketoのアクティビティ履歴に記録されます。 さらに、リードが E メールに関与すると、開封数、クリック数および返信数もログに記録されます。

以下のアクティビティは、Sales Connect からMarketoに記録されます。

>[!NOTE]
>
>これらのアクティビティと属性は、アドビの REST および Bulk API で使用できます。

## アクティビティ {#activities}

<table>
 <tr>
  <th>販売活動</th>
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
  <td>販売テンプレート URL</td>
 </tr>
 <tr>
  <td>販売キャンペーン URL</td>
 </tr>
 <tr>
  <td>販売テンプレート名</td>
 </tr>
 <tr>
  <td>電子メールの件名</td>
 </tr>
 <tr>
  <td>販売キャンペーン名</td>
 </tr>
 <tr>
  <td>Marketo Sales Person ID</td>
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
  <td>販売テンプレート URL</td>
 </tr>
 <tr>
  <td>販売キャンペーン URL</td>
 </tr>
 <tr>
  <td>販売テンプレート名</td>
 </tr>
 <tr>
  <td>電子メールの件名</td>
 </tr>
 <tr>
  <td>販売キャンペーン名</td>
 </tr>
 <tr>
  <td>Marketo Sales Person ID</td>
 </tr>
 <tr>
  <th rowspan="10">販売の電子メールのクリック</th>
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
  <td>販売テンプレート URL</td>
 </tr>
 <tr>
  <td>販売キャンペーン URL</td>
 </tr>
 <tr>
  <td>販売テンプレート名</td>
 </tr>
 <tr>
  <td>電子メールの件名</td>
 </tr>
 <tr>
  <td>販売キャンペーン名</td>
 </tr>
 <tr>
  <td>Marketo Sales Person ID</td>
 </tr>
<tr>
  <th rowspan="3">受信済み販売の電子メール</th>
  <td>受信者</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>ユーザー ID(MSC)</td>
 </tr>
 <tr>
  <th rowspan="11">セールス電話を受信</th>
  <td>セールス電話発信者</td>
 </tr>
 <tr>
  <td>販売呼び出しの状態</td>
 </tr>
 <tr>
  <td>営業電話の件名</td>
 </tr>
 <tr>
  <td>販売キャンペーン名</td>
 </tr>
 <tr>
  <td>販売キャンペーン URL</td>
 </tr>
 <tr>
  <td>電話番号の発信</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>営業コール期間</td>
 </tr>
 <tr>
  <td>セールス電話録音 URL</td>
 </tr>
  <tr>
  <td>セールス電話対応者</td>
 </tr>
 <tr>
  <td>Marketoの販売担当者 ID(MSC)</td>
 </tr>
 <tr>
  <th rowspan="6">セールスキャンペーンに追加</th>
  <td>販売キャンペーン名</td>
 </tr>
 <tr>
  <td>販売呼び出しの状態</td>
 </tr>
 <tr>
  <td>販売キャンペーン URL</td>
 </tr>
 <tr>
  <td>送信者</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>Sales Campaign ID</td>
 </tr>
 <tr>
  <th rowspan="6">販売キャンペーンから削除</th>
  <td>販売キャンペーン名</td>
 </tr>
 <tr>
  <td>販売呼び出しの状態</td>
 </tr>
 <tr>
  <td>販売キャンペーン URL</td>
 </tr>
 <tr>
  <td>送信者</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>Sales Campaign ID</td>
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
   <td><strong>受信者</strong></td> 
   <td>E メールを送信した人の E メールアドレス。</td> 
  </tr>
  <tr> 
   <td><strong>セールス電話対応者</strong></td> 
   <td>通話に回答した人の名前。</td> 
  </tr>
  <tr> 
   <td><strong>営業コール期間</strong></td> 
   <td>呼び出しの長さ（秒）。</td> 
  </tr>
  <tr> 
   <td><strong>セールス電話発信者</strong></td> 
   <td>通話を行った販売担当者の電子メールアドレス。</td> 
  </tr>
  <tr> 
   <td><strong>セールス電話録音 URL</strong></td> 
   <td>呼び出し記録の URL。</td> 
  </tr>
  <tr> 
   <td><strong>販売呼び出しの状態</strong></td> 
   <td>次を含む呼び出しの最終的な呼び出しステータスを保存します。完了、回答なし、キャンセル、失敗</td> 
  </tr>
  <tr> 
   <td><strong>営業電話の件名</strong></td> 
   <td>ダイヤラ内の販売ユーザーが選択したコール結果。</td> 
  </tr>
  <tr> 
   <td><strong>Sales Campaign ID</strong></td> 
   <td>Sales Connect の Sales Campaign アセットの一意の ID。</td> 
  </tr>
  <tr> 
   <td><strong>販売キャンペーン名</strong></td> 
   <td>Sales Campaign の名前。</td> 
  </tr>
  <tr> 
   <td><strong>販売キャンペーン URL</strong></td> 
   <td>Sales Connect URL は、Sales Campaign 用です。</td> 
  </tr>
  <tr> 
   <td><strong>販売の電子メールの件名</strong></td> 
   <td>電子メールの件名行。</td> 
  </tr>
  <tr> 
   <td><strong>電話番号の発信</strong></td> 
   <td>営業から電話番号。</td> 
  </tr>
  <tr> 
   <td><strong>販売テンプレート名</strong></td> 
   <td>Sales Connect の電子メールテンプレートの名前。</td> 
  </tr>
  <tr> 
   <td><strong>販売テンプレート URL</strong></td> 
   <td>Sales Connect 電子メールテンプレートの URL。</td> 
  </tr>
  <tr> 
   <td><strong>送信者</strong></td>
   <td>E メールを送信した人の E メールアドレス。</td> 
  </tr> 
  <tr> 
   <td><strong>ソース</strong></td> 
   <td>アクティビティのソース。 Sales Connect アクティビティの「Tout」に設定されます。</td> 
  </tr> 
  <tr> 
   <td><strong>テンプレート ID</strong></td> 
   <td>ソースが Tout の場合、テンプレート ID はMarketo Sales Connect テンプレート ID になります。 複数のテンプレートに存在する可能性のある件名行ではなく、特定のテンプレートをターゲットにする場合に使用します。
</td> 
  </tr> 
 </tbody> 
</table>
