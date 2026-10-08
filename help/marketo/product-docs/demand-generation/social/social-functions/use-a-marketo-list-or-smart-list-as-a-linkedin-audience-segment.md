---
unique-page-id: 7504180
description: Marketo リストまたはスマートリストをLinkedIn オーディエンスセグメントとして使用する方法について説明します。 LinkedInにリストを送り、Ad Bridgeを通じて広告のターゲティングを行います。
title: Marketo のリストまたはスマートリストを LinkedIn のオーディエンスセグメントとして使用する
exl-id: 9a7943fe-b2e7-443a-87e0-da01001682de
feature: Social
TQID: 'https://experienceleague.adobe.com/n7Z4AKx6Hiu6f9cxXPpfSTJJdOLakTwy7ejQ-6LK4Bo'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: e9b7b90f-6f8a-4637-a2ca-00239808918c
    internal-label: Social
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 80%
---
# LinkedIn のオーディエンスセグメントとしての Marketo リストまたはスマートリストの使用 {#use-a-marketo-list-or-smart-list-as-a-linkedin-audience-segment}

Marketo Engage の人物を LinkedIn のオーディエンスと統合します。

>[!PREREQUISITES]
>
>[LinkedIn と一致したオーディエンスを LaunchPoint サービスとして追加](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}

1. **[!UICONTROL データベース]**&#x200B;に移動します。

   ![](assets/list-as-a-linkedin-audience-segment-1.png)

1. スマートリストを選択します。

   ![](assets/list-as-a-linkedin-audience-segment-2.png)

1. 「**[!UICONTROL リード]**」タブをクリックします。

   ![](assets/list-as-a-linkedin-audience-segment-3.png)

1. リストの下部にある **[!UICONTROL Ad Bridge 経由で送信]**&#x200B;アイコン![—](assets/icon-ad-bridge.png)をクリックします。

   ![](assets/list-as-a-linkedin-audience-segment-4.png)

   >[!NOTE]
   >
   >広告ネットワーク統合を使用してオーディエンスを LinkedIn に送信する場合、Marketo はメールアドレスのみを送信します。

1. 「**[!UICONTROL LinkedIn]**」を選択し、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/list-as-a-linkedin-audience-segment-5.png)

1. **[!UICONTROL LinkedIn オーディエンス]**&#x200B;を選択します。

   >[!NOTE]
   >
   >「**[!UICONTROL +新規オーディエンス]**」をクリックすると、LinkedIn Campaign Manager でオーディエンスが作成されます。

   ![](assets/list-as-a-linkedin-audience-segment-6.png)

   >[!NOTE]
   >
   >LinkedIn は、2018年3月に「オーディエンスの消去とリードの追加」プッシュタイプに使用される API を非推奨（廃止予定）にしました。 このオプションは、Marketo の 2018 年第 1 四半期リリース以降は使用できなくなりました。

1. **[!UICONTROL プッシュタイプ]**&#x200B;を選択します。 「**[!UICONTROL 更新]**」をクリックします。

   ![](assets/list-as-a-linkedin-audience-segment-7.png)

   >[!NOTE]
   >
   >同期が完了するまでに15分かかります。

これで、データはLinkedInのオーディエンスと同期されます。 アカウントおよび連絡先のターゲティング用に LinkedIn にリストをアップロードする方法については、[LinkedIn Marketing Solutions ヘルプセンター](https://www.linkedin.com/help/lms/answer/73938?query=ad%20segment){target="_blank"}にアクセスしてください。
