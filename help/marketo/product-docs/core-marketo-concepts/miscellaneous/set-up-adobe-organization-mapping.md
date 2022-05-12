---
unique-page-id: 42762511
description: Adobe組織マッピングの設定 — Marketoドキュメント — 製品ドキュメント
title: 組織マッピングAdobeの設定
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
source-git-commit: bbe5f4a1502ab79d0081807ea6aab196ae75360a
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 44%

---

# 組織マッピングAdobeの設定 {#set-up-adobe-organization-mapping}

Audience Manager、B2B CDP Marketoコネクタ、Dynamic Chat などのAdobeアプリケーションと同期するには、まずMarketoでAdobe IMS組織の資格情報を入力する必要があります。

>[!NOTE]
>
>Marketo インスタンスの HIPAA 対応デプロイメントでは、この統合を使用できません。

>[!CAUTION]
>
>AdobeビジネスプラットフォームとIdentity Managementシステムにオンボーディングされた顧客の場合、サブスクリプションに関連付けられている組織 ID は既に入力されており、読み取り専用フィールドになります。

1. Marketo で、「**管理者**」をクリックします。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. 統合で、「**アドビ組織マッピング**」をクリックします。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. 「**編集**」をクリックします。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. アドビの IMS 組織 ID を入力し（[こちら](https://experienceleague.adobe.com/docs/control-panel/using/faq.html)を参照して特定）、「**OK**」をクリックします。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. 「**確認**」をクリックします。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. 「**閉じる**」をクリックします。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >セキュリティ上の理由から、マッピング先のアドビ組織の組織管理者である必要があります。そうでない場合、アクションは失敗します。 また、AdobeユーザーとMarketoユーザーは、ログイン時に同じ電子メールアドレスを使用する必要があります。

1. _まだログインしていない_&#x200B;場合は、新しいタブ／ウィンドウにポップアップが表示されます。アドビ組織にログインします（このアクションで組織アクセスが検証されます）。

これで完了です。次の操作を実行できます。 [オーディエンスデータを共有](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target=&quot;_blank&quot;} をまたは [オーディエンスを同期](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/sync-an-audience-from-adobe-experience-cloud.md)Adobe Experience Cloudから {target=&quot;_blank&quot;}。
