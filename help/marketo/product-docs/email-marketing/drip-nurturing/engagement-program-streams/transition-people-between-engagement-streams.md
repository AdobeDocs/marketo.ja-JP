---
unique-page-id: 2359947
description: エンゲージメントストリーム間のトランジション者 — Marketto Docs — 製品ドキュメント
title: エンゲージメントストリーム間のトランジションユーザー
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---


# エンゲージメントストリーム間のトランジションユーザー{#transition-people-between-engagement-streams}

エンゲージメントプログラムは複数のストリームを持つことができます。 [ストリーム](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md)を追加する場合は、人々があるストリームから別のストリームに移動する方法を定義する必要があります。 これらは&#x200B;**トランジション規則と呼ばれます。**

1. **マーケティングアクティビティ**&#x200B;に移動します。

   ![](assets/ma.png)

1. マルチストリームエンゲージメントプログラムを選択し、**Streams**&#x200B;に移動します。

   ![](assets/multistream.jpg)

1. 他のストリームから取り込むストリームの&#x200B;**トランジションルール**&#x200B;をクリックし、**トランジションルールの編集**&#x200B;をクリックします。

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >トランジションルールはストリームに引き込まれ、取り込むストリームに対して、常にルールを定義します。

   トランジションルールウィンドウが開いたら、選択したトリガー内で探してドラッグします。 この場合、オポチュニティに追加されたユーザーを中段階に移行させます。

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. 演算子を&#x200B;**はany**&#x200B;に設定し、追加されたオポチュニティに人々が移動できるようにします。

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >1つのトランジションルールに複数のトリガーとフィルターを追加できますが、トランジションルールではすべてのフィルターが使用されます(「すべてのフィルターを使用する」のみ)。 トランジションルールでORを使用する必要がある場合は、代わりに外部のスマートキャンペーンを設定することをお勧めします。

1. 「**閉じる**」をクリックします。

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   素晴らしい！ これで、エンゲージメントプログラム内でオポチュニティに追加されたすべてのユーザーが、中間ステージストリームに移動されます。

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >*do*&#x200B;に示した手順は、pause](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md)の[にある人にも当てはまります。
