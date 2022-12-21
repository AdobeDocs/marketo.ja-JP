---
unique-page-id: 1147027
description: 個人を SFDC に同期する - Marketo ドキュメント - 製品ドキュメント
title: 個人を SFDC に同期する
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 100%

---

# 個人を SFDC に同期する {#sync-person-to-sfdc}

>[!NOTE]
>
>Salesforce との連携時にのみ有効です。

## 概要 {#overview}

このフローステップは、Marketo が作成した人物を Salesforce CRM に挿入するものです。

![](assets/sync-person-to-sfdc.png)

## 使用方法 {#usage}

1. デフォルトでは、このフローステップは、Salesforce 自動割り当てルールに基づいてリード所有者に割り当てます。

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >Salesforce では、人物の「会社」と「姓」のフィールドが入力されている必要があります。入力されていない場合、リードレコードは拒否されます。

1. 特定の Salesforce ユーザーまたはリードのキューをリード所有者として設定できます。

   ![](assets/sync-person-to-sfdc-2.png)

   このフローステップを使用する場合、人物は Salesforce のリードとして即座に同期され、通常の同期を待つ必要はありません。

   >[!CAUTION]
   >
   >Salesforce では「連絡先」をリードのキューに割り当てることはできません。この場合、Marketo は Salesforce で「リード」を重複して作成します。
