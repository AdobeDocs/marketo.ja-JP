---
unique-page-id: 2359947
description: エンゲージメントストリーム間でユーザーを移動するための移行ルールを設定する方法を説明します。 取り込むストリームにルールを定義します。
title: エンゲージメントストリーム間でリードを遷移させる
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
feature: Engagement Programs
TQID: https://experienceleague.adobe.com/viGLYAkvGqF-9K5bhAHWDSOMYaiBuKRe8F2QginuYps
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 243
ht-degree: 62%

---

# エンゲージメントストリーム間でリードを遷移させる {#transition-people-between-engagement-streams}

エンゲージメントプログラムでは、複数のストリームを使用できます。 [ ストリームを追加](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md)する場合は、ユーザーがストリームから別のストリームに移動する方法を定義します。 この定義を&#x200B;**遷移ルール**&#x200B;と呼びます。

1. **[!UICONTROL マーケティングアクティビティ]**&#x200B;に移動します。

   ![](assets/ma.png)

1. ストリームが複数あるエンゲージメントプログラムを選択し、「**[!UICONTROL ストリーム]**」タブに移動します。

   ![](assets/multistream.jpg)

1. 他のストリームから取り込むストリームの「**[!UICONTROL 遷移ルール]**」をクリックし、「**[!UICONTROL 遷移ルールの編集]**」をクリックします。

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >遷移ルールに従って、リードがこのストリームに移ります。必ず、遷移先のストリームでルールを定義します。

   遷移ルールウィンドウが開いたら、選択したトリガーを探してドラッグします。 この例では、人物は商談に追加されると[!UICONTROL  ミッドステージ ]に移動されます。

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. 演算子を&#x200B;**[!UICONTROL is any]**&#x200B;に設定して、追加された商談に対してユーザーが移動できるようにします。

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >1 つの遷移ルールに複数のトリガーやフィルターを用いることはできますが、その遷移ルールではすべてのフィルターを使用します（すべてのフィルターを使用するのが、唯一のオプションです）。 トランジションルールでORを使用する必要がある場合は、代わりに外部スマートキャンペーンを設定することをお勧めします。

1. 「**[!UICONTROL 閉じる]**」をクリックします。

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   これで、エンゲージメントプログラムのリードが商談に追加された場合、その人物は[!UICONTROL 中間ステージ]ストリームに遷移します。

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >上記の手順は、[一時停止](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md)中の人物にも適用&#x200B;*されます*。
