---
unique-page-id: 4718672
description: 売上高モデルトランジションの使用 — Marketto Docs — 製品ドキュメント
title: 売上高モデルトランジションの使用
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 0%

---


# 売上高モデルトランジションの使用 {#using-revenue-model-transitions}

>[!PREREQUISITES]
>
>[新しい売上高モデルの作成](create-a-new-revenue-model.md)

モデルを作成し、在庫ステージを選択して整理する場合は、トランジションを設定する時間です。

![](assets/one-2.png)

1. 開始する矢印の1つを右クリック(重複を押しながらクリック)し、「トランジションを **編集**」を選択します。

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >「匿名→既知」トランジションルールは編集できません。

1. 選択したトランジションに対して新しいタブが開きます。   ![](assets/three-1.png)
1. トランジションは、ステージ間のリードの移動方法を制御します。 選択したトリガー（またはフィルター）を右からドラッグし、カンバスの任意の場所に放します。 この例では、「Fills Out Form」トリガーを選択します。

   >[!TIP]
   >
   >売上高モデラーはレポートを設定しているので、トランジションにトリガーを常に含めることをお勧めします。 これにより、モデル/ステージフローの真の速度がレポートに反映されます。 フィルターは、トリガーを使用して追加の制約を適用して追加できます。

   ![](assets/four-2.png)

1. 選択したトリガー/フィルターのパラメーターを選択します。

   ![](assets/five-2.png)

1. モデルに戻るには、[ **モデラ**]をクリックします。

   ![](assets/six.png)

1. 画面の下部に、トランジションルールが表示されます。

   ![](assets/seven.png)

1. すべてのトランジションに対してルールを設定したら、「 **検証** 」をクリックして確認します。

   ![](assets/eight.png)

1. 正しく実行されると、次のメッセージが表示されます。

   ![](assets/nine.png)

よくやった！ モデルトランジションの変更が完了しました。

>[!NOTE]
>
>**関連記事**
>
>[売上高モデルの承認/未承認](approve-unapprove-a-revenue-model.md)
