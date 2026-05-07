---
unique-page-id: 11379622
description: MarketoでFacebook リード広告を設定する方法について説明します。 Facebook アカウントを連携し、リードと送信された情報をMarketoに同期します。
title: Facebook リード広告の設定
exl-id: 24cb74da-6b46-45de-ba4a-66e3d490afd7
feature: Integrations
source-git-commit: d20c398cd1f5ed2646f56995c35a57630c3f2e95
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 68%

---

# Facebook リード広告の設定 {#set-up-facebook-lead-ads}

[Facebook リード広告](https://www.facebook.com/business/ads/ad-objectives/lead-generation){target="_blank"}を使用して、Facebook で広告キャンペーンを実行し、Marketo のリードを生成します。

>[!NOTE]
>
>* **管理者権限が必要**
>
>* Facebook リード広告フォームを作成する際に、フォーム名に数字以外の文字が含まれていないことを確認します。 フォーム名はアルファベットまたは英数字にする必要があります。

>[!AVAILABILITY]
>
>Facebook リード広告をインスタンスに追加するには、Adobe アカウントチーム（アカウントマネージャー）にお問い合わせください。

1. Marketo Engage で、**管理**&#x200B;エリアに移動します。

   ![](assets/set-up-facebook-lead-ads-1.png)

1. 「**LaunchPoint**」に移動します。「**新規**」をクリックして、「**新規サービス**」を選択します。

   ![](assets/set-up-facebook-lead-ads-2.png)

1. サービスの&#x200B;**[!UICONTROL 表示名]**&#x200B;を入力します。ドロップダウンから「**[!UICONTROL Facebook リード広告]**」サービスを選択し、「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/set-up-facebook-lead-ads-3.png)

1. 同じブラウザーで新しいタブを開き、[facebook.com](https://www.facebook.com){target="_blank"}.に移動します。 統合に使用するアカウントを使用して Facebook にログインします。

   >[!NOTE]
   >
   >[!DNL Facebook] アカウントで、リード広告を取り込むすべての [!DNL Facebook] ビジネスページにアクセスできる必要があります。

   ![](assets/set-up-facebook-lead-ads-4.png)

1. [!DNL Facebook]にログインしたら、Marketoに戻り、**[!UICONTROL 認証]**&#x200B;をクリックします。

   ![](assets/set-up-facebook-lead-ads-5.png)

1. プロンプトが表示されたら、「**[!UICONTROL OK]**」をクリックして、[!DNL Facebook] への Marketo アプリケーションのインストールを受け入れます。

   ![](assets/set-up-facebook-lead-ads-6.png)

1. 承認されたことに気づきます。 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/set-up-facebook-lead-ads-7.png)

1. Marketo で [!UICONTROL Facebook リード広告]を取り込むページを選択し、「**[!UICONTROL 次へ]**」をクリックします。

   >[!TIP]
   >
   >想定しているページが表示されない場合は、認証に使用された[!DNL Facebook] アカウントが[!DNL Facebook]のページに追加されていることを確認して、もう一度試してください。

   ![](assets/set-up-facebook-lead-ads-8.png)

1. Marketo フィールドのマッピングに対するデフォルトの[!DNL Facebook]を受け入れるには、**[!UICONTROL 作成]**&#x200B;をクリックします。

   >[!TIP]
   >
   >マッピングを変更することで、リード広告データが Marketo 内のどこに保存されるかをカスタマイズできます。 また、[リード広告カスタム質問からデータを取り込む](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md){target="_blank"}こともできます。

   >[!CAUTION]
   >
   >Marketo では、2 つの [!DNL Facebook] フィールドを 1 つの Marketo フィールドにマッピングできません。マッピングは 1 対 1 のみです。 2 対 1 のマッピングをおこなうと、リードを Marketo システムに配置できない場合があります。

   ![](assets/set-up-facebook-lead-ads-9.png)

   [!DNL Facebook] リード広告キャンペーンを成功に導くと、リードの Marketo への流れが始まります。

   ![](assets/set-up-facebook-lead-ads-10.png)

>[!MORELIKETHIS]
>
>* [リードアクセスマネージャー（Facebook）での権限の割り当て／削除](https://www.facebook.com/business/help/540596413257598?id=735435806665862){target="_blank"}
>* [スマートキャンペーンでのリード広告のフィルターとトリガーの使用](/help/marketo/product-docs/demand-generation/facebook/use-lead-ads-filters-and-triggers-in-a-smart-campaign.md){target="_blank"}
>* [カスタムフィールドの Marketo へのマッピング](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md){target="_blank"}
