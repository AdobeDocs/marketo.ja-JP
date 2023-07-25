---
unique-page-id: 1147082
description: 人物の削除 - Marketo ドキュメント - 製品ドキュメント
title: 人物の削除
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 100%

---

# 人物の削除 {#delete-person}

誤った人物がデータベースに格納されることがあります。人物の削除フローステップで削除できます。

## 概要 {#overview}

スマートキャンペーンのフローステップを使用します。

![](assets/one-4.png)

>[!CAUTION]
>
>人物を削除すると、その人物の履歴 RCE データもすべて削除されます。これは元に戻せません。

## 使用方法 {#usage}

フローステップにドラッグすると、CRM からも自動的に削除されるように設定されます。

![](assets/two-4.png)

次のように、CRM ではなく Marketo から削除できます。

![](assets/three-3.png)

>[!NOTE]
>
>CRM からの人物の削除は、**Salesforce でのみ機能**&#x200B;します。人物を Marketo から削除し、Salesforce で保持することにした場合、Salesforce のレコードが更新された場合は、Marketo で再作成されます。
