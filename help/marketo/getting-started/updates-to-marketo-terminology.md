---
unique-page-id: 11387674
description: マーケティング用語 — マーケティングツールドキュメント — 製品ドキュメントの更新
title: マーケティングの用語の更新
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---


# マーケティングの用語の更新 {#updates-to-marketo-terminology}

プラットフォームに変更を加えています。これは、何と呼ばれるかに影響を与えます。 2016年3月時点で新しいMarketoインスタンスがある場合、または2016年7月以降に会社が更新された場合は、現在新しい用語が表示されている可能性があります。

Marketoのドキュメントには様々な用語が記載されていますが、これらの変更を反映するために、すべての記事がすぐに更新されます。 すべての手順は同じです。

何が変わったの？

## リードが現在の人 {#lead-is-now-person}

最大の変更点は、個人/人に対するリード/リードの名前変更です。

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>古い</strong></td> 
   <td><strong>新規</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img width="295" src="assets/leads.png" data-linked-resource-id="11387678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img width="295" src="assets/people.png" data-linked-resource-id="11387679" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

場合によっては、「Lead」という単語が単に削除されることがあります。

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>古い</strong></td> 
   <td><strong>新規</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/lead-database.png" data-linked-resource-id="11387676" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <p><img src="assets/database.png" data-linked-resource-id="11387677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"></p> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

鉛と人 **は同じもの**。

## トークン {#tokens}

leadという単語を含むトークン **は変更されません**。 ご混乱をおかけして申し訳ございません。ただし、新しい用語に一致するようにすべてのトークンを変更すると、現在使用中のトークンが大量に破棄されます。 「`{{lead.First Name}}`」などのトークンは引き続き表示されます。 個人固有のトークンはありません。

>[!NOTE]
>
>「人 *物ノート* 」と呼ばれるトークンがありますが、常にそのトークンが存在していました。 この変数は、CRMの説明フィールドに使用されます（すべての場合）。

## フィールド管理 {#field-management}

「Lead」という用語を含むフィールドは、「Person」で置き換えられたか、「Lead」という語がドロップされました。 ただし、「Lead Owner（リードの所有者）」フィールドは例外です。 現在は「Sales Owner（販売所有者）」と呼ばれています。

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>古い</strong></td> 
   <td><strong>新規</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/lead-owner.png" data-linked-resource-id="11387757" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img src="assets/sales-owner.png" data-linked-resource-id="11387758" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>影響を受けるフィールド名の完全なリストについては、この [サポート記事を参照してください](https://nation.marketo.com/docs/DOC-4218#jive_content_id_Field_Names_and_Tokens)。

## リアルタイムパーソナライゼーション(RTP)がウェブパーソナライゼーションに {#real-time-personalization-rtp-is-now-web-personalization}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>古い</strong></td> 
   <td><strong>新規</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/rtp.png" data-linked-resource-id="11387692" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img src="assets/web.png" data-linked-resource-id="11387693" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

名前の変更に加え、4つの個別のアプリで構成されるようになりました。

| ** [Webパーソナライゼーション](http://docs.marketo.com/display/DOCS/Web+Personalization+-+RTP)** | ホーム画面に独自のタイルを表示 |
|---|---|
| ** [アカウントベースのWebマーケティング](http://docs.marketo.com/display/DOCS/Account-Based+Web+Marketing)** | Webパーソナライゼーションタイルを使用してアクセス可能 |
| ** [パーソナライズされたリターゲティング](http://docs.marketo.com/display/DOCS/Website+Retargeting)** | Webパーソナライゼーションタイルを使用してアクセス可能 |
| ** [予測コンテンツ](http://docs.marketo.com/display/DOCS/Predictive+Content)** | ホーム画面に独自のタイルを表示 |

>[!NOTE]
>
>ホーム画面に表示されるタイルには、購入したモジュールが反映されます。

更新中、ご辛抱ありがとうございました。

