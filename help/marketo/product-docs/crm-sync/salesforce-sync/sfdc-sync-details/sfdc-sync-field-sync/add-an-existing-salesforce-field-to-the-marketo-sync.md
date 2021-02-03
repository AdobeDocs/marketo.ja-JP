---
unique-page-id: 4719308
description: Marketo Sync - Marketto Docs — 製品ドキュメントに追加対する既存のSalesforceフィールド
title: マーケティ追加ング担当者との同期に使用する既存のSalesforceフィールド
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# Marketo Sync &lt;a0追加/>に対する既存のSalesforceフィールド{#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**必要な管理者権限**

通常、Salesforceの新しいカスタムフィールドは、自動的にMarketoに同期されます。 そうでない場合は、Marketor Syncユーザーに対してこれらのフィールドが表示されない場合があります。 この問題を解決する方法を次に示します。

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

   甘い！ 次の同期サイクルで、Marketoはフィールドと開始に魔法を見せます。

   >[!NOTE]
   >
   > Salesforceにフィールドに既に値が含まれている場合、これらの値は、次のレコードが更新されるまで、Marketoに同期されません。
