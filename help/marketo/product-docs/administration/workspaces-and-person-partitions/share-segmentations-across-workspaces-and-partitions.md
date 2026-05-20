---
unique-page-id: 7515767
description: ワークスペースとパーティション間でセグメントを共有するためのルールと手順（デフォルトワークスペースでセグメントを作成するための制限とヒントを含む）。
title: ワークスペースとパーティションをまたいだセグメント化の共有
exl-id: b50f4328-fdba-4e39-bc0d-75bade1f9cbc
feature: Partitions, Workspaces
TQID: https://experienceleague.adobe.com/fzHumE5x1Y5tSVjUUlHabe-cZgPC5jmqwtl4aLYhjDA
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: cdd4e0f6-e87e-453f-88ee-2ee54a7de272
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 471
ht-degree: 75%

---

# ワークスペースとパーティションをまたいだセグメント化の共有 {#share-segmentations-across-workspaces-and-partitions}

>[!PREREQUISITES]
>
>この記事は、ワークスペースとパーティションをお使いのお客様専用です。

## セグメンテーションとは？ {#whats-a-segmentation}

Marketoは、プログラムやスマートキャンペーンに適した人物を特定します。 ただし、より永続的なペルソナの場合は、セグメント化を使用する必要があります。 セグメント化は、Marketo で高度な動的コンテンツを使用するために必要です。

>[!NOTE]
>
>[セグメント化の作成方法](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)を参照してください。

これらのペルソナを設定したら（_および_&#x200B;ワークスペースを使用している場合）、ワークスペース全体で共有します。 次に、知っておくといい点を示します。

## ルールとヒント {#rules-tips}

* 各 Marketo サブスクリプションには、複数のワークスペースをまたいで最大 20 個のセグメントを「合計」で含めることができます（**1 ワークスペースあたり 20 ではありません**）。
* セグメント化は、アクセス権のあるワークスペースとのみ共有できます。
* すべてのパーティションを可視化する&#x200B;**デフォルトのワークスペース**&#x200B;を作成して活用します。

* セグメント化処理は、セグメント化が作成されたワークスペース内の人物に対してのみ実行されます。

   * デフォルトのワークスペース内で共有するセグメントを作成します。
      * セグメント化の承認
      * 共有ワークスペースにはロックされたフォルダーが表示され、セグメント化は読み取り専用です。
      * 共有バージョンは編集できません。 元のセグメントを作成した場所でのみ編集できます。

   * 共有セグメント内のセグメント（医療など）をクリックすると、表示される人物は、表示中のワークスペースに関連付けられたパーティション内の人物のみになります。
      * Workspace 1 （WS1）でセグメント化を作成し、それをWS2と共有し、WS1がWS2のパーティションにアクセスできない場合、セグメント化は再計算されません。
      * パーティションが制限されたワークスペースでセグメント化を作成し、別のワークスペースで共有した場合、共有セグメントを受け取ったワークスペースには、重複したユーザのみが表示されます。

>[!NOTE]
>
>これらのルールのいくつかは複雑です。 特定の人を対象とした検査が推奨されます。 必要に応じて、新しいセグメントを作成したり、古いセグメントを削除したりできます。

## シナリオの例 {#example-scenarios}

![](assets/share-segmentations-across-workspaces-and-partitions-1.png)

![](assets/share-segmentations-across-workspaces-and-partitions-2.png)

## セグメントの共有 {#share-a-segmentation}

1. **[!UICONTROL データベース]**&#x200B;に移動します。

   ![](assets/share-segmentations-across-workspaces-and-partitions-3.png)

1. 「**[!UICONTROL セグメント化]**」を右クリックし、「**[!UICONTROL 新規フォルダー]**」を選択します。

   ![](assets/share-segmentations-across-workspaces-and-partitions-4.png)

1. ワークスペース間で共有するフォルダーに名前を付け（例：セグメントを共有）、**[!UICONTROL 作成]**&#x200B;をクリックします。

   ![](assets/share-segmentations-across-workspaces-and-partitions-5.png)

1. 共有するセグメントをフォルダーに移動します。

   ![](assets/share-segmentations-across-workspaces-and-partitions-6.png)

1. フォルダーを右クリックし、「**[!UICONTROL フォルダーを共有]**」を選択します。

   ![](assets/share-segmentations-across-workspaces-and-partitions-7.png)

1. フォルダーを共有するワークスペースを選択します。 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/share-segmentations-across-workspaces-and-partitions-8.png)

   >[!NOTE]
   >
   >このダイアログには、表示権限を持つワークスペースが表示されます。そのため、Marketo では、すべてのワークスペースとパーティションを表示できるデフォルトワークスペースからセグメント化を作成して共有することをお勧めします。

元のフォルダーは、他のワークスペースと共有されていることを示す矢印付きのデータベースツリーに表示されます。 共有ワークスペース内では、フォルダーはロック付きで表示され、そのフォルダーの内容が別のワークスペースから共有され、読み取り専用であることを示します。
