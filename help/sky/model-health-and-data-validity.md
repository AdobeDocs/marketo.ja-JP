---
title: モデルの正常性とデータの有効性
description: モデルの正常性およびデータの有効性
exl-id: b14ec648-be1c-467b-b41d-2c53d74e25ea
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# モデルの正常性およびデータの有効性

<br> 

モデルのパフォーマンスは、入力データの品質と完全性に依存します。 モデルの健康状態を評価する方法を次に示します。

Marketo Classicの&#x200B;**[!UICONTROL 管理者]**&#x200B;の&#x200B;**[!UICONTROL 予測オーディエンス]**&#x200B;の下の&#x200B;**[!UICONTROL モデルとデータの正常性]**&#x200B;セクションに移動します。 すべてのモデルとそのステータスが表示されます。

![イメージ1](/help/sky/assets/predictive-audiences/model-health-and-data-validity/model-health-and-data-validity-1.png)

* **トレーニングステータス**:モデルが積極的にトレーニング（予測の改善）を行っているかどうかを示します。トレーニングは2週間ごとに自動的に行われます。 _処理_&#x200B;のモデルは、完了までに最大24時間かかる場合があります。 _失敗した_&#x200B;モデルについては、[Marketoサポート](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。
* **スコアリングステータス**:モデルがプログラムメンバーの予測（尤度の割合）を積極的に計算しているかどうかを示します。
* **パフォーマンス**：データの完全性とデータの質に基づくモデルの正常性の分類（以下を参照）。
* **データの完全性**:存在する/完了しているデータ属性の割合。
* **データの質**:良好で使いやすいデータを含む属性の割合。
