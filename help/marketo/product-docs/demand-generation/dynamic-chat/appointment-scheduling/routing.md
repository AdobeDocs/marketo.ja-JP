---
description: ルーティング — Marketoドキュメント — 製品ドキュメント
title: ルーティング
hide: true
hidefromtoc: true
source-git-commit: 0ca537b46247eef1e7200180d7c1516465910dac
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 1%

---

# ルーティング {#routing}

Dynamic Chat で予約された会議は、2 つの方法でルーティングできます。 ラウンドロビン、またはカスタムルールを使用します。

ラウンドロビン：ミーティングはエージェントに順次割り当てられます。 エージェントが 5 人、エージェントが 3 人で最後の会議を取った場合、エージェント 4 が次のミーティングを取得し、次にエージェント 5 が取得され、次にエージェント 1 に戻ります。

カスタムルール：選択した属性に基づいて、特定のエージェントを選択してミーティングを受け取ることができます。

## カスタムルールの作成 {#create-a-custom-rule}

この例では、CA、OR、WA の推測される状態から John のエージェントにすべてのミーティングを送信しています。

1. Dynamic Chat で、 **ルーティング**.

   ![](assets/routing-1.png)

1. 次をクリック： **カスタムルール** タブをクリックします。

   ![](assets/routing-2.png)

1. クリック **ルールを作成**.

   ![](assets/routing-3.png)

1. ルールに名前を付け、「 **次へ**.

   ![](assets/routing-4.png)

1. 目的のエージェントを選択します。

   ![](assets/routing-5.png)

1. 目的の属性の上にドラッグします。

   ![](assets/routing-6.png)

1. 目的の値を見つけて選択します。

   ![](assets/routing-7.png)

1. 目的の値をすべて選択したら、 **保存**.

   ![](assets/routing-8.png)
