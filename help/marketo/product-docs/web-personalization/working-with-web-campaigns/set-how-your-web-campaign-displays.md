---
unique-page-id: 12978906
description: Web キャンペーンの表示方法を設定して、Marketo Engageでのweb キャンペーンの表示方法を設定する方法について説明します。 このガイドを使用して、次のステップを完了してください。
title: Web キャンペーンの表示方法の設定
exl-id: fa0f2421-9536-4a3a-a28b-4f5b1b58ed56
feature: Web Personalization
TQID: https://experienceleague.adobe.com/HIEbtOzKJ0bSHfPY6W-LHBI-HStuLGqx7RFGqyWA8Co
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 235
ht-degree: 88%

---

# Web キャンペーンの表示方法の設定 {#set-how-your-web-campaign-displays}

Web キャンペーンがいつ、どのように表示されるかに関して、いつ利用するかに関しては、いくつかの方法があります。

## ページ読み込み {#page-load}

デフォルトで選択されています。この選択では、ページの読み込み時にキャンペーンが表示されます。

![](assets/pl1.png)

## 遅延 {#delay}

ウェブサイト上で web キャンペーンが反応するまでの時間の遅延（合計秒数）を指定します。

1. **[!UICONTROL 表示先]**&#x200B;ドロップダウンをクリックして、「**[!UICONTROL 遅延]**」を選択します。

   ![](assets/d1.png)

1. **[!UICONTROL 待機]**&#x200B;ドロップダウンをクリックして、目的の時間を選択します。

   ![](assets/d2.png)

## スクロール {#scroll}

1. **[!UICONTROL 表示先]**&#x200B;ドロップダウンをクリックして「**[!UICONTROL スクロール]**」を選択します。

   ![](assets/s1.png)

1. **[!UICONTROL タイミング]**&#x200B;ドロップダウンをクリックし、web キャンペーンを表示するタイミングを選択します。

   ![](assets/s2.png)

<table>
 <tbody>
  <tr>
   <td><strong>[!UICONTROL 下の折り目]</strong></td>
   <td>訪問者がスクロールしなければ見えない画面領域にまでスクロールすると、キャンペーンが表示されます。 訪問者がスクロールしないで閲覧する事のできる画面領域に戻ると、キャンペーンは非表示になります。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL パーセント]</strong></td>
   <td>訪問者がページの事前に決定された割合にスクロールした場合に、キャンペーンが表示されます。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL ピクセル]</strong></td>
   <td><p>訪問者がページの事前に指定された最上位ピクセルにスクロールすると、キャンペーンが表示されます。</p></td>
  </tr>
 </tbody>
</table>

## エグジットインテント {#exit-intent}

ブラウザーのマウスカーソル終了時に web キャンペーンが表示されます。

1. **[!UICONTROL 表示先]**&#x200B;ドロップダウンをクリックして「**[!UICONTROL エグジットインテント]**」を選択します。

   ![](assets/ei1.png)

1. [!UICONTROL エグジットインテント]がモバイルと互換性がないことを示すメッセージが表示されます。

   ![](assets/ei2.png)

>[!TIP]
>
>選択した効果がどう見えるかを事前に確認したい場合は、 [web キャンペーンプレビュー](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/preview-and-test-a-web-campaign.md)を使用して確認します。
