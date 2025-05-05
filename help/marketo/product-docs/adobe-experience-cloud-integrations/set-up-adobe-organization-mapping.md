---
unique-page-id: 42762511
description: アドビ組織マッピングの設定 - Marketo ドキュメント - 製品ドキュメント
title: アドビ組織マッピングの設定
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
feature: Integrations
source-git-commit: 5ef17e8c3988706a4d95332312ffb035f35bb269
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 93%

---

# アドビ組織マッピングの設定 {#set-up-adobe-organization-mapping}

Audience Manager、B2B CDP Marketo コネクタ、[!DNL Dynamic Chat]などのアドビアプリケーションと同期するには、まず Marketo Engage で Adobe IMS 組織の資格情報を入力する必要があります。

>[!NOTE]
>
>* Marketo インスタンスの HIPAA 対応デプロイメントでは、この統合を使用できません。
>* 統合が機能するには、Marketo と他のアドビアプリケーションが同じ組織内に存在する必要があります。

>[!IMPORTANT]
>
>Adobe Business Platform と Identity Management システムにオンボードされているユーザの場合、サブスクリプションに関連付けられた組織 ID は既に入力されており、読み取り専用フィールドになっています。そのため、この記事の手順は当てはまりません。

1. Marketo で、「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. 統合で、「**[!UICONTROL アドビ組織マッピング]**」をクリックします。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. 「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. Adobe IMS 組織 ID を入力し（確認方法については、[こちら](https://experienceleague.adobe.com/docs/control-panel/using/faq.html?lang=ja){target="_blank"}を参照）、「**[!UICONTROL OK]**」をクリックします。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. 「**[!UICONTROL 確認]**」をクリックします。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. 「**[!UICONTROL 閉じる]**」をクリックします。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >セキュリティ上の理由から、マッピング先のアドビ組織の組織管理者である必要があります。さもないと、アクションは失敗します。また、アドビユーザと Marketo ユーザは、ログイン時に同じメールアドレスを使用する必要があります。

1. _まだログインしていない_&#x200B;場合は、新しいタブ／ウィンドウにポップアップが表示されます。アドビ組織にログインします（このアクションで組織アクセスが検証されます）。

これで完了です。Adobe Experience Cloudから [ オーディエンスデータを共有 ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target="_blank"} または [ オーディエンスを同期 ](/help/marketo/product-docs/adobe-experience-cloud-integrations/sync-an-audience-from-adobe-experience-cloud.md){target="_blank"} できるようになりました。
