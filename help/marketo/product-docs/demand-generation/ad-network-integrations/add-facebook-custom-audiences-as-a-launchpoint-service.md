---
unique-page-id: 4720257
description: LaunchPointサービスとしての追加Facebookのカスタムオーディエンス-Marketoドキュメント — 製品ドキュメント
title: LaunchPointサービスとしての追加Facebookのカスタムオーディエンス
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# LaunchPointサービスとしての追加Facebookのカスタムオーディエンス{#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**必要な管理者権限**

この統合により、Marketoの静的でスマートなリストからFacebookにオーディエンスデータを送信し、Facebook広告キャンペーンのカスタムオーディエンスとして使用できます。 設定方法を次に示します。

1. Marketo **管理者**&#x200B;に移動します。

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. **LaunchPoint**&#x200B;に移動し、「**新規**」をクリックして、「**新しいサービス**」を選択します。

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. サービスの&#x200B;**表示名**&#x200B;を入力し、**サービス**&#x200B;ドロップダウンから&#x200B;**Facebookカスタムオーディエンス**&#x200B;サービスを選択します。

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. 同じブラウザーで新しいタブを開き、[facebook.com](https://www.facebook.com/)に移動します。 統合に使用するアカウントを使用して、Facebookにログインします。

   >[!CAUTION]
   >
   >Marketoが複数のAd Managerアカウントでオーディエンスを送信するには、次の手順で承認するFacebookユーザーは、これらのアカウントの&#x200B;*すべて*&#x200B;にアクセスできる必要があります。

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. facebookにログインした後、Marketoに戻ります。 「**許可**」をクリックします。

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >カスタムオーディエンスの統合を機能させるには、_Facebookビジネスマネージャーのアカウントを使用する必要があります。_ Business Managerアカウントの設定方法については、[Facebookのヘルプ](https://www.facebook.com/business/help/1710077379203657)を参照してください。

1. プロンプトが表示されたら、「**OK**」をクリックして、FacebookへのMarketoアプリケーションのインストールを受け入れます。

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. 認証されました！ 一致するモードを選択し、「**作成**」をクリックします。

   >[!NOTE]
   >
   >**「基本** 一致」では、電子メールアドレスのみを使用します。**高度な** 一致では、コンバージョンを高めるために7つの追加のフィールドを使用します。一致率が増加します。ただし、会社のプライバシーポリシーで追加のフィールドの共有が許可されていない場合や、フィールドが含まれていない場合は、「基本一致」を選択します。

   ![](assets/fb-custom-adv-matching-hands.png)

   OK！Marketoの静的またはスマートなリストに移動して、オーディエンスデータをFacebookに送信できるようになりました。

   >[!CAUTION]
   >
   >ああ、行く前に、Facebookアカウント内で必ず[Facebookのカスタムオーディエンス条件](https://www.facebook.com/ads/manage/customaudiences/tos.php)に同意してください！ これを行わないと、オーディエンスの更新は失敗します。

>[!MORELIKETHIS]
>
>* [facebookでカスタムオーディエンスを作成](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
   >
   >
* [facebookリード広告の設定](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)

