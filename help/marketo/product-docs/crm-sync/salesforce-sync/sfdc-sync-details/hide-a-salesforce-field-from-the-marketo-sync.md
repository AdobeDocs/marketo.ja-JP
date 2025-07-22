---
unique-page-id: 4719306
description: Marketo 同期に対する Salesforce フィールドの非表示 — Marketo ドキュメント — 製品ドキュメント
title: Marketo 同期に対する Salesforce フィールドの非表示
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 66%

---

# Marketo同期から [!DNL Salesforce] フィールドを非表示にする {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**管理者権限が必要**

Salesforce のすべてのフィールドがマーケティングに役立つわけではありません。必要なフィールドのみを含めることで、同期のパフォーマンスを最適化できます。Marketo Engageでフィールドを非表示にする方法を以下に示します。

1. 名前メニューをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. 検索バーに「プロファイル」と入力し、「ユーザーを管理 **[!UICONTROL の下の]** プロファイル **[!UICONTROL をクリック]** ます。

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. 同期ユーザーのプロファイルをクリックします。

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. **[!UICONTROL フィールドレベルのセキュリティ]**&#x200B;セクションで、ターゲットフィールドを含むオブジェクトの横にある「**[!UICONTROL 表示]**」をクリックします。

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. 「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. 非表示にするフィールドの横にある「**[!UICONTROL 表示]**」のチェックをオフにします。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >[!DNL Salesforce] で非表示にするフィールドが既にMarketoと同期されている場合、それを使用しないようにするには、Marketoでも非表示にする必要があります。

   これで完了です。次の同期が完了すると、Marketo ではこのフィールドは表示されなくなります。

   >[!MORELIKETHIS]
   >
   >[フィールドの表示／非表示](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md){target="_blank"}
