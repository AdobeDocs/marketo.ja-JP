---
unique-page-id: 13796471
description: ライブフィードの概要 - Marketo ドキュメント - 製品ドキュメント
title: ライブフィードの概要
exl-id: 646a3650-538d-4ea5-b29f-44ad6588e247
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 100%

---

# ライブフィードの概要 {#live-feed-overview}

ライブフィードは、web アプリケーションまたは Gmail プラグインから起動できるフローティングウィンドウで、見込み客のエンゲージメントをリアルタイムで確認できます。

## 「エンゲージメント」タブ {#engagement-tab}

![](assets/engagement.jpg)

MSE メールのエンゲージメント（表示、クリック、返信）をリアルタイムで確認できます。

紫色のマークが付いたリードはマーケティングコンテンツに関心を持っています。これらのリードは MSE に存在しない可能性があります。下向き矢印をクリックして追加し、その他のクイックアクションの一覧を表示できます。

![](assets/purple.png)

青い線でマークされたリードは、MSE を通じて送信されたメールとのエンゲージメントを表します。

>[!NOTE]
>
>一般的に、場所は IP トラッキングに基づいて可能な限り正確に特定されていますが、残念ながらこれは精密科学ではありません。受信者の 1 人に対して場所が正しくない場合、その理由に関するいくつかのオプションを次に示します。
>
>* 受信者が、自社の IT 本部が別の都市や国にある企業のワイヤレスネットワークにログインした場合、受信者の現在のロケールではなく、その場所がログに記録されます。
>* メールが CC／BCC フィールドに入力されている人によって転送または開封された場合、それらの人々がいる場所を正確に表示しようとします。


## 「タスク」タブ {#tasks-tab}

![](assets/task.jpg)

ライブフィードから TODO リストをすばやく確認します。

新規作成するか、開いているタスクを管理します。

今日、明日、今日&#x200B;*と*&#x200B;明日、または次の 7 日間をフィルタリングできます。

>[!NOTE]
>
>カスタムの日付フィルターはライブフィードでは使用できませんが、web アプリケーションでは使用できます。

クイックアクションボタンを使用して、通話、メールの送信、リードの Linkedin プロファイルへの移動をすばやくおこなうことができます。

## 「ターゲット」タブ {#target-tab}

![](assets/target.jpg)

リードスコア別にランク付けされた上位のリードを確認できます（リードは最上位から最下位の順になっています）。リードスコアは Marketo インスタンスから引き出されます。

* リードは、Marketo でユーザースコアが増加すると生成されます。
* 上位 50 名のリードが表示されます。
* Salesforce で割り当てられたリードのみが表示されます。

## アイコン用語集 {#icon-glossary}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td> 
    <div> 
     <p><img alt="--" height="22" src="assets/viewed-icon.png" data-linked-resource-id="45417223" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="13796471" title="--"></p> 
    </div></td> 
   <td><p>誰かがあなたのメールを閲覧しました</p></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <p><img alt="--" src="assets/clicked-icon.png" data-linked-resource-id="45417224" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="13796471" title="--"></p> 
    </div></td> 
   <td><p>誰かがあなたのメール内のリンクをクリックしました</p></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <p><img alt="--" width="23" src="assets/replied-icon.png" data-linked-resource-id="45417226" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="13796471" title="--"></p> 
    </div></td> 
   <td><p>誰かがあなたのメールに返信しました</p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <div> 
     <p><img alt="--" width="20" src="assets/im-icon.png" data-linked-resource-id="45417225" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="13796471" title="--"></p> 
    </div></td> 
   <td colspan="1">メール、Web、マイルストーンを含む、注目のアクションにリストされた通知</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>誰かがライブフィードでメールを何度も閲覧している場合は、そのメールを追加の受信者に転送している可能性があります。表示の場所が変更され始めたことに気付いたら、多くの場合これが理由です。
