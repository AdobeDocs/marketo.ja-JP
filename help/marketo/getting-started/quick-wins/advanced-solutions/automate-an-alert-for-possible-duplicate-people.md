---
unique-page-id: 7513680
description: 可能な重複者に対するアラートの自動化 —Marketoドキュメント — 製品ドキュメント
title: 重複の可能性があるユーザーに対するアラートの自動化
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# 考えられる重複の人に対するアラートの自動化{#automate-an-alert-for-possible-duplicate-people}

重複担当者が作成されるたびにアラートを送信しますか？ スマートキャンペーンを設定する方法を次に示します。

1. [新しいスマートキャンペーンを作成します](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md)。次のスマートリストを定義します。

* トリガー:**人物は作成されました**
* フィルタ：**重複フィールド。** Field Name  **is Full Name**

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >創造力を持って。 様々なフィールドを試して、より適切なフィルター結果を得ることができます。

1. フローステップで、「[警告](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md)の送信」フローアクションを選択します。

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >[警告情報トークン](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md)を使用して、CRM内のユーザーへのリンクを含めます。

   >[!CAUTION]
   >
   >大きなリストをインポートすると、これらの警告の一括が一度に表示される場合があります。
   >
   >また、同じ名前の2人が自動的に同じ人物であるとは限りません。

1. 「**スケジュール**」タブでキャンペーンをアクティブにします。

   ![](assets/image2017-3-27-8-3a24-3a37.png)

それだ！ このスマートキャンペーンは、既存のフルネームを持つ新しい人がMarketoで作成されるたびにトリガーを行います。

>[!MORELIKETHIS]
>
>[重複ユーザーの検索と結合](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)
