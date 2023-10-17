---
unique-page-id: 1147009
description: プログラムの成功を変更 - Marketo ドキュメント - 製品ドキュメント
title: プログラムの成功を変更
exl-id: 5b45b6d0-0c3d-4677-8b9a-8bbf03b1209e
feature: Smart Campaigns
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 100%

---

# プログラムの成功を変更 {#change-program-success}

## 概要 {#overview}

誤ってプログラムの成功とマークされたリードのグループが存在する場合、このフローステップを使用して、プログラムの成功の true/false を設定できます。

![](assets/image2014-9-22-14-3a45-3a8.png)

## 使用方法 {#usage}

1. このフローステップにドラッグしたプログラムは、編集中のスマートキャンペーンが含まれるプログラムに自動で設定されます。

   >[!NOTE]
   >
   >プログラムのメンバーのみに影響します。

   ![](assets/image2014-9-22-14-3a45-3a35.png)

1. 属性として「**[!UICONTROL 成功]**」か「**[!UICONTROL 成功日]**」を選択します。

   ![](assets/image2014-9-22-14-3a45-3a39.png)

   >[!NOTE]
   >
   >成功日に日付を設定すると、成功は自動的に「true」に設定されます。成功が「true」に設定されると、成功日は自動で現在の日付に設定されます。

1. 「**[!UICONTROL 新しい値]**」を **[!UICONTROL true]** か **[!UICONTROL false]** に設定します。

   ![](assets/image2014-9-22-14-3a45-3a55.png)

   >[!TIP]
   >
   >このフローステップを 2 回使用して、成功フラグならびに成功日の両方を設定することができます。

これで完了です。成功を解除・修正する方法を理解できました。
