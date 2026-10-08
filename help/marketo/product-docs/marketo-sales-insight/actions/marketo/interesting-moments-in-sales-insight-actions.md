---
description: Sales Insight Actionsの注目のアクションについて説明します。 MarketoとSalesforceで、主要なアクティビティがどのようにログに記録され、表示されるかを把握できます。
title: セールスインサイトアクションでの注目のアクション
exl-id: b2423fbb-9ce0-4ce9-bc26-93aa69aa9e12
feature: Sales Insight Actions
TQID: 'https://experienceleague.adobe.com/--be0j0yB-bSIgIqwXzBN2tIXb715oyun3RNqPj5-F0'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: 412786a7-b8da-5b9d-8c3f-2539a3faad9f
    internal-label: Sales Insight Actions
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 91%
---
# [!DNL Sales Insight Actions] での注目のアクション {#interesting-moments-in-sales-insight-actions}

注目のアクションは、[!DNL Marketo Sales Insight Actions] を通じてセールスチームとコミュニケーションを取る鍵となります。

## 注目のアクションとは？ {#what-is-an-interesting-moment}

それは、あなた次第です。 どんな情報がセールスチームに関係あるのかを自分で決定します。 セールスチームがリードについて知りたいのは、例えば次のようなことです。

* 自社 web サイトの価格設定ページを訪問する
* 新製品発表メールに記載されたリンクをクリック
* 製品デモをリクエスト

## 注目のアクションを作成するには {#how-do-i-create-an-interesting-moment}

1. [スマートキャンペーン](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md){target="_blank"}を選択します。トリガーされた場合にセールスチームが興味を持つものがいいでしょう。

   ![](assets/interesting-moments-in-sales-insight-actions-1.png)

1. **[!UICONTROL 注目のアクション]**&#x200B;フローステップをドラッグします。

   ![](assets/interesting-moments-in-sales-insight-actions-2.png)

1. **タイプ**&#x200B;を選択します（メール、マイルストーン、web）。

   ![](assets/interesting-moments-in-sales-insight-actions-3.png)

1. このアクションが重要である理由として、セールスチームへのメッセージを「**[!UICONTROL 説明]**」フィールドに記入します。

   ![](assets/interesting-moments-in-sales-insight-actions-4.png)

   >[!NOTE]
   >
   >Marketo によって、そのアクションが発生した日付と、どのようにして注目のアクションとして追加されたか（例：リードアクション > フローステップ、SOAP API）も追加されます。

## 注目のアクションは、Marketo でどのように表示されるか  {#what-does-an-interesting-moment-look-like-in-marketo}

注目のアクションは、[リードのアクティビティログ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}に表示されます。

![](assets/interesting-moments-in-sales-insight-actions-5.png)

## 注目のアクションは、[!DNL Sales Insight Actions] でどのように表示されるか {#what-does-an-interesting-moment-look-like-in-sales-insight-actions}

注目のアクションは、ユーザのライブフィードにリアルタイムで表示されます。 [!DNL Salesforce] のリード所有者 ID を利用して、ユーザが所有する関連リードの注目のアクションを表示します。 リード名の横にあるドロップダウンをクリックすると、メール／電話／セールスキャンペーンでリードを素早くフォローアップできます。

![](assets/interesting-moments-in-sales-insight-actions-6.png)
