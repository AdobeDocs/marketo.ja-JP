---
unique-page-id: 4720257
description: サービスとして  [!DNL Facebook]  カスタムオーディエ  [!DNL LaunchPoint]  スの追加 – Marketo ドキュメント – 製品ドキュメント
title: Add [!DNL Facebook] Custom Audiences as a [!DNL LaunchPoint] Service
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 32%

---

# カスタムオ [!DNL Facebook] ディエンスを [!DNL LaunchPoint] Service として追加 {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**管理者権限が必要**

この統合を利用すると、オーディエンスデータをMarketoの静的リストとスマートリストから送信し、[!DNL Facebook] Ad キャンペーンでカスタムオーディエンスとして使用で [!DNL Facebook] るようになります。 その設定方法を説明しましょう。

1. Marketo の「**[!UICONTROL 管理]**」に移動します。

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. **[!UICONTROL LaunchPoint]** に移動して、「**[!UICONTROL 新規]**」をクリックし、「**[!UICONTROL 新規サービス]**」を選択します。

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. サービスの&#x200B;**[!UICONTROL 表示名]**&#x200B;を入力します。ドロップダウンから「**[!UICONTROL Facebook カスタムオーディエンス]**」サービスを選択し、「**[!UICONTROL 作成]**」をします。

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. 同じブラウザーで新しいタブを開き、[facebook.com](https://www.facebook.com/).に移動します。統合に使用したいアカウントを使用して、[!DNL Facebook] にログインします。

   >[!CAUTION]
   >
   >Marketoが複数の Ad Manager アカウントをまたいでオーディエンスを送信するには、次の手順で認証する [!DNL Facebook] ユーザーがこれらのアカウントの *すべて* にアクセスできる必要があります。

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. [!DNL Facebook] にログインしたら、Marketoに戻ります。 「**[!UICONTROL 許可]**」をクリックします。

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >カスタムオーディエンス統合を機能させるには ** Business Manager アカウントを使用する [!DNL Facebook] 必要があります）。 Business Manager アカウントの設定方法については、[[!DNL Facebook]  ヘルプ &#x200B;](https://www.facebook.com/business/help/1710077379203657) を参照してください。

1. プロンプトが表示されたら、「**[!UICONTROL OK]**」をクリックして、[!DNL Facebook] へのMarketo アプリケーションのインストールを承認します。

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. 認証されました。一致モードを選択し、「**[!UICONTROL 作成]**」をクリックします。

   >[!NOTE]
   >
   >「**[!UICONTROL 基本照合]**」では電子メールアドレスのみが使用されます。**[!UICONTROL 詳細照合]**&#x200B;では、7 つの追加フィールドが使用されて、一致率を高め、コンバージョンを増やします。ただし、会社のプライバシーポリシーで追加フィールドの共有が許可されていない場合や、データに含まれていない場合は、「[!UICONTROL &#x200B; 基本一致 &#x200B;]」を選択します。

   ![](assets/fb-custom-adv-matching-hands.png)

   これで完了です。Marketo内の静的リストまたはスマートリストに移動して、オーディエンスデータを [!DNL Facebook] に送信できるようになりました。

   >[!CAUTION]
   >
   >移動する前に、[&#x200B; アカウント内で  [!DNL Facebook] カスタムオーディエンス条件に同意する &#x200B;](https://www.facebook.com/ads/manage/customaudiences/tos.php) [!DNL Facebook] ことを確認してください。 これをおこなわないと、オーディエンスのアップデートが失敗します。

>[!MORELIKETHIS]
>
>* [&#x200B; でのカスタムオーディエンスの作成  [!DNL Facebook]](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
>
>* [&#x200B; リード広告  [!DNL Facebook]  設定 &#x200B;](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
