---
description: 販売活動の用語集 — Marketoドキュメント — 製品ドキュメント
title: 販売活動の用語集
hide: true
hidefromtoc: true
source-git-commit: 70f17106efe52ee742c8e31013e533fc36ce9835
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 17%

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
  <tr> 
   <td><strong>受信者</strong></td> 
   <td>Eメールを送信した人のEメールアドレス。</td> 
  </tr> 
  <tr> 
   <td><strong>詳細</strong></td> 
   <td>バウンスエラーメッセージの詳細。</td> 
  </tr> 
  <tr> 
   <td><strong>メール</strong></td> 
   <td>バウンスした電子メールアドレス。</td> 
  </tr> 
 </tbody> 
</table>