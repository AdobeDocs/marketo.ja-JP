---
unique-page-id: 4720257
description: Facebook カスタムオーディエンスを LaunchPoint サービスとして追加 - Marketo ドキュメント - 製品ドキュメント
title: Facebook カスタムオーディエンスを LaunchPoint サービスとして追加
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 68%

---

# Facebook カスタムオーディエンスを LaunchPoint サービスとして追加 {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**管理者権限が必要**

この統合により、オーディエンスデータをMarketo Engageの静的リストおよびスマートリストからFacebookに送信し、Facebook広告キャンペーンでカスタムオーディエンスとして使用できます。 その設定方法を説明しましょう。

1. Marketo の「**[!UICONTROL 管理]**」に移動します。

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. **[!UICONTROL LaunchPoint]** に移動し、「新規 **[!UICONTROL をクリックして]** 新規サービス **[!UICONTROL を選択し]** す。

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. サービスの&#x200B;**[!UICONTROL 表示名]**&#x200B;を入力します。ドロップダウンから「**[!UICONTROL Facebook カスタムオーディエンス]**」サービスを選択し、「**[!UICONTROL 作成]**」をします。

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. 同じブラウザーで新しいタブを開き、[facebook.com](https://www.facebook.com/){target="_blank"} に移動します。 統合に使用するアカウントを使用して Facebook にログインします。

   >[!CAUTION]
   >
   >Marketo が複数の Ad Manager アカウント間でオーディエンスを送信するには、次の手順で承認した Facebook ユーザーはこれらのアカウントの&#x200B;*すべて*&#x200B;にアクセスできる必要があります。

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Facebook にログインした後、Marketo に戻ります。「**[!UICONTROL 許可]**」をクリックします。

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >カスタムオーディエンスの統合を機能させるには、Facebook Business Manager アカウントを使用する&#x200B;_必要があります_。Business Manager アカウントの設定方法については、[Facebook ヘルプ ](https://www.facebook.com/business/help/1710077379203657){target="_blank"} を参照してください。

1. プロンプトが表示されたら、「**[!UICONTROL OK]**」をクリックして、Facebook への Marketo アプリケーションのインストールを受け入れます。

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. 認証されました。一致モードを選択し、「**[!UICONTROL 作成]**」をクリックします。

   >[!NOTE]
   >
   >「**基本照合**」では電子メールアドレスのみが使用されます。**詳細照合**&#x200B;では、7 つの追加フィールドが使用されて、一致率を高め、コンバージョンを増やします。ただし、貴社のプライバシーポリシーで追加フィールドの共有が許可されていない場合や、追加フィールドがデータに含まれていない場合は、「基本照合」を選択してください。

   ![](assets/fb-custom-adv-matching-hands.png)

   完成です。Marketo内の静的リストまたはスマートリストに移動して、オーディエンスデータをFacebookに送信できるようになりました。

   >[!CAUTION]
   >
   >移動する前に、Facebook アカウント内で [Facebookのカスタムオーディエンス条件に同意する ](https://www.facebook.com/ads/manage/customaudiences/tos.php){target="_blank"} ことを確認してください。 これをおこなわないと、オーディエンスのアップデートが失敗します。

>[!MORELIKETHIS]
>
>* [Facebook でのカスタムオーディエンスの作成](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md){target="_blank"}
>
>* [Facebook リード広告の設定](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md){target="_blank"}
