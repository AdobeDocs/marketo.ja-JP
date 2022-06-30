---
unique-page-id: 7513680
description: 重複の可能性がある人物のアラートの自動化 - Marketo ドキュメント - 製品ドキュメント
title: 重複の可能性がある人物のアラートの自動化
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 78%

---

# 重複の可能性がある人物のアラートの自動化 {#automate-an-alert-for-possible-duplicate-people}

重複の可能性がある人物が作成されるたびにアラートを表示しますか？スマートキャンペーンを設定する方法を次に示します。

1. [新しいスマートキャンペーンを作成](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target=&quot;_blank&quot;}。 次のスマートリストを定義します。

* トリガー：**人物が作成される**
* フィルター：**重複フィールド。**&#x200B;フィールド名は「**氏名**」

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >クリエイティブになりましょう。様々なフィールドを試すことで、フィルタリング結果を向上できます。

1. フローステップで、 [アラートの送信](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md){target=&quot;_blank&quot;} フローアクション。

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >の使用 [アラート情報トークンの送信](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target=&quot;_blank&quot;} をクリックして、CRM に個人へのリンクを含めます。

   >[!CAUTION]
   >
   >サイズの大きいリストをインポートすると、大量のアラートが表示される可能性があります。
   >
   >また、同じ名前の 2 人が自動的に同じ人物であるとは限りません。

1. 「**スケジュール**」タブのキャンペーンをアクティブ化します。

   ![](assets/image2017-3-27-8-3a24-3a37.png)

これで完了です。このスマートキャンペーンは、既存の氏名を持つ新しい人物が Marketo で作成されるたびにトリガーされます。

>[!MORELIKETHIS]
>
>[重複リードの検索と結合](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target=&quot;_blank&quot;}
