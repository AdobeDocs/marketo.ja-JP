---
unique-page-id: 2359791
description: 紹介オファーの目標を指定する - Marketo ドキュメント - 製品ドキュメント
title: 紹介オファーの目標を指定する
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 100%

---

# 紹介オファーの目標を指定する {#specify-goal-for-referral-offer}

[紹介オファーを作成](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)する場合、達成目標を定義する必要があります。目標は、ページ訪問数や新規登録数など、Web ページ上のユーザーのアクティビティによって定義できます。さらに、[カスタム JavaScript イベント](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md)を使用することもできます。

また、Marketo のスマートリストトリガーを使用して、参照元に対して商談が作成されるなど、任意のマイルストーンを待つこともできます。

目標の例：

* 10 件の参照による訪問
* 5 件の参照による新規登録
* 1 件の参照による商談の作成
* 2 件の参照による e コマース購入
* 5 件の参照によるウェビナー参加者

1. **マーケティング活動**&#x200B;に移動します。

   ![](assets/ma.png)

1. 紹介オファーを選択して、「**下書きの編集**」をクリックします。

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. 紹介オファーエディターで、「**アプリ設定**」、「**オファーの詳細**」の順に移動します。

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. **設定**&#x200B;で、イベントタイプを&#x200B;**達成目標**&#x200B;ドロップダウンリストから選択します。

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>**参照元にクレジットを付与**&#x200B;フローステップを使用する予定がある場合、ここで達成目的タイプとして&#x200B;**スマートリストトリガー**&#x200B;を選択する必要があります。

* 参照による訪問：オファー参加者は、オファーをホストする友達からページへの訪問ごとにクレジットを受け取ります。
* 参照による新規登録：オファー参加者は、オファーに新規登録する各友達のクレジットを受け取ります。
* スマートリストトリガー：オファー参加者は、[スマートキャンペーン](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md)で[スマートリスト](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)トリガーの条件を満たす各友達のクレジットを受け取ります。例えば、参照元の見込み客がウェビナーに新規登録したときに実行されるトリガーを使用できます。

* カスタム JavaScript イベント：オファー参加者は、ページ上の定義済みの JavaScript イベントにトリガーを持つ各友達のクレジットを受け取ります。[カスタムイベントのコンバージョンスクリプト](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)を参照してください。

>[!NOTE]
>
>スマートキャンペーンで、ソーシャルアクティビティを監視するための新しいフィルターとトリガーが利用できます。[ソーシャルアクティビティのトリガーとフィルターの使用](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)を参照してください。

>[!MORELIKETHIS]
>
>次に、紹介オファーから送信する[新規登録メールと達成メールを選択](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md)できます。
