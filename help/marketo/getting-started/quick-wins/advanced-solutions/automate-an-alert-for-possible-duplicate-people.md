---
unique-page-id: 7513680
description: 考えられる重複者に対するアラートの自動化 — マーケティング担当者ドキュメント — 製品ドキュメント
title: 重複の可能性があるユーザーに対するアラートの自動化
translation-type: tm+mt
source-git-commit: 3c24395e55c756184615941327e15e050fa7d0ac
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---


# 重複の可能性があるユーザーに対するアラートの自動化 {#automate-an-alert-for-possible-duplicate-people}

重複担当者が作成されるたびにアラートを送信しますか？ スマートキャンペーンを設定する方法を次に示します。

>[!NOTE]
>
>**FYI**
>
>Marketoは現在、すべての購読で言語を標準化しているので、購読およびdocs.marketo.comの人物/人物にリード/リードを表示できます。 これらの用語は同じことを意味し、記事の説明には影響しません。 他にも変化がある。 [詳細情報](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

1. [新しいスマートキャンペーンを作成します](../../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md)。 次のスマートリストを定義します。

   * トリガー： **個人が作成される**
   * フィルタ：**重複フィールド **Field Name **は** Full Name ****。

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >創造力を持って。 様々なフィールドを試して、より適切なフィルター結果を得ることができます。

1. フローステップで、「アラート [フローアクションの送信](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) 」を選択します。

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >警告情報トークン [の送信を使用して](../../../product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) 、CRMのユーザーへのリンクを含めます。

   >[!CAUTION]
   >
   >大きなリストをインポートすると、これらの警告の一括が一度に表示される場合があります。
   >
   >
   >また、同じ名前の2人が自動的に同じ人物であるとは限りません。

1. 「 **スケジュール** 」タブでキャンペーンをアクティブにします。

   ![](assets/image2017-3-27-8-3a24-3a37.png)

それだ！ このスマートキャンペーンは、既存のフルネームを持つ新しいユーザーがMarketoで作成されるたびにトリガーされます。

>[!MORELIKETHIS]
>
>* [重複ユーザーの検索と結合](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)

