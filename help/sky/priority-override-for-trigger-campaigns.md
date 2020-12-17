---
title: priority-override-for-trigger-キャンペーン
description: トリガーキャンペーンの優先度の上書き
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---


# トリガーキャンペーンの優先度の上書き

<br> 

管理者は、ビジネス目標に適した優先順位を設定するためのトリガーキャンペーンに対して、Marketorの決定された優先順位を上書きできます。

>[!NOTE]
>
>この機能は、トリガーキャンペーンおよび「トリガーキャンペーンの優先度を編集」権限を付与されているユーザーに対してのみ使用できます。

>[!CAUTION]
>
>この機能は、限られたビジネスクリティカルなキャンペーンに対して使用することを強くお勧めします（25が推奨される最大数）。 大きなセットに対して軽く機能を使用すると、キャンペーン全体の実行に悪影響を及ぼす可能性があります。

## 優先順位を上書き

1. トリガーキャンペーンで、「**[!UICONTROL スケジュール]**」タブをクリックし、「**[!UICONTROL 優先順位を上書き]**」をクリックします。

   ![イメージ1](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-1.png)

1. ドロップダウンから新しい優先度レベルを選択します。 「**[!UICONTROL 確認]**」をクリックします。

   ![イメージ2](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-2.png)

   ![イメージ3](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-3.png)

>[!NOTE]
>
>* [!UICONTROL マーケティングアクティビティ]の下の[!UICONTROL キャンペーンキュー]で、キャンペーンのデフォルトの優先度を表示できます。 実行率を上げるには、キャンペーンの優先度をデフォルトより1レベル高く設定することをお勧めします。
>* ユーザーセットの優先順位は、キャンペーン資格を持つ新しい人にのみ適用されます。既にキューに登録されているユーザーは影響を受けません。


## 優先度をリセット

1. キャンペーンの優先度をシステムのデフォルトに戻すには、トリガーキャンペーンの&#x200B;**[!UICONTROL スケジュール]**&#x200B;タブに移動し、**[!UICONTROL 優先度をリセット]**&#x200B;をクリックします。

   ![画像4](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-4.png)

1. 「**[!UICONTROL リセット]**」をクリックして確認します。

   ![画像5](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-5.png)

>[!NOTE]
>
>優先度の上書きとリセットは、監査証跡に取り込まれます。 Classicエクスペリエンスの[!UICONTROL 管理者]領域を通じて、[監査証跡](https://docs.marketo.com/x/GZ2t)を表示できます。

## 優先順位上書きアクセスの許可

>[!CAUTION]
>
>管理者または管理責任を持つユーザーのみが、キャンペーンの優先順位の上書きアクセス権を持つ必要があります。

1. 「[!UICONTROL 管理者]」領域で、「**[!UICONTROL ユーザーとロール]**」をクリックします。

   ![画像6](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-6.png)

1. 「**[!UICONTROL ロール]**」タブをクリックし、アクセスを許可するユーザーを選択して、「**[!UICONTROL ロールを編集]**」をクリックします。

   ![画像7](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-7.png)

1. 「[!UICONTROL マーケティングアクティビティへのアクセス]」で、「**[!UICONTROL トリガーキャンペーンの優先度を編集]**」をオンにします。 「**[!UICONTROL 保存]**」をクリックします。

   ![画像8](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-8.png)

## Marketo Classicの表示キャンペーンの優先度

トリガーキャンペーン内の「**[!UICONTROL スケジュール]**」タブをクリックして、[!DNL Classic]エクスペリエンスの表示キャンペーンの優先度を設定できます。

![画像9](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-9.png)

>[!NOTE]
>
>[!DNL Classic]エクスペリエンスの優先順位は表示のみです。 キャンペーンの優先度の変更またはリセットは、Marketo Skyを通じてのみ行えます。
