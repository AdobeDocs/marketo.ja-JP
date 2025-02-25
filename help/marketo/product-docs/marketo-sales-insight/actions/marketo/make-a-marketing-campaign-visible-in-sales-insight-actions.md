---
description: Sales Insight アクションにマーケティングキャンペーンを表示 - Marketo ドキュメント - 製品ドキュメント
title: Sales Insight アクションにマーケティングキャンペーンを表示
exl-id: 223baca3-159e-4f0d-b26f-f4c924a39fc3
feature: Sales Insight Actions
source-git-commit: c6132bf5b393df38700ad9dd6f0c6414860e8bb6
workflow-type: ht
source-wordcount: '300'
ht-degree: 100%

---

# Sales Insight アクションにマーケティングキャンペーンを表示 {#make-a-marketing-campaign-visible-in-sales-insight-actions}

キャンペーンは、表示されている場合にのみ共有できます。

Sales Insight アクションを使用すると、ユーザは toutapp.com という新しいセールスアプリにアクセスできます。このアプリは新しいアクション機能セットを提供しますが、コアバージョンの Sales Insights で使用できる&#x200B;_マーケティングキャンペーンに追加_&#x200B;機能も継承します。マーケティングキャンペーンに追加機能へのアクセスをユーザに許可する場所（toutapp.com または MSI SFDC パッケージエクスペリエンス）に応じて、Marketo キャンペーンを異なる方法で設定する必要があるので、この点に留意することが重要です。詳しくは、手順 4 のメモを参照してください。

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
   >toutapp.com web アプリから&#x200B;_マーケティングキャンペーンに追加_&#x200B;を利用しているユーザにマーケティングキャンペーンを表示する場合（Marketo Sales Outbox オブジェクト経由で CRM に web アプリを埋め込んでいる場合も含まれます）、キャンペーンリクエストソースを「Web サービス API」に設定します。ユーザが Salesforce の MSI パネルのリード、取引先責任者、アカウントページでアクションを使用した際や、リードと取引先責任者リストビューの一括アクションボタンを使用した際に、マーケティングキャンペーンを表示するには、キャンペーンリクエストソースを「Sales Insight」に更新します。

1. 「**フロー**」タブをクリックします。

   ![](assets/make-a-marketing-campaign-visible-sia-5.png)

1. _注目のアクション_&#x200B;フローアクションを追加します。

   ![](assets/make-a-marketing-campaign-visible-sia-6.png)

1. タイプには、「**Web**」を選択します。

   ![](assets/make-a-marketing-campaign-visible-sia-7.png)

1. _説明_&#x200B;ボックスに、セールスチームにメッセージを書き込みます。この例では、トークンを使用して、入力されたフォームを指定します。

   ![](assets/make-a-marketing-campaign-visible-sia-8.png)

1. 「**スケジュール**」タブをクリックし、キャンペーンを&#x200B;**アクティベート**&#x200B;します。

   ![](assets/make-a-marketing-campaign-visible-sia-9.png)
