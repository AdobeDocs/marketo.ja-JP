---
description: Adobe Experience CloudからMarketo Engageにオーディエンスを同期する方法について説明します。 オーディエンスライブラリからオーディエンスをMarketoデータベースに取り込み、キャンペーンやプログラムで使用できます。
title: Adobe Experience Cloud からのオーディエンスの同期
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
feature: Integrations
TQID: https://experienceleague.adobe.com/XCskpUNcNae-ikOLXxREb4kePbFs9HRheIihzJqHKoU
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: c5f60233-d5ea-4453-a799-0ad258b4d399id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 294
ht-degree: 52%

---

# Adobe Experience Cloud からのオーディエンスの同期 {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Marketo インスタンスの HIPAA 対応デプロイメントでは、この統合を使用できません。

>[!PREREQUISITES]
>
>[アドビ組織マッピングの設定](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## オーディエンスの同期方法 {#how-to-sync-an-audience}

1. My Marketo で、「**[!UICONTROL データベース]**」タイルをクリックします。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. 「**[!UICONTROL 新規]**」ドロップダウンをクリックして、「**[!UICONTROL Experience Cloud オーディエンスから同期]**」を選択します。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. 「**[!UICONTROL オーディエンスライブラリフォルダー]**」ドロップダウンリストをクリックして、目的の元フォルダーを選択します。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. **[!UICONTROL オーディエンス名]**&#x200B;を選択します。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. 宛先については、既存のリストを選択するか、新しいリストの名前を入力できます。 この例では、新しいリストが作成されています。 終了したら「**[!UICONTROL 同期]**」をクリックします。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. 「**[!UICONTROL OK]**」をクリックします。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## よくある質問 {#faq}

**Cookie の同期は、どのよう仕組みなのですか？**

Marketo サブスクリプションでcookie syncが有効になっている場合、Marketoのmunchkin.jsは、統合の設定中に指定したAdobe IMS組織のAdobe ECIDを取得して保存し、これらのECIDを対応するMarketo Cookie IDと照合しようとします。 これにより、Marketo の匿名ユーザプロファイルを Adobe ECID で強化できます。

匿名ユーザープロファイルをリードプロファイルに関連付けるには、さらに手順が必要です。このプロファイルは、プレーンテキストメールを使用して識別されます。 この機能の正確な仕組みは、[こちらで説明しています](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"}。

**Marketo のリストサイズがアドビのリストサイズと異なるのはなぜですか？**

また、ECID Cookie IDをMarketoの既知のユーザーに関連付けられない場合、ユーザーは同期しません。

**これは 1 回限りの同期ですか？**

同期を開始する必要があるのは 1 回だけです。 その後、レコードは自動的に同期されます。 最初の同期には最大24時間かかります。今後、新しいレコードは2～3時間で同期されます。
