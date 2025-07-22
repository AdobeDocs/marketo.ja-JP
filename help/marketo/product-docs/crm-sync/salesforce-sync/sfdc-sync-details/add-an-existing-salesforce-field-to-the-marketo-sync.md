---
unique-page-id: 4719308
description: 既存の Salesforce フィールドの Marketo  同期への追加 - Marketo ドキュメント - 製品ドキュメント
title: 既存の Salesforce フィールドの Marketo 同期への追加
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 66%

---

# Marketo Sync に既存の [!DNL Salesforce] フィールドを追加する {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**管理者権限が必要**

通常、Salesforceの新しいカスタムフィールドは、Marketo Engageに自動的に同期されます。 そうでない場合、Marketo 同期ユーザーにはフィールドが表示されない場合があります。この問題の修正方法を次に示します。

1. 名前をクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. 左側の検索バーに「プロファイル」と入力し、「ユーザーを管理 **[!UICONTROL の下の]** プロファイル **[!UICONTROL をクリック]** ます。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. 同期ユーザーのプロファイルをクリックします。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. **[!UICONTROL フィールドレベルのセキュリティ]**&#x200B;セクションで、フィールドを含むオブジェクトの横にある「**[!UICONTROL 表示]**」をクリックします。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. 「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. 同期に追加するフィールドの「**[!UICONTROL 表示]**」のチェックをオンにし、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   次の同期サイクルで、Marketo はフィールドを表示し、マジックを開めます。

   >[!NOTE]
   >
   > フィールドに既に [!DNL Salesforce] の値が含まれている場合、次のレコードが更新されるまでそれらの値はMarketoに同期されません。
