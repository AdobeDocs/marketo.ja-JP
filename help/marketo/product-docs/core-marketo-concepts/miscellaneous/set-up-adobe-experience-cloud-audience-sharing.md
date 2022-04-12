---
unique-page-id: 42762511
description: Adobe Experience Cloud オーディエンス共有のセットアップ - Marketo ドキュメント - 製品ドキュメント
title: Adobe Experience Cloud オーディエンス共有のセットアップ
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
source-git-commit: 41d8762203786bac9aea03ac978daa0549ac8e93
workflow-type: ht
source-wordcount: '167'
ht-degree: 100%

---

# Adobe Experience Cloud オーディエンス共有のセットアップ {#set-up-adobe-experience-cloud-audience-sharing}

アドビのアプリケーションとオーディエンスデータを共有するには、まず Marketo にアドビの IMS 組織資格情報を入力する必要があります。手順は以下のとおりです。

>[!NOTE]
>
>Marketo インスタンスの HIPAA 対応デプロイメントでは、この統合を使用できません。

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

   >[!NOTE]
   >
   >セキュリティ上の理由から、マッピング先のアドビ組織の組織管理者である必要があります。さもないと、アクションは失敗します。

1. _まだログインしていない_&#x200B;場合は、新しいタブ／ウィンドウにポップアップが表示されます。アドビ組織にログインします（このアクションで組織アクセスが検証されます）。

これで完了です。Adobe Experience Cloud から[オーディエンスデータを共有する](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)または[同期する](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/sync-an-audience-from-adobe-experience-cloud.md)ことができるようになります。
