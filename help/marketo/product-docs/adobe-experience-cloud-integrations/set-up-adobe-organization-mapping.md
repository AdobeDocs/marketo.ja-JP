---
unique-page-id: 42762511
description: Audience Managerおよびその他のAdobe アプリと同期するように、Marketo EngageでAdobe組織マッピングを設定する方法について説明します。
title: アドビ組織マッピングの設定
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
feature: Integrations
TQID: https://experienceleague.adobe.com/8Pypw9omyxldMxJqHj-KHBRzl-P5ttDhujCwcEVfLwQ
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
subfeature_v2: id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 247
ht-degree: 71%

---

# アドビ組織マッピングの設定 {#set-up-adobe-organization-mapping}

Audience Manager、B2B CDP Marketo コネクタ、[!DNL Dynamic Chat]などのアドビアプリケーションと同期するには、まず Marketo Engage で Adobe IMS 組織の資格情報を入力する必要があります。

>[!NOTE]
>
>* Marketo インスタンスの HIPAA 対応デプロイメントでは、この統合を使用できません。
>* 統合が機能するには、Marketo と他のアドビアプリケーションが同じ組織内に存在する必要があります。

>[!IMPORTANT]
>
>Adobe Business Platform と Identity Management システムにオンボードされているユーザの場合、サブスクリプションに関連付けられた組織 ID は既に入力されており、読み取り専用フィールドになっています。 そのため、この記事の手順は当てはまりません。

1. Marketo で、「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. 統合で、「**[!UICONTROL アドビ組織マッピング]**」をクリックします。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. 「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. [Adobe IMS組織ID](https://experienceleague.adobe.com/docs/control-panel/using/faq.html){target="_blank"}）を入力し、**[!UICONTROL OK]**&#x200B;をクリックします。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. 「**[!UICONTROL 確認]**」をクリックします。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. 「**[!UICONTROL 閉じる]**」をクリックします。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >セキュリティ上の理由から、マッピング先のアドビ組織の組織管理者である必要があります。 そうでない場合、アクションは失敗します。 また、アドビユーザと Marketo ユーザは、ログイン時に同じメールアドレスを使用する必要があります。

1. _まだ_&#x200B;にログインしていない場合、新しいタブまたはウィンドウにポップアップが表示されます。 アドビ組織にログインします（このアクションで組織アクセスが検証されます）。

Adobe Experience Cloudから[ オーディエンスデータを](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target="_blank"}様と共有したり、[ オーディエンスを同期](/help/marketo/product-docs/adobe-experience-cloud-integrations/sync-an-audience-from-adobe-experience-cloud.md){target="_blank"}したりできるようになりました。
