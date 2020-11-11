---
title: モデルの正常性とデータの有効性
description: モデルの正常性およびデータの有効性
translation-type: tm+mt
source-git-commit: cd1b7e65c73de0b31f20289402f1c0832c382b33
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---


# モデルの正常性およびデータの有効性

<br> 

モデルのパフォーマンスは、入力データの品質と完全性に依存します。 モデルの健康状態を評価する方法を次に示します。

Marketo Classicの [!UICONTROL **管理**] 領域にある「 [!UICONTROL **予測オーディエンス**] 」の下の「モデルとデータの正常性 [!UICONTROL ****] 」セクションに移動します。 すべてのモデルとそのステータスが表示されます。

![イメージ1](/help/sky/assets/predictive-audiences/model-health-and-data-validity/model-health-and-data-validity-1.png)

* **トレーニングステータス**:モデルが積極的にトレーニング（予測の改善）を行っているかどうかを示します。 トレーニングは2週間ごとに自動的に行われます。 「_処理」のモデルの完了には_ 、最大24時間かかる場合があります。 _失敗したモデルについては_ 、 [マーケティング担当者にお問い合わせください](https://nation.marketo.com/t5/Support/ct-p/Support)。
* **スコアリングステータス**:モデルがプログラムメンバーの予測（尤度の割合）を積極的に計算しているかどうかを示します。
* **パフォーマンス**：データの完全性とデータの質に基づくモデルの正常性の分類（以下を参照）。
* **データの完全性**:存在する/完了しているデータ属性の割合。
* **データの質**:良好で使いやすいデータを含む属性の割合。
