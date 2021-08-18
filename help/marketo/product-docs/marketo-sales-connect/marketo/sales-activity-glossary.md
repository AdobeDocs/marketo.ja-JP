---
description: 販売活動の用語集 — Marketoドキュメント — 製品ドキュメント
title: 販売活動の用語集
source-git-commit: 9f8d6895e88250afc2799b2fb7fc73442018362f
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 14%

---

# 販売活動の用語集 {#sales-activity-glossary}

Sales Connectで、販売者が次の操作を実行した場合：販売サイクルにリードを追加したり、電子メールを送信したり、呼び出しをアクティビティにしたりすると、Marketoのアクティビティ履歴に記録されます。 さらに、リードがEメールに関与すると、開封数、クリック数および返信数もログに記録されます。

以下のアクティビティは、Sales ConnectからMarketoに記録されます。

>[!NOTE]
>
>これらのアクティビティと属性は、アドビのRESTおよび一括APIで使用できます。

## アクティビティ {#activities}

<table>
 <tr>
  <th>販売活動</th>
  <th>属性</th>
 </tr>
 <tr>
  <th rowspan="3">セールスメールの送信</th>
  <td>送信者</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>テンプレート ID</td>
 </tr>
 <tr>
  <th rowspan="3">セールスメールを開く</th>
  <td>送信者</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>テンプレート ID</td>
 </tr>
 <tr>
  <th rowspan="4">販売の電子メールをクリック</th>
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
  <th rowspan="2">受信済み販売の電子メール</th>
  <td>受信者</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <th rowspan="4">セールスメールバウンス</th>
  <td>詳細</td>
 </tr>
 <tr>
  <td>テンプレート ID</td>
 </tr>
 <tr>
  <td>メール</td>
 </tr>
 <tr>
  <td>送信者</td>
 </tr>
 <tr>
  <th rowspan="7">セールス電話を受信しました</th>
  <td>セールス電話発信者</td>
 </tr>
 <tr>
  <td>販売呼び出しステータス</td>
 </tr>
 <tr>
  <td>営業電話の件名</td>
 </tr>
 <tr>
  <td>販売キャンペーン名</td>
 </tr>
 <tr>
  <td>販売キャンペーンURL</td>
 </tr>
 <tr>
  <td>電話番号の受信</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <th rowspan="6">セールスキャンペーンに追加</th>
  <td>販売キャンペーン名</td>
 </tr>
 <tr>
  <td>販売呼び出しステータス</td>
 </tr>
 <tr>
  <td>販売キャンペーンURL</td>
 </tr>
 <tr>
  <td>送信者</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>販売キャンペーンID</td>
 </tr>
 <tr>
  <th rowspan="6">販売キャンペーンから削除</th>
  <td>販売キャンペーン名</td>
 </tr>
 <tr>
  <td>販売呼び出しステータス</td>
 </tr>
 <tr>
  <td>販売キャンペーンURL</td>
 </tr>
 <tr>
  <td>送信者</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>販売キャンペーンID</td>
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
   <td>クリックされたURL。</td> 
  </tr> 
  <tr> 
   <td><strong>受信者</strong></td> 
   <td>Eメールを送信した人のEメールアドレス。</td> 
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
   <td>電話をかけた営業担当者の電子メールアドレス。</td> 
  </tr>
  <tr> 
   <td><strong>セールス電話録音 URL</strong></td> 
   <td>通話記録のURL。</td> 
  </tr>
  <tr> 
   <td><strong>販売呼び出しステータス</strong></td> 
   <td>次を含む呼び出しの最終呼び出しステータスを保存します。完了、回答なし、キャンセル、失敗。</td> 
  </tr>
  <tr> 
   <td><strong>営業電話の件名</strong></td> 
   <td>ダイヤラの販売ユーザーが選択したコール結果。</td> 
  </tr>
  <tr> 
   <td><strong>販売キャンペーンID</strong></td> 
   <td>Sales ConnectのSales Campaignアセットの一意のID。</td> 
  </tr>
  <tr> 
   <td><strong>販売キャンペーン名</strong></td> 
   <td>Sales Campaignの名前。</td> 
  </tr>
  <tr> 
   <td><strong>販売キャンペーンURL</strong></td> 
   <td>Sales Connect URLのSales Campaign。</td> 
  </tr>
  <tr> 
   <td><strong>販売の電子メールの件名</strong></td> 
   <td>電子メールの件名行。</td> 
  </tr>
  <tr> 
   <td><strong>電話番号の受信</strong></td> 
   <td>Salesから呼び出された電話番号。</td> 
  </tr>
  <tr> 
   <td><strong>販売テンプレート名</strong></td> 
   <td>Sales Connectの電子メールテンプレートの名前。</td> 
  </tr>
  <tr> 
   <td><strong>販売テンプレートURL</strong></td> 
   <td>電子メールテンプレートの販売接続URL。</td> 
  </tr>
  <tr> 
   <td><strong>送信者</strong></td>
   <td>Eメールを送信した人のEメールアドレス。</td> 
  </tr> 
  <tr> 
   <td><strong>ソース</strong></td> 
   <td>アクティビティのソース。 Sales Connectアクティビティの「Tout」に設定されます。</td> 
  </tr> 
  <tr> 
   <td><strong>テンプレート ID</strong></td> 
   <td>ソースが「Tout」の場合、テンプレートIDはMarketo Sales Connect Template IDになります。 複数のテンプレートに存在する件名行ではなく、特定のテンプレートをターゲットにする場合に使用します。
</td> 
  </tr> 
 </tbody> 
</table>