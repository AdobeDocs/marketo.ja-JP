---
unique-page-id: 4718683
description: ステージの承認と収益モデルへのリードの割り当て - Marketo ドキュメント - 製品ドキュメント
title: ステージの承認と収益モデルへのリードの割り当て
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 100%

---

# ステージの承認と収益モデルへのリードの割り当て {#approving-stages-and-assigning-leads-to-a-revenue-model}

既存のリードを追加し、新しいリードの割り当てルールを作成して、**収益モデル**&#x200B;を稼働させます。

## 承認するステージ {#approving-stages}

リードを追加する前に、モデルのステージを承認してみましょう。

1. **分析**&#x200B;領域に移動します。

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. ステージを承認するモデルを選択します。

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. **モデルのアクション**&#x200B;で、「**ステージを承認**」を選択します。

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. 警告が表示されます。「**リードを割り当て**」をクリックします。

   ![](assets/image2015-4-28-17-3a5-3a39.png)

これで完了です。次に進み、それらのリードを割り当てましょう。

## 既存のリードの割り当て {#assigning-existing-leads}

「[スマートリストを作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)」をクリックして、リードデータベース内のモデルの 1 つのステージのリードを特定します。

1. [スマートリストを作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)したら、「**リード**」タブをクリックします。

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. 「**すべて選択**」をクリックしてリードを選択します。

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. **リードアクション**&#x200B;ドロップダウンを開いて、「**特別**」を選択します。「**収益ステージを変更**」をクリックします。

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. 正しい&#x200B;**モデル**&#x200B;と正しい&#x200B;**ステージ**&#x200B;を選択します。「**今すぐ実行**」をクリックします。

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. すべてのリードがモデルの様々なステージに割り当てられるまで繰り返します。

その調子です。新規リードをステージに割り当てる方法を指定するには、割り当てルールを作成します。

>[!NOTE]
>
>モデルが「承認済みステージ」の状態の場合、リードのアクティビティログに収益ステージの変更イベントは表示されません。モデルが完全に承認されている場合、現在の同じステージにリードを移動すると、このフローステップはスキップされます。

## 新規リード：割り当てルールの作成  {#new-leads-create-assignment-rules}

1. **Marketo ホーム**&#x200B;を再度クリックして、「**分析**」を選択します。

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. ツリーでモデルをクリックし、**モデルのアクション**&#x200B;メニューをクリックして、「**割り当てルール**」を選択します。

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. 割り当てルールに複数の既定の選択肢が含まれている場合は、「**ステージ**」をクリックして、選択をおこない、「**選択肢を追加**」をクリックします。

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## 割り当てルールの例 {#example-assignment-rule}

リードスコアルールを作成して、最小スコアの新規リードを適切な手順に割り当てます。

1. **If** で、「**リードスコア**」を選択します。次に、**at least** を選択します。

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. フィールドに「**40**」と入力し、**セールスリード**&#x200B;をステージとして使用します。「**保存**」をクリックして終了します。

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>モデルを承認するには、**[収益モデルの承認と承認取消](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**&#x200B;ヘルプページを参照してください。
