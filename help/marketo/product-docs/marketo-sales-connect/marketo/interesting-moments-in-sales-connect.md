---
unique-page-id: 30082174
description: Sales ConnectとMarketoで、注目のアクションを把握。 セールス活動がライブフィードに流れる瞬間をどのように作成するかを説明します。
title: セールスコネクトにおける注目のアクション
exl-id: 210f31d1-606a-479d-8a2b-351b2b1a7678
feature: Marketo Sales Connect
TQID: 'https://experienceleague.adobe.com/KgwnG6Rpi3BJy-Vboy7MuPkjhz-O-BOzmncdgpbrNVU'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: ab9cc269-26ac-5c58-b645-e0736aefe9f3
    internal-label: Marketo Sales Connect
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 93%
---
# [!DNL Sales Connect] での注目のアクション {#interesting-moments-in-sales-connect}

注目のアクションは、[!DNL Marketo Sales Connect] を通じてセールスチームとコミュニケーションを取る鍵となります。

>[!AVAILABILITY]
>
>注目のアクションを使用できるのは、[Marketo セールスインサイト](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/using-interesting-moments.md)と[!DNL Marketo Sales Connect] を契約されたお客様だけです。

>[!PREREQUISITES]
>
>* [Salesforce CRM への接続](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md){target="_blank"}が必要です
>* Salesforce のリードまたは取引先責任者の所有者である必要があります
>* [Marketo Engage 接続へのアクセス権を付与](/help/marketo/product-docs/marketo-sales-connect/marketo/granting-access-to-users.md){target="_blank"}するには、アクセス権が必要です

## 注目のアクションとは何でしょうか。 {#what-is-an-interesting-moment}

それは、あなた次第です。 どんな情報がセールスチームに関係あるのかを自分で決定します。 セールスチームがリードについて知りたいのは、例えば次のようなことです。

* 自社 web サイトの価格設定ページを訪問する
* 新製品発表メールに記載されたリンクをクリック
* 製品デモをリクエスト

## 注目のアクションを作成するには {#how-do-i-create-an-interesting-moment}

1. [スマートキャンペーン](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)を選択します。トリガーされた場合にセールスチームが興味を持つものがいいでしょう。

   ![](assets/image2015-1-8-18-3a8-3a54.png)

1. **[!UICONTROL 注目のアクション]**&#x200B;フローステップをドラッグします。

   ![](assets/image2015-1-8-18-3a15-3a20.png)

1. **タイプ**&#x200B;を選択します（[!UICONTROL メール]、[!UICONTROL マイルストーン]、[!UICONTROL web]）。

   ![](assets/image2015-1-8-18-3a17-3a16.png)

1. このアクションが重要である理由として、セールスチームへのメッセージを「**[!UICONTROL 説明]**」フィールドに記入します。

   ![](assets/image2015-1-8-18-3a18-3a23.png)

   >[!NOTE]
   >
   >Marketo によって、そのアクションが発生した日付と、どのようにして注目のアクションとして追加されたか（例：リードアクション > フローステップ、SOAP API）も追加されます。

## 注目のアクションは、Marketo でどのように表示されるか  {#what-does-an-interesting-moment-look-like-in-marketo}

注目のアクションは、[リードのアクティビティログ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)に表示されます。

![](assets/image2015-1-14-18-3a45-3a58.png)

## 注目のアクションは、[!DNL Sales Connect] でどのように表示されるか {#what-does-an-interesting-moment-look-like-in-sales-connect}

注目のアクションは、ユーザのライブフィードにリアルタイムで表示されます。 [!DNL Salesforce] のリード所有者 ID を利用して、ユーザが所有する関連リードの注目のアクションを表示します。 リード名の横にあるドロップダウンをクリックすると、メール／電話／セールスキャンペーンでリードを素早くフォローアップできます。

![](assets/engagement.jpg)
