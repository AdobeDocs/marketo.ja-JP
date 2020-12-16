---
unique-page-id: 1147031
description: SFDCから人物を削除 — マーケティング担当者ドキュメント — 製品ドキュメント
title: SFDCから人物を削除
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---


# SFDCから人物を削除 {#delete-person-from-sfdc}

Salesforceから特定のリードのセットを削除し、Marketoの担当者のままにする必要がある場合は、SFDCフローアクションの「個人を削除」を使用できます。

>[!NOTE]
>
>Salesforceと統合されている場合にのみ使用できます。

1. データベースで、Salesforceから削除するユーザーをクリックします。 次に、「 **個人アクション** 」をクリックし、「 **Salesforce**」を選択します。

   ![](assets/person-actions-salesforce.png)

1. 「 **Delete Person from SFDC**」を選択します。

   ![](assets/delete-person-from-sfdc.png)

1. 「マーケティング先の **削除** 」設定が **falseに設定されていることを確認し、「今すぐ**&#x200B;実行 ****」をクリックします。

   ![](assets/run-action-delete-lead-from-sfdc.png)

   フローステップの実行後、担当者はSalesforceのリードではなくなり、Marketoに残ります。

   >[!CAUTION]
   >
   >Marketorの **削除を** trueに設定し **** 、Marketoからの訪問者およびSalesforceからのリードを削除すると、訪問者は永久に削除されます。 これは元に戻せません。

