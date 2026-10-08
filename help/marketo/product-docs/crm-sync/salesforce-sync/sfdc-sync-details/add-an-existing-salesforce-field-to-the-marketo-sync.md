---
unique-page-id: 4719308
description: 既存のSalesforce フィールドをMarketoに追加する方法について説明します。 Salesforceの同期ユーザーが次のサイクルで同期するように、このフィールドを表示します。
title: 既存の Salesforce フィールドの Marketo 同期への追加​
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
TQID: 'https://experienceleague.adobe.com/Vb-1DhNwUPQSPYuCkVzzSDDqWd4tvO-XoPhXn58hj6E'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 83%
---
# 既存の [!DNL Salesforce] フィールドの Marketo 同期への追加 {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**管理者権限が必要**

通常、Salesforce の新しいカスタムフィールドは Marketo Engage に自動的に同期されます。 そうでない場合、Marketo 同期ユーザーにはフィールドが表示されない場合があります。 この問題の修正方法を次に示します。

1. 名前をクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. 左の検索バーで「プロファイル」と入力し、「**[!UICONTROL ユーザを管理]**」の下の「**[!UICONTROL プロファイル]**」をクリックします。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. 同期ユーザーのプロファイルをクリックします。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. **[!UICONTROL フィールドレベルのセキュリティ]**&#x200B;セクションで、フィールドを含むオブジェクトの横にある「**[!UICONTROL 表示]**」をクリックします。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. 「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. 同期に追加するフィールドの「**[!UICONTROL 表示]**」のチェックをオンにし、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   次の同期サイクルで、Marketo がそのフィールドを認識し、同期処理が開始されます。

   >[!NOTE]
   >
   > [!DNL Salesforce] でフィールドに既に値が含まれている場合、これらの値は次のレコードが更新されるまで Marketo に同期されません。
