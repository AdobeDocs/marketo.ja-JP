---
unique-page-id: 4719308
description: Marketo同期 —追加Marketoドキュメント — 製品ドキュメントの既存のSalesforceフィールド
title: Marketo同期追加の既存のSalesforceフィールド
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# 追加Marketo同期{#add-an-existing-salesforce-field-to-the-marketo-sync}に対する既存のSalesforceフィールド

>[!NOTE]
>
>**必要な管理者権限**

通常、Salesforceの新しいカスタムフィールドは、自動的にMarketoに同期されます。 そうでない場合は、これらのフィールドはMarketo同期ユーザーに表示されない場合があります。 この問題を解決する方法を次に示します。

1. 名前をクリックし、**セットアップ**&#x200B;を選択します。

   ![](assets/image2015-6-30-14-3a20-3a6.png)

1. 左の検索バーに&#x200B;**プロファイル**&#x200B;と入力し、「**ユーザーを管理**」の下の「**プロファイル**」をクリックします。

   ![](assets/image2015-6-30-14-3a20-3a52.png)

1. 同期ユーザーのプロファイルをクリックします。

   ![](assets/image2015-6-30-14-3a23-3a41.png)

1. 「**フィールドレベルのセキュリティ**」セクションで、フィールドを含むオブジェクトの横にある「**表示**」をクリックします。

   ![](assets/image2015-6-30-14-3a23-3a59.png)

1. 「**編集**」をクリックします。

   ![](assets/image2015-6-30-14-3a24-3a28.png)

1. 同期に追加するフィールドの「**表示**」チェックボックスをオンにし、「**保存**」をクリックします。

   ![](assets/image2015-6-30-14-3a24-3a49.png)

   甘い！ 次の同期サイクルで、Marketoはフィールドと開始に魔法を見る。

   >[!NOTE]
   >
   > Salesforceにフィールドに既に値が含まれている場合、これらの値は、次のレコードが更新されるまでMarketoに同期されません。
