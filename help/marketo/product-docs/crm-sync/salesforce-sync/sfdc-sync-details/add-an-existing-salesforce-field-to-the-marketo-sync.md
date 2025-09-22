---
unique-page-id: 4719308
description: 既存の Salesforce フィールドの Marketo  同期への追加 - Marketo ドキュメント - 製品ドキュメント
title: 既存の Salesforce フィールドの Marketo 同期への追加
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 100%

---

# 既存の [!DNL Salesforce] フィールドの Marketo 同期への追加 {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**管理者権限が必要**

通常、Salesforce の新しいカスタムフィールドは Marketo Engage に自動的に同期されます。そうでない場合、Marketo 同期ユーザーにはフィールドが表示されない場合があります。この問題の修正方法を次に示します。

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

   次の同期サイクルで、Marketo はフィールドを表示し、マジックを開きます。

   >[!NOTE]
   >
   > [!DNL Salesforce] でフィールドに既に値が含まれている場合、これらの値は次のレコードが更新されるまで Marketo に同期されません。
