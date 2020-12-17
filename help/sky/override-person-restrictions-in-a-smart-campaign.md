---
title: override-person-restrictions-in-a-smart-キャンペーン
description: スマートキャンペーンの個人制限の上書き
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# スマートキャンペーンの個人制限の上書き

<br> 

Marketorでは、スマートキャンペーンに振り分けられる最大人数を設定できます。これにより、データベース全体を誤って電子メールで送信するのを防ぐことができます。 この制限を上書きする場合は、次の方法を使用します。

>[!IMPORTANT]
>
>Marketor [!UICONTROL 管理者]のスマートキャンペーン](https://docs.marketo.com/display/DOCS/Enable+Person+Restrictions+for+Smart+Campaigns)に対する個人制限を必ず[有効にしてください。

1. スマートキャンペーンを探し、**[!UICONTROL スケジュール]**&#x200B;をクリックします。

   ![イメージ1](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-1.png)

1. 「**[!UICONTROL 資格ルール]**」をクリックします。

   ![イメージ2](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >デフォルトの制限は、管理で設定された制限です。

1. **[!UICONTROL 「Abort」キャンペーンの横に、条件を満たすリードが]**&#x200B;を超えた場合に、新しい制限を入力します。

   ![イメージ3](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-3.png)

>[!NOTE]
>
>資格を得た人の数が設定された制限を超えると、スマートキャンペーンは実行されません。

>[!CAUTION]
>
>誤って多くの人を含めすぎないように、この機能に注意してください。
