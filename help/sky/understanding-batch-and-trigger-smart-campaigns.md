---
title: understanding-batch-and-trigger-smart-キャンペーン
description: バッチとトリガースマート・キャンペーンの理解
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# バッチとトリガースマート・キャンペーンの理解

<br> 

スマートキャンペーンには2種類あります。バッチとトリガーを参照してください。

## バッチスマートキャンペーン

バッチキャンペーンは、特定の時刻に起動し、特定の一連のユーザーにすべて同時に影響します。 例えば、カリフォルニアに住むデータベース内の全員に電子メールを送信する場合です。

バッチスマートキャンペーンは、スマートリストセクション内のフィルターのみを持ちます（つまり、トリガーは持ちません）。

![イメージ1](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-1.png)

「**[!UICONTROL スケジュール]**」タブをクリックすると、スマートキャンペーンが「バッチ」に設定されていることが確認されます。

![イメージ2](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-2.png)

**バッチスマートキャンペーン**

* 毎日、毎週、毎月など、繰り返しのスケジュールを設定できます。 1回だけ実行させることもできます。
* [プログラムスケジュール表示](https://docs.marketo.com/display/DOCS/Navigating+the+Program+Schedule+View)に表示されます。
* スマートキャンペーン内の「待機」ステップの後にある項目は、表示に含まれません。

## スマートキャンペーンのトリガー

トリガースマートキャンペーンは、トリガーされたイベントに基づいて、一度に1人の人に影響を与える。 トリガーの例としては、電子メール内のリンクをクリックします。

スマート・キャンペーンがスマート・リスト・セクション内で少なくとも1つのトリガを使用する場合、モードは自動的にトリガに設定されます。

![イメージ3](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-3.png)

「**[!UICONTROL スケジュール]**」タブをクリックすると、スマートキャンペーンが「トリガー」に設定されていることが確認されます。

![画像4](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-4.png)

**スマートキャンペーンのトリガー**

* 繰り返しのスケジュールは設定できません。 アクティブまたは非アクティブに設定することのみ可能です。
* 複数のトリガーを設定できます。 ただし、_任意の_&#x200B;トリガが起動された場合、キャンペーンアクションが実行されます。

>[!TIP]
>
>[アクティビティログ](https://docs.marketo.com/display/DOCS/Locate+the+Activity+Log+for+a+Person)を使用して、スマートキャンペーン内で何が順を追って発生したかを確認します。 アクティビティログは、ユーザーの詳細ページの最後のタブに表示されます。
