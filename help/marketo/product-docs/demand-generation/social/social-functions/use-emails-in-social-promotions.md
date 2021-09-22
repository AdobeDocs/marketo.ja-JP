---
unique-page-id: 2359793
description: ソーシャルプロモーションでのメールの使用 - Marketo ドキュメント - 製品ドキュメント
title: ソーシャルプロモーションでのメールの使用
exl-id: 633ad86e-d085-420f-8e28-9b722e345852
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '237'
ht-degree: 100%

---

# ソーシャルプロモーションでのメールの使用 {#use-emails-in-social-promotions}

[紹介オファー](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)や[スイープステーク](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)を作成する場合、新規登録時と、その人物が報酬を獲得した後に送信するメールを含めることがきます。

>[!TIP]
>
>メールを作成するには、[メールブラストの送信](/help/marketo/getting-started/quick-wins/send-an-email.md)を参照してください。

メールでは、次のトークンを使用します。

* **新規登録用メール**：**`{{social.Share Url}}`** を使用して、参加する各ユーザーにパーソナライズされた共有リンクを送信します。

* **フルフィルメントメール**：**`{{social.Promo Code}}`** を使用して、各当選者に[プロモーションコード](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md)を送信します。

>[!PREREQUISITES]
>
>ソーシャルアプリにメールを追加するには、そのメールが&#x200B;_動作しており_、_承認済み_&#x200B;である必要があります。[メールの設定の編集](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)を参照してください。

1. **マーケティングアクティビティ**&#x200B;に移動します。

   ![](assets/ma.png)

1. アプリを選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. ソーシャルアプリエディターで、**アプリ設定／オファーの詳細**（または&#x200B;**スイープステークの詳細**）に移動します。

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. 新規登録用のメールを追加します。

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >確認メールは、ユーザーが新規登録すると自動的に送信されます。

1. フルフィルメントメールを追加します。

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. 紹介オファーで、フルフィルメントメールを自動的に送信するか、手動で送信するかを選択します。

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>スイープステークでは、](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md)当選者を選択[すると、必ずフルフィルメントメールが自動的に送信されます。

>[!NOTE]
>
>**定義**
>
>* **目標に応じて自動**：各参加者が目標を達成すると、フルフィルメントメールが自動的に送信されます。
>* **手動で送信**：ユーザーが目標を達成し始めたら、紹介オファーに戻って、[フルフィルメントメールを手動で送信](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md)します。

>



>[!MORELIKETHIS]
>
>次に、[共有 URL](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md)を選択するか、紹介オファーで送信する](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md)プロモーションコードをアップロード[します。
