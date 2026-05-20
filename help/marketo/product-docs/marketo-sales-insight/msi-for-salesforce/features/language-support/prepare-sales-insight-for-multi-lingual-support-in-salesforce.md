---
unique-page-id: 7516460
description: Salesforceの多言語サポート用にMarketo Sales Insightを準備する方法について説明します。 グローバルユーザーの言語とロケールを設定します。
title: Salesforce での多言語サポートに向けたセールスインサイトの準備
exl-id: b808fa91-accd-4e0c-8223-0717faccab10
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/OyeA8IbYicPJp56c6epuyFqr619J8sMQA4hmT--kry8
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 240
ht-degree: 91%

---

# Salesforce での多言語サポートに向けたセールスインサイトの準備 {#prepare-sales-insight-for-multi-lingual-support-in-salesforce}

>[!NOTE]
>
>**管理者権限が必要**

Marketo セールスインサイトは言語別に格納されます。 したがって、複数の言語を扱う場合は、言語ごとに別個に資格情報を入力する必要があります。

>[!NOTE]
>
>[!DNL Sales Insight] は現在、次をサポートしています。
>
>* 英語
>* フランス語
>* ドイツ語
>
>それ以外の言語は、デフォルトで英語に設定されます。

## [!DNL Marketo Sales Insight] 用の新しい言語の追加 {#adding-a-new-language-for-marketo-sales-insight}

1. [!DNL Salesforce] にログインします。 右上隅の名前のドロップダウンで、「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/image2015-7-6-16-3a5-3a6.png)

1. 「**[!UICONTROL マイ個人情報]**」で、「**[!UICONTROL 個人情報]**」をクリックします。

   ![](assets/image2015-7-6-16-3a5-3a25.png)

1. 「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-7-6-16-3a5-3a38.png)

1. 言語を選択し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-7-6-16-3a5-3a47.png)

1. これで、[!DNL Salesforce] インターフェイスが選択した言語に変わります。 「**+**」アイコンをクリックすると、使用可能なタブがすべて表示されます。

   ![](assets/image2015-7-6-16-3a6-3a10.png)

1. 「**[!UICONTROL Marketo セールスインサイト]**&#x200B;設定」をクリックします（選択した言語で）。

   ![](assets/image2015-7-6-16-3a7-3a15.png)

1. Marketo に移動します。 [[!DNL Marketo Sales Insight] **[!UICONTROL &#x200B; API 設定&#x200B;]**&#x200B;の詳細](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md#configure-marketo-sales-insight)を見つけます。

   ![](assets/image2015-7-6-16-3a41-3a2.png)

1. Marketo から API の詳細を入力し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-7-6-16-3a7-3a43.png)

## [!DNL Salesforce] を英語に戻す {#change-salesforce-back-to-english}

[!DNL Salesforce] 組織のカスタマイズが完了したら、次の手順で個人設定を英語に戻します。

>[!NOTE]
>
>次のスクリーンショットは、英語の説明を含むフランス語版です。  前の手順で選択した言語のテキストと同じ画面が表示されます。

1. 自分の名前で、「**[!UICONTROL 設定]**」をクリックします。

![](assets/image2015-7-6-16-3a5-3a6.png)

1. 「**[!UICONTROL マイ個人情報]**」の「**[!UICONTROL 個人情報]**」をクリックします。

   ![](assets/image2015-7-6-16-3a8-3a3.png)

1. 「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2015-7-6-16-3a8-3a19.png)

1. 「言語」ドロップダウンから「**[!UICONTROL 英語]**」を選択し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-7-6-16-3a8-3a31.png)

   これで、[!DNL Salesforce] が英語に戻りました。
