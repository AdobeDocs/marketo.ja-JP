---
unique-page-id: 1147034
description: SFDCキャンペーン追加- Marketto Docs — 製品ドキュメント
title: SFDC追加キャンペーン
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# SFDC追加キャンペーン {#add-to-sfdc-campaign}

>[!NOTE]
>
>**FYI**
>
>Marketoは現在、すべての購読で言語を標準化しているので、購読およびdocs.marketo.comの人物/人物にリード/リードを表示できます。 これらの用語は同じことを意味し、記事の説明には影響しません。 他にも変化がある。 [詳細情報](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!NOTE]
>
>Salesforceと統合されている場合にのみ使用できます。

## 概要 {#overview}

このフローステップは、Marketorキャンペーンで使用することも、Salesforceキャンペーンでリードとして人を追加する単一のフローステップとして使用することもできます。 リードがSalesforceにまだ存在しない場合は、自動的に同期され、指定されたステータスでキャンペーンに追加されます。

![](assets/image2014-9-22-15-3a43-3a36.png)

## 使用状況 {#usage}

1. リードを追加するSalesforceキャンペーンを探して選択します。

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >キャンペーンリストにSalesforceキャンペーンが表示されない場合：
   >
   >    
   >    
   >    1. [キャンペーンの同期が有効になっていることを確認します](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)。
   >    1. Salesforceの [マーケティングユーザー](../../../../product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) (Marketto Sync User [](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) )であることを確認します。


   >[!TIP]
   >
   >Salesforceキャンペーン [マイトークン](../../../../product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) (My Tokens)を使用すると、プログラムのクローン作成を容易にできます。

1. リードが追加されたときに、リードに割り当てるSalesforceキャンペーンメンバーのステータスを選択します。

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >既にSalesforceキャンペーンのリードメンバーになっている人はスキップされ、そのステータスは更新されません。 代わりに、SFDCキャンペーンでこれらのステータスを [変更することができます](change-status-in-sfdc-campaign.md) 。

