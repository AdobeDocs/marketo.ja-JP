---
unique-page-id: 4719306
description: Marketo SyncでSalesforceフィールドを非表示にする — Marketoドキュメント — 製品ドキュメント
title: Marketo Syncに対するSalesforceフィールドの非表示
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 5%

---

# Marketo Syncに対するSalesforceフィールドの非表示 {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**管理者権限が必要です**

Salesforceのすべてのフィールドがマーケティングに役立つとは限りません。 必要なフィールドのみを含めることで、同期のパフォーマンスを最適化できます。 次に、フィールドをMarketoから非表示にする方法を示します。

1. 名前メニューをクリックし、「**設定**」を選択します。

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. 検索バーに&#x200B;**プロファイル**&#x200B;と入力し、**ユーザーの管理**&#x200B;の下の&#x200B;**プロファイル**&#x200B;をクリックします。

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. ユーザーのプロファイルを同期をクリックします。

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. 「**フィールドレベルのセキュリティ**」セクションで、ターゲットフィールドを含むオブジェクトの横にある「**表示**」をクリックします。

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. 「**編集**」をクリックします。

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. 非表示にするフィールドの横にある「**表示**」チェックボックスをオフにします。 「**保存**」をクリックします。

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Salesforceで非表示にしたフィールドが既にMarketoと同期されている場合は、Marketoでも非表示にする必要があります。

   これで完了です。次の同期が完了すると、Marketoでこのフィールドは表示されなくなります。

   >[!MORELIKETHIS]
   >
   >[フィールドの表示/非表示](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md)
