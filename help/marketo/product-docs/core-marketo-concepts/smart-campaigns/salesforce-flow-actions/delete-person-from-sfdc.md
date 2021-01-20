---
unique-page-id: 1147031
description: SFDCから人物を削除 — マーケティング担当者ドキュメント — 製品ドキュメント
title: SFDCから人物を削除
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---


# SFDCから人物を削除{#delete-person-from-sfdc}

Salesforceから特定のリードのセットを削除し、Marketoの担当者のままにする必要がある場合は、SFDCフローアクションの「個人を削除」を使用できます。

>[!NOTE]
>
>Salesforceと統合されている場合にのみ使用できます。

1. データベースで、Salesforceから削除するユーザーをクリックします。 次に、「**個人アクション**」をクリックし、「**Salesforce**」を選択します。

   ![](assets/person-actions-salesforce.png)

1. 「**SFDCから人物を削除**」を選択します。

   ![](assets/delete-person-from-sfdc.png)

1. 「Marketor **の**&#x200B;削除」設定が&#x200B;**false**&#x200B;であることを確認し、「**今すぐ実行**」をクリックします。

   ![](assets/run-action-delete-lead-from-sfdc.png)

   フローステップの実行後、担当者はSalesforceのリードではなくなり、Marketoに残ります。

   >[!CAUTION]
   >
   >Marketor **の** Deleteを&#x200B;**true**&#x200B;に設定し、Marketoからの訪問者およびSalesforceからのリードを削除した場合、それらの訪問者は永久に消え去ります。 これは元に戻せません。
