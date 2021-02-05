---
unique-page-id: 2359793
description: ソーシャルプロモーションでの電子メールの使用 — Marketto Docs — 製品ドキュメント
title: Social Promotionでの電子メールの使用
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---


# ソーシャルプロモーションでの電子メールの使用{#use-emails-in-social-promotions}

[参照オファー](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)または[懸賞](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)を作成する場合、登録時に送信する電子メールを含め、報酬を受け取ったときに再び送信する電子メールを含めることができます。

>[!TIP]
>
>電子メールの作成については、[電子メール送信](/help/marketo/getting-started/quick-wins/send-an-email.md)を参照してください。

電子メールでは、次のトークンを使用します。

* **入会用電子メール**:各参加者 **`{{social.Share Url}}`** に対してパーソナライズされた共有リンクを送信するために使用します。

* **購読提供数の電子メール**:各推奨結果 **`{{social.Promo Code}}`** にプロ [モーションコードを送信する場合に使用します](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md)。

>[!PREREQUISITES]
>
>Socialアプリに電子メールを追加する前に、_operational_&#x200B;および&#x200B;_approved_&#x200B;にする必要があります。 「[電子メールの設定の編集](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)」を参照してください。

1. **マーケティングアクティビティ**&#x200B;に移動します。

   ![](assets/ma.png)

1. アプリを選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. Social App Editorで、**アプリの設定/オファーの詳細**（または&#x200B;**懸賞の詳細**）に移動します。

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. 入追加会用の電子メール。

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >確認電子メールは、ユーザーがサインアップすると自動的に送信されます。

1. 購読提供数追加の電子メール

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. 参照オファーで、購読提供数電子メールを自動的に送信するか、手動で送信するかを選択します。

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>懸賞では、勝者](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md)を[選択したときに、購読提供数の電子メールが常に自動的に送信されます。

>[!NOTE]
>
>**定義**
>
>* **目標に対する自動**:各参加者が目標を達成すると、購読提供数の電子メールが自動的に送信されます。
>* **手動送信**:訪問者の開始が目標を達成したら、照会オファーに戻って、受渡通知用電子メールを手動で [送信し](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md)ます。

>



>[!MORELIKETHIS]
>
>次に、[共有URL](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md)を選択するか、参照オファーで送信するプロモーションコード](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md)を[アップロードします。
