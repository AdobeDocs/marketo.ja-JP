---
title: 理解バッチとトリガースマートキャンペーン
description: バッチおよびトリガースマートキャンペーンについて
exl-id: 54f38ecc-1b4c-4944-9f42-d8c1190c99d0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# バッチおよびトリガースマートキャンペーンについて

<br> 

スマートキャンペーンには2種類あります。バッチとトリガー。

## バッチスマートキャンペーン

バッチキャンペーンは、特定の時刻に起動し、特定の一連のユーザーにすべて同時に影響します。 例えば、カリフォルニアに住むデータベース内の全員に電子メールを送信する場合です。

バッチスマートキャンペーンは、スマートリストセクション内のフィルターのみを持ちます(トリガーは持ちません)。

![イメージ1](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-1.png)

「**[!UICONTROL スケジュール]**」タブをクリックすると、スマートキャンペーンが「バッチ」に設定されていることが確認されます。

![イメージ2](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-2.png)

**バッチスマートキャンペーン**

* 毎日、毎週、毎月など、繰り返しのスケジュールを設定できます。 1回だけ実行させることもできます。
* [プログラムスケジュール表示](https://docs.marketo.com/display/DOCS/Navigating+the+Program+Schedule+View)に表示されます。
* スマートキャンペーン内の「待機」ステップの後にある項目は、表示に含まれません。

## トリガースマートキャンペーン

トリガースマートキャンペーンは、トリガーされたイベントに基づいて、一度に1人の人に影響を与える。 トリガーの例としては、電子メール内のリンクをクリックします。

スマート・キャンペーンがスマート・リスト・セクション内で少なくとも1つのトリガーを使用する場合、モードは自動的にトリガーに設定されます。

![イメージ3](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-3.png)

「**[!UICONTROL スケジュール]**」タブをクリックすると、スマートキャンペーンが「トリガー」に設定されていることが確認されます。

![画像4](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-4.png)

**トリガースマートキャンペーン**

* 繰り返しのスケジュールは設定できません。 アクティブまたは非アクティブに設定することのみ可能です。
* 複数のトリガーを設定できます。 ただし、_いずれかの_&#x200B;トリガーが起動された場合は、キャンペーンアクションが実行されます。

>[!TIP]
>
>[アクティビティログ](https://docs.marketo.com/display/DOCS/Locate+the+Activity+Log+for+a+Person)を使用して、スマートキャンペーン内で何が順を追って発生したかを確認します。 アクティビティログは、ユーザーの詳細ページの最後のタブに表示されます。
