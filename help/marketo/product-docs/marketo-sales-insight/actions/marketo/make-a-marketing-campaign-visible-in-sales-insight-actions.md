---
description: Sales Insight ActionsにMarketo マーケティングキャンペーンを表示する方法を説明します。 セールスユーザーがアクションからキャンペーンにリードを追加できるようにします。
title: セールスインサイトアクションへのマーケティングキャンペーンの表示
exl-id: 223baca3-159e-4f0d-b26f-f4c924a39fc3
feature: Sales Insight Actions
TQID: 'https://experienceleague.adobe.com/hIuHfnPyopakqjUeEmBc-EZ4sRrNnM-TptIOiqa1TEY'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: 412786a7-b8da-5b9d-8c3f-2539a3faad9f
    internal-label: Sales Insight Actions
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 92%
---
# セールスインサイトアクションにマーケティングキャンペーンを表示 {#make-a-marketing-campaign-visible-in-sales-insight-actions}

キャンペーンは、表示されている場合にのみ共有できます。

セールスインサイトアクションを使用すると、ユーザは toutapp.com という新しいセールスアプリにアクセスできます。 このアプリは新しいアクション機能セットを提供しますが、コアバージョンのセールスインサイトで使用できる&#x200B;_マーケティングキャンペーンに追加_&#x200B;機能も継承します。 マーケティングキャンペーンに追加機能へのアクセスをユーザに許可する場所（toutapp.com または MSI SFDC パッケージエクスペリエンス）に応じて、Marketo キャンペーンを異なる方法で設定する必要があるので、この点に留意することが重要です。 詳しくは、手順 4 のメモを参照してください。

1. 共有するキャンペーンを選択（または作成）します。

   ![](assets/make-a-marketing-campaign-visible-sia-1.png)

1. 「**スマートリスト**」タブをクリックします。

   ![](assets/make-a-marketing-campaign-visible-sia-2.png)

1. 「_キャンペーンをリクエスト_」トリガーに追加します。

   ![](assets/make-a-marketing-campaign-visible-sia-3.png)

1. ソースには、「is」「**Web サービス API**」を選択します。

   ![](assets/make-a-marketing-campaign-visible-sia-4.png)

   >[!NOTE]
   >
   >toutapp.com web アプリから&#x200B;_マーケティングキャンペーンに追加_&#x200B;を利用しているユーザにマーケティングキャンペーンを表示する場合（Marketo Sales Outbox オブジェクト経由で CRM に web アプリを埋め込んでいる場合も含まれます）、キャンペーンリクエストソースを「Web サービス API」に設定します。 ユーザーが Salesforce の MSI パネルで、リード、取引先責任者、アカウントのページ上のアクションや、リードおよび取引先責任者リストビューの一括アクションボタンを使用したときにマーケティングキャンペーンを表示したい場合は、キャンペーンリクエストソースを「セールスインサイト」に更新します。

1. 「**フロー**」タブをクリックします。

   ![](assets/make-a-marketing-campaign-visible-sia-5.png)

1. _注目のアクション_&#x200B;フローアクションを追加します。

   ![](assets/make-a-marketing-campaign-visible-sia-6.png)

1. タイプには、「**Web**」を選択します。

   ![](assets/make-a-marketing-campaign-visible-sia-7.png)

1. _説明_&#x200B;ボックスに、セールスチームにメッセージを書き込みます。 この例では、トークンを使用して、入力されたフォームを指定します。

   ![](assets/make-a-marketing-campaign-visible-sia-8.png)

1. 「**スケジュール**」タブをクリックし、キャンペーンを&#x200B;**アクティベート**&#x200B;します。

   ![](assets/make-a-marketing-campaign-visible-sia-9.png)
