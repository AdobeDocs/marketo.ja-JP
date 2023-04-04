---
unique-page-id: 7515767
description: ワークスペースとパーティションをまたいだセグメント化の共有 - Marketo ドキュメント - 製品ドキュメント
title: ワークスペースとパーティションをまたいだセグメント化の共有
exl-id: b50f4328-fdba-4e39-bc0d-75bade1f9cbc
source-git-commit: 686530e63cffef89bc7b9cbf6affa862689c0a46
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# ワークスペースとパーティションをまたいだセグメント化の共有 {#share-segmentations-across-workspaces-and-partitions}

>[!PREREQUISITES]
>
>この記事は、ワークスペースとパーティションをお使いのお客様専用です。

## セグメントとは {#whats-a-segmentation}

Marketo は、プログラムやスマートキャンペーンに適した人物を選ぶのが得意です。ただし、より永続的なペルソナの場合は、セグメント化を使用する必要があります。セグメント化は、Marketo で高度な動的コンテンツを使用するために必要です。

>[!NOTE]
>
>[セグメント化の作成方法](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)を参照してください。

これらのペルソナを設定したら（_および_&#x200B;ワークスペースを使用している場合）、ワークスペース全体で共有します。次に、知っておくといい点を示します。

## ルールとヒント {#rules-tips}

* 各 Marketo サブスクリプションには、複数のワークスペースをまたいで最大 20 個のセグメントを「合計」で含めることができます（**1 ワークスペースあたり 20 ではありません**）。
* セグメント化は、アクセス権のあるワークスペースとのみ共有できます。
* **すべてのパーティションを表示するデフォルトのワークスペース**&#x200B;を作成して使用するようにしてください。

* セグメント化処理は、セグメント化が作成されたワークスペース内の人物に対してのみ実行されます。

   * デフォルトのワークスペース内で共有するセグメントを作成します。
      * セグメント化の承認
      * 共有ワークスペースにはロックされたフォルダーが表示され、セグメント化は読み取り専用です。
      * 共有バージョンは編集できません。元のセグメントを作成した場所でのみ編集できます。
   * 共有セグメント内のセグメント（医療など）をクリックすると、表示される人物は、表示中のワークスペースに関連付けられたパーティション内の人物のみになります。
      * Workspace 1 (WS1) でセグメント化を作成し、WS2 と共有した場合、WS2 のパーティションに WS1 がアクセスできない場合は、セグメント化は再計算されません。
      * パーティションが制限されたワークスペースでセグメント化を作成し、別のワークスペースで共有した場合、共有セグメントを受け取ったワークスペースには、重複したユーザーのみが表示されます。


>[!NOTE]
>
>いくつかのルールは少し複雑です。最も手早く使い始めるには、特定の人物を使用してテストすることです。新しいセグメント化の作成と、古いセグメントの削除はいつでも行えます。

## シナリオの例 {#example-scenarios}

![](assets/share-segmentations-across-workspaces-and-partitions-1.png)

![](assets/share-segmentations-across-workspaces-and-partitions-2.png)

## セグメントの共有 {#share-a-segmentation}

1. 「**データベース**」に移動します。

   ![](assets/share-segmentations-across-workspaces-and-partitions-3.png)

1. 右クリック **セグメント化** を選択し、 **新規フォルダ**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-4.png)

1. 複数のワークスペースで共有するフォルダーに名前を付けます ( 例：セグメントを共有を参照 )、「 **作成**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-5.png)

1. 共有するセグメントをフォルダーに移動します。

   ![](assets/share-segmentations-across-workspaces-and-partitions-6.png)

1. フォルダーを右クリックし、「**フォルダーを共有**」を選択します。

   ![](assets/share-segmentations-across-workspaces-and-partitions-7.png)

1. フォルダーを共有するワークスペースを選択します。「**保存**」をクリックします。

   ![](assets/share-segmentations-across-workspaces-and-partitions-8.png)

   >[!NOTE]
   >
   >このダイアログには、表示権限を持つワークスペースが表示されます。そのため、Marketo では、すべてのワークスペースとパーティションを表示できるデフォルトワークスペースからセグメント化を作成して共有することをお勧めします。

元のフォルダーは、他のワークスペースと共有されていることを示す矢印付きのデータベースツリーに表示されます。共有ワークスペース内では、フォルダーはロック付きで表示され、そのフォルダーの内容が別のワークスペースから共有され、読み取り専用であることを示します。
