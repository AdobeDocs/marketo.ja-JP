---
unique-page-id: 2359947
description: エンゲージメントストリーム間でリードを遷移させる — Marketo ドキュメント — 製品ドキュメント
title: エンゲージメントストリーム間でリードを遷移させる
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
feature: Engagement Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 83%

---

# エンゲージメントストリーム間でリードを遷移させる {#transition-people-between-engagement-streams}

エンゲージメントプログラムでは、複数のストリームを使用できます。[ストリームを追加](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md)する場合は、ストリーム間でどのようにリードを遷移させるのかを定義することができます。この定義を&#x200B;**遷移ルール**&#x200B;と呼びます。

1. 「**[!UICONTROL マーケティングアクティビティ]**」に移動します。

   ![](assets/ma.png)

1. ストリームが複数あるエンゲージメントプログラムを選択し、「**[!UICONTROL ストリーム]**」タブに移動します。

   ![](assets/multistream.jpg)

1. 他のストリームから取り込むストリームの「**[!UICONTROL 遷移ルール]**」をクリックし、「**[!UICONTROL 遷移ルールの編集]**」をクリックします。

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >遷移ルールに従って、リードがこのストリームに移ります。必ず、遷移先のストリームでルールを定義します。

   遷移ルールウィンドウが開いたら、選択したトリガーを探してドラッグします。この例では、ユーザーをオポチュニティに追加したときに、そのユーザーを [!UICONTROL &#x200B; 中間ステージ &#x200B;] に移動します。

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. 演算子を「**[!UICONTROL is any]**」に設定し、追加された商談にリードが移動するようにします。

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >1 つの遷移ルールに複数のトリガーやフィルターを用いることはできますが、その遷移ルールではすべてのフィルターを使用します（すべてのフィルターを使用するのが、唯一のオプションです）。遷移ルールで演算子「OR」の使用が必要な場合、代わりに別のスマートキャンペーンを設定することをお勧めします。

1. 「**[!UICONTROL 閉じる]**」をクリックします。

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   完成です。これで、オポチュニティに追加されたエンゲージメントプログラム内の人物は、[!UICONTROL &#x200B; ミッドステージ &#x200B;] ストリームに移動されます。

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >上記の手順は、[一時停止](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md)中のリードにも適用&#x200B;*されます*。
