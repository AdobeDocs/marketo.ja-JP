---
description: Sales Insight アクションでマーケティングキャンペーンを表示 – Marketo ドキュメント – 製品ドキュメント
title: マーケティングキャンペーンをセールスインサイトアクションに表示
exl-id: 223baca3-159e-4f0d-b26f-f4c924a39fc3
feature: Sales Insight Actions
source-git-commit: c6132bf5b393df38700ad9dd6f0c6414860e8bb6
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 16%

---

# マーケティングキャンペーンをセールスインサイトアクションに表示 {#make-a-marketing-campaign-visible-in-sales-insight-actions}

キャンペーンは、表示可能になっている場合にのみ共有できます。

Sales Insight Actions を使用すると、ユーザーはtoutapp.comという新しい販売アプリにアクセスできます。 このアプリは、新しいアクション機能セットを提供するだけでなく、コアバージョンの Sales Insights で使用可能な _マーケティングキャンペーンに追加_ 機能も継承します。 ユーザーがマーケティングキャンペーンに追加機能（toutapp.comまたは MSI SFDC パッケージエクスペリエンス）にアクセスする場所に応じて、Marketo キャンペーンを別の方法で設定する必要があるので、この点に留意することが重要です。 詳しくは、手順 4 のメモを参照してください。

1. 共有するキャンペーンを選択（または作成）します。

   ![](assets/make-a-marketing-campaign-visible-sia-1.png)

1. 「**スマートリスト**」タブをクリックします。

   ![](assets/make-a-marketing-campaign-visible-sia-2.png)

1. _キャンペーンをリクエスト済み_&#x200B;トリガーーを追加します。

   ![](assets/make-a-marketing-campaign-visible-sia-3.png)

1. ソースには、「is」「**Web サービス API**」を選択します。

   ![](assets/make-a-marketing-campaign-visible-sia-4.png)

   >[!NOTE]
   >
   >toutapp.com web アプリから _マーケティングキャンペーンに追加_ を使用しているユーザーにマーケティングキャンペーンを表示する場合（これは、web アプリをMarketo Sales Outbox オブジェクト経由で CRM に埋め込んでいる場合も含みます）、Campaign リクエストのソースを「Web サービス API」に設定します。 Salesforceの MSI パネルのリード、連絡先、アカウントページ、またはリードビューと連絡先リストビューの一括アクションボタンでユーザーがアクションを使用する際にマーケティングキャンペーンを表示する場合は、キャンペーンリクエストソースを「Sales Insight」に更新します

1. 「**フロー**」タブをクリックします。

   ![](assets/make-a-marketing-campaign-visible-sia-5.png)

1. _興味深い瞬間_ フローアクションを追加します。

   ![](assets/make-a-marketing-campaign-visible-sia-6.png)

1. タイプには、「**Web**」を選択します。

   ![](assets/make-a-marketing-campaign-visible-sia-7.png)

1. 「_説明_」ボックスに、営業チームへのメッセージを入力します。 この例では、トークンを使用して、入力されたフォームを指定します。

   ![](assets/make-a-marketing-campaign-visible-sia-8.png)

1. 「**スケジュール**」タブをクリックし、キャンペーンを&#x200B;**アクティベート**&#x200B;します。

   ![](assets/make-a-marketing-campaign-visible-sia-9.png)
