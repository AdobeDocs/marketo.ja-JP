---
description: 対話型フローの概要 – Marketo ドキュメント – 製品ドキュメント
title: 対話型フローの概要
feature: Dynamic Chat
exl-id: c741886d-d672-471f-8902-208d25898afa
source-git-commit: 14ccfe39059b9c900a5e5e00b082146bb500d79d
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 3%

---

# 対話型フローの概要 {#conversational-flow-overview}

会話フローを設計し、特定のアクション（コールトゥアクションボタンのクリック、ページ読み込み時、ページでの滞在時間など）に基づいて任意の訪問者にトリガー付けします。

![](assets/conversational-flow-overview-1.png)

## ダイアログと会話フロー {#dialogues-vs-conversational-flows}

ダイアログと会話フローにはいくつかの類似点がありますが、2 つの異なる機能があります。

<table> 
 <tbody> 
  <tr> 
   <th style="width:50%">ダイアログ</th> 
   <th style="width:50%">対話型フロー</th>
  </tr> 
  <tr> 
   <td>ダイアログはターゲット設定されます。実装したパラメーターに基づいて、特定のページおよびオーディエンス向けの会話をデザインします。</td> 
   <td>会話フローがトリガーされる – フォームの入力やリンクのクリックなど、訪問者のアクションに基づいてトリガーできる会話をデザインします。</td>
  </tr>
   <tr> 
   <td>Chatbot インターフェイスでのみサポートされます。</td> 
   <td>現在は、より多くのインターフェイスが計画されているポップアップインターフェイスでサポートされています。</td>
  </tr>
  </tr>
   <tr> 
   <td>同じリードセグメントに対して優先順位を付けて複数のダイアログを作成できるので、各訪問者は、引き続きエンゲージしながら、優先順位に従ってダイアログを表示できます。</td> 
   <td>会話フローには優先順位がなく、決定されたコールトゥアクションに基づいて、同じリードで任意の回数トリガーできます。</td>
  </tr>
  <tr>
   <td>チャットボットの会話はダイアログによって実現します。</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">会話Forms</a> Marketo Engageでは、対話型フローを活用します。</td>
  </tr>
 </tbody> 
</table>

## 「ストリームデザイナー」タブ {#stream-designer-tab}

対話型フローのストリーム デザイナは、ダイアログのストリーム デザイナとほとんど同じです。 [詳しくは、こちらを参照してください](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"}.

![](assets/conversational-flow-overview-2.png)

## 「レポート」タブ {#reports-tab}

「レポート」タブでは、会話フローのパフォーマンスに関する指標を確認できます。

![](assets/conversational-flow-overview-3.png)

エンゲージメント率、コンバージョン率、既知の訪問者や不明な訪問者でフィルタリングしたなどを表示します。

![](assets/conversational-flow-overview-4.png)

## 「設定」タブ {#settings-tab}

![](assets/conversational-flow-overview-5.png)

「設定」タブの上半分では、会話フローの名前を更新し、オプションで説明を追加して、言語を変更できます。

![](assets/conversational-flow-overview-6.png)

>[!NOTE]
>
>別の言語を選択すると、システムテキストの言語のみが変更されます。 コンテンツの翻訳は、あなたが担当します。

### 会話 SDK {#conversations-sdk}

「設定」タブの下半分で、「Conversation」トリガー（「Conversations SDK」とも呼ばれる）をカスタマイズします。 訪問者がリンクをクリックしたとき、またはページを読み込んだときに、web サイトで会話をトリガーするかどうかを指定できます。

![](assets/conversational-flow-overview-7.png)

>[!TIP]
>
>参照： [会話 SDK](https://experienceleague.adobe.com/tools/marketo-dynamic-chatbot/conversations-sdk/){target="_blank"} 実行中！

>[!MORELIKETHIS]
>
>[会話フローの作成](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-conversational-flow.md){target="_blank"}
