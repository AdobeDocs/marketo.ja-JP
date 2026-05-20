---
unique-page-id: 4719287
description: 最初のSalesforce同期の前に、最初のフィールドマッピングを編集する方法について説明します。 Marketoで、マッピングされていないカスタムフィールドをマッピングしたり、リードとコンタクトのフィールドの自動マッピングを解除したりできます。
title: 初期フィールドマッピングの編集
exl-id: 320613d1-3845-4e05-a704-0db0f8027dc8
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/wqBJIxz5JX1iHb-iE2NuhrbWcUypLEN3dndu36kJNXs
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 297
ht-degree: 60%

---

# 初期フィールドマッピングの編集 {#edit-initial-field-mappings}

>[!NOTE]
>
>この機能は、Salesforceに最初に同期する前にのみアクセスできます。 一度「**[!UICONTROL 今すぐ同期]**」ボタンが押されると、この操作は実行できなくなります。

Adobe Marketo Engageでは、Salesforceとの初回同期時に、同様の名前のカスタムフィールドをMarketo側の1つのフィールドに自動的に組み合わせ、CRMのリードオブジェクトと連絡先オブジェクトの両方とデータをやり取りできるようにしています。 この記事では、これらのマッピングをカスタマイズする方法について説明します。

## マッピングされていないフィールドをマッピング {#map-unmapped-fields}

「[!UICONTROL  マッピングされていないフィールド ]」フォルダーにフィールドが表示された場合、Salesforceのリードまたは取引先責任者の同様のフィールドにマッピングされていないことを意味します。 これは修正できます。

1. 「**[!UICONTROL マッピングを編集]**」をクリックします。

![](assets/image2014-12-9-13-3a31-3a0.png)

1. **[!UICONTROL マッピングされていないカスタムフィールド]**&#x200B;フォルダーを開きます。

   ![](assets/two.png)

1. マッピングされていないカスタムフィールドをドラッグして別のマッピングされていないカスタムフィールドに重ね、まとめます。

   >[!NOTE]
   >
   >編集できるのは、カスタムフィールドマッピングのみです。 標準フィールドマッピングは変更できません。

   ![](assets/three.png)

1. 完了したら「**[!UICONTROL マッピングを終了]**」をクリックします。

   ![](assets/four.png)

## 既存のマッピングを解除 {#break-existing-mapping}

リードと連絡先オブジェクトに似た名前のフィールドがある場合、Marketo はそれらを自動的にマッピングします。 異なるデータを保持し、異なるデータを持つと見なすこともできます。 このようにマッピングを解除します。

1. 「**[!UICONTROL マッピングを編集]**」をクリックします。

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. マッピングされたフィールドをハイライトし、「**[!UICONTROL マッピングを解除]**」をクリックしてフィールドを分けます。

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. 完了したら「**[!UICONTROL マッピングを終了]**」をクリックします。

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   初期同期はほぼ完了です。

## スキーマのリセット {#reset-schema}

1. マッピングの操作中に Salesforce のスキーマに変更を加えた場合は、「**[!UICONTROL スキーマをリセット]**」をクリックして変更を適用します。

   * すべてのマッピングの変更がリセットされます。
   * スキーマのリセットでは、フィールドの追加のみがおこなわれ、削除はおこなわれません（同期ユーザーから非表示にした場合でも）。

   ![](assets/image2014-12-9-13-3a32-3a8.png)
