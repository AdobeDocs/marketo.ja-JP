---
unique-page-id: 1147031
description: SFDCから人物を削除 —Marketoドキュメント — 製品ドキュメント
title: SFDC からの担当者の削除
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 5%

---

# SFDC からの担当者の削除 {#delete-person-from-sfdc}

Salesforceから特定のリードのセットを削除し、Marketoの担当者のままにする必要がある場合は、SFDCフローアクションの「個人を削除」を使用できます。

>[!NOTE]
>
>Salesforceと統合されている場合にのみ使用できます。

1. データベースで、Salesforceから削除するユーザーをクリックします。 次に、「**個人アクション**」をクリックし、「**Salesforce**」を選択します。

   ![](assets/person-actions-salesforce.png)

1. 「**SFDCから人物を削除**」を選択します。

   ![](assets/delete-person-from-sfdc.png)

1. 「Marketo **の**&#x200B;削除」設定が&#x200B;**false**&#x200B;になっていることを確認し、「**今すぐ実行**」をクリックします。

   ![](assets/run-action-delete-lead-from-sfdc.png)

   フローステップの実行後、担当者はSalesforceのリードではなくなり、Marketoに残ります。

   >[!CAUTION]
   >
   >Marketo **の**&#x200B;削除を&#x200B;**true**&#x200B;に設定し、Marketoの人々とSalesforceのリードを削除すると、それらは永遠に消え去ります。 これは元に戻せません。
