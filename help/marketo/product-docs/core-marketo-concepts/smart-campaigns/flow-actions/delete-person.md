---
unique-page-id: 1147082
description: 人物の削除 - Marketo ドキュメント - 製品ドキュメント
title: 人物の削除
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '123'
ht-degree: 56%

---

# 人物の削除 {#delete-person}

誤ったユーザーがデータベースに入り込むことがあります。 人物の削除フローステップで削除できます。

## 概要 {#overview}

スマートキャンペーンのフローステップを使用します。

![](assets/one-4.png)

>[!CAUTION]
>
>人物を削除すると、その人物の履歴 RCE データもすべて削除されます。これは元に戻せません。

## 使用方法 {#usage}

フローステップにドラッグすると、CRM からも自動的に削除されるように設定されます。

![](assets/two-4.png)

次のように、CRM ではなくMarketo Engageからを削除できます。

![](assets/three-3.png)

>[!NOTE]
>
>CRM からの人物の削除は、_でのみ機能[!DNL Salesforce]_&#x200B;します。Marketoから人物を削除し、その人物を保持することを選択した場合 [!DNL Salesforce]を呼び出した場合、それらのイベントはMarketoに再作成されます ( [!DNL Salesforce] レコードが更新される前に
