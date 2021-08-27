---
unique-page-id: 4719308
description: 既存のSalesforceフィールドのMarketo Syncへの追加 — Marketoドキュメント — 製品ドキュメント
title: 既存のSalesforceフィールドのMarketo Syncへの追加
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 3%

---

# 既存のSalesforceフィールドのMarketo Syncへの追加 {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**管理者権限が必要です**

通常、Salesforceの新しいカスタムフィールドは、Marketoに自動的に同期されます。 そうでない場合、Marketo Syncのユーザーにはこれらのフィールドが表示されない場合があります。 これを修正する方法は次のとおりです。

1. 名前をクリックし、「**設定**」を選択します。

   ![](assets/image2015-6-30-14-3a20-3a6.png)

1. 左側の検索バーに&#x200B;**profile**&#x200B;と入力し、**Manage Users**&#x200B;の下の&#x200B;**Profiles**&#x200B;をクリックします。

   ![](assets/image2015-6-30-14-3a20-3a52.png)

1. ユーザーのプロファイルを同期をクリックします。

   ![](assets/image2015-6-30-14-3a23-3a41.png)

1. 「**フィールドレベルのセキュリティ**」セクションで、フィールドを含むオブジェクトの横にある「**表示**」をクリックします。

   ![](assets/image2015-6-30-14-3a23-3a59.png)

1. 「**編集**」をクリックします。

   ![](assets/image2015-6-30-14-3a24-3a28.png)

1. 同期に追加するフィールドの「**表示**」チェックボックスをオンにして、「**保存**」をクリックします。

   ![](assets/image2015-6-30-14-3a24-3a49.png)

   できましたね。次の同期サイクルで、Marketoがフィールドを表示し、マジックを開始します。

   >[!NOTE]
   >
   > Salesforceに既に値が含まれているフィールドの場合、次のレコードが更新されるまで、それらの値はMarketoに同期されません。
