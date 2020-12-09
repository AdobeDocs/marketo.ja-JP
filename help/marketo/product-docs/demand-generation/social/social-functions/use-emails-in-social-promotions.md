---
unique-page-id: 2359793
description: ソーシャルプロモーションでの電子メールの使用 — Marketto Docs — 製品ドキュメント
title: Social Promotionでの電子メールの使用
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 0%

---


# Social Promotionでの電子メールの使用 {#use-emails-in-social-promotions}

リフ [ァラルオファー](../../../../product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) 、 [懸賞を作成する場合](../../../../product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)、登録時に送信する電子メールを含めたり、受賞時に再送信したりできます。

>[!TIP]
>
>電子メールの作成については、「電子メール送信 [](../../../../getting-started/quick-wins/send-an-email.md)」を参照してください。

電子メールでは、次のトークンを使用します。

* **入会用電子メール**:各参加者 **`{{social.Share Url}}`** に対してパーソナライズされた共有リンクを送信する場合に使用します。

* **購読提供数の電子メール**:各推奨結果 **`{{social.Promo Code}}`** にプロ [モーションコードを送信する場合に使用します](use-promo-codes-for-offer-fulfillment.md)。

>[!PREREQUISITES]
>
>Socialアプリに電子メールを追加する前に、電子メールが *操作可能で* 、 *承認されている必要があります*。 「電子メールの設定の [編集](../../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)」を参照してください。

1. 「 **マーケティングアクティビティ**」に移動します。

   ![](assets/ma.png)

1. アプリを選択し、「ドラフトを **編集**」をクリックします。

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. Socialアプリエディターで、 **アプリ設定/オファーの詳細** (または「 **懸賞の詳細**」)に移動します。

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
>懸賞では、勝者を [選択した場合、受賞者の電子メールが常に自動的に送信されます](../../../../product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md)。

>[!NOTE]
>
>**定義**
>
>* **目標に対する自動**:各参加者が目標を達成すると、購読提供数の電子メールが自動的に送信されます。
>* **手動送信**:訪問者の開始が目標を達成したら、照会オファーに戻って、受渡通知用電子メールを手動で [送信し](../../../../product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md)ます。

>



>[!NOTE]
>
>**関連記事**
>
>次に、共有URL [を選択するか](choose-the-share-url-for-a-social-app.md) 、参照オファーで送信するプロモーションコードを [アップロードします](use-promo-codes-for-offer-fulfillment.md) 。

