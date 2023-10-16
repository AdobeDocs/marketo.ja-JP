---
unique-page-id: 6095008
description: " [!DNL Google AdWords]  を  [!DNL LaunchPoint]  サービスとして追加 - Marketo ドキュメント - 製品ドキュメント"
title: " [!DNL Google AdWords]  を  [!DNL LaunchPoint]  サービスとして追加"
exl-id: 993a057a-3f98-4a9f-a770-c9c80dedfd81
feature: Administration, Integrations
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 93%

---

# [!DNL Google AdWords] を [!DNL LaunchPoint] サービスとして追加 {#add-google-adwords-as-a-launchpoint-service}

[!DNL Google AdWords] アカウントを Marketo にリンクして、オフラインのコンバージョンデータを Marketo から [!DNL Google AdWords] に自動的にアップロードします。[!DNL AdWords] に[カスタム列を追加](https://support.google.com/adwords/answer/3073556){target="_blank"}した後、どのクリックが条件を満たすリードや商談、新規顧客（またはトラッキングしたいあらゆる売上高ステージ）につながったのかを [!DNL AdWords] UI から簡単に確認できるようになります。この情報は、Marketo UI には表示されません。

詳しくは、[Google のオフラインコンバージョンのインポート機能](https://support.google.com/adwords/answer/2998031?hl=ja){target="_blank"}を参照してください。

>[!AVAILABILITY]
>
>すべてのMarketo Engageユーザーがこの機能を購入したわけではありません。 詳しくは、Adobeアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

>[!NOTE]
>
>**管理者権限が必要**

>[!NOTE]
>
>また、[[!DNL Google AdWords] as a [!DNL Launchpoint]  サービスをマネージャーアカウント](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md){target="_blank"}と統合できます。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-1.png)

1. 「**[!UICONTROL LaunchPoint]**」を選択します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-2.png)

1. 「**[!UICONTROL 新規]**」と「**[!UICONTROL 新規サービス]**」を選択します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-3.png)

1. [!UICONTROL 表示名]を入力し、「**[!UICONTROL Google AdWords]**」を選択します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-4.png)

1. 「**[!UICONTROL Marketo を承認]**」を選択します。

   >[!NOTE]
   >
   >個人の [!DNL Gmail] アカウントからログアウトし、ポップアップを有効にします。

   ![](assets/add-google-adwords-as-a-launchpoint-service-5.png)

1. [!DNL Google AdWords] に関連付けられたアカウントを選択します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-6.png)

1. 「**[!UICONTROL 承認]**」を選択します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-7.png)

1. ステータスは「**[!UICONTROL 成功]**」と表示されます。「**[!UICONTROL 次へ]**」を選択します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-8.png)

1. Marketo から [!DNL Google AdWords] にオフラインコンバージョンをアップロードする送信頻度として、「**[!UICONTROL 毎週]**」または「**[!UICONTROL 毎日]**」を選択します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-9.png)

1. 属性コンバージョンで、「**[!UICONTROL 最初のクリック]**」または「**[!UICONTROL 最後のクリック]**」を選択します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-10.png)

   | タイプ | 定義 |
   |---|---|
   | [!UICONTROL 最初のクリック] | オフラインコンバージョンは、過去 90 日間で人物がクリックした最初の [!DNL AdWords] 広告に起因します |
   | [!UICONTROL 最後のクリック] | オフラインコンバージョンは、人物がクリックした最後の [!DNL AdWords] 広告に起因します |

   >[!NOTE]
   >
   >Marketo と [!DNL AdWords] で一貫したアトリビューションモデルを使用することで、最も正確なデータが得られます。

1. 「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/add-google-adwords-as-a-launchpoint-service-11.png)

   >[!NOTE]
   >
   >この機能を使用するには、[自動タギング](https://support.google.com/adwords/answer/1752125?hl=ja){target="_blank"}を選択する必要があります。非アクティブ化は [!DNL AdWords] 内で行う必要があります。

完了です。次は、関連記事を参照して、売上高モデルで [!DNL AdWords] のオフラインコンバージョンをマッピングする方法を学びましょう。

>[!MORELIKETHIS]
>
>[売上高モデルでの  [!DNL Google AdWords]  コンバージョンの設定](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model.md){target="_blank"}
