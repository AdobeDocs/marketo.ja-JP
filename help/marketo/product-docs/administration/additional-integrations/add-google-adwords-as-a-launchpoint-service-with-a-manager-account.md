---
unique-page-id: 7504893
description: '"追加 [!DNL Google AdWords] as a [!DNL Launchpoint] Manager アカウントを使用したサービス — Marketoドキュメント — 製品ドキュメント»'
title: '"追加 [!DNL Google AdWords] as a [!DNL Launchpoint] 管理者アカウントを使用したサービス»'
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
source-git-commit: eb20d804a06bd02b61368e34ad1965a873d2fdf5
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 40%

---

# 追加 [!DNL Google AdWords] as a [!DNL Launchpoint] 管理者アカウントを使用したサービス {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

リンク [!DNL Google AdWords] アカウントをMarketoに自動的にアップロードし、Marketoからにオフラインのコンバージョンデータを [!DNL Google AdWords]. 次に、 [!DNL AdWords] UI では、どのクリックが選定されたリード、商談、新規顧客（または追跡したい収益ステージ）につながったかを簡単に確認できます  [カスタム列を追加](https://support.google.com/adwords/answer/3073556){target="_blank"} in [!DNL AdWords]. この情報は、Marketo UI には表示されません。

複数の [!DNL Google Adwords] アカウントを使用する場合、 [[!DNL Google AdWords Manager Account]](https://www.google.com/adwords/manager-accounts/){target="_blank"} ( 旧称： [!DNL My Client Center]) を使用して、Marketoと統合できます。

詳しくは、[Google のオフラインコンバージョンのインポート機能](https://support.google.com/adwords/answer/2998031?hl=ja){target="_blank"}を参照してください。

>[!AVAILABILITY]
>
>必ずしもすべてのお客様がこの機能を購入済みとは限りません。詳しくは、アドビアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

>[!NOTE]
>
>**管理者権限が必要**

>[!NOTE]
>
>また、 [スタンドアロン [!DNL Google AdWords] としてアカウント [!DNL Launchpoint] サービス](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md){target="_blank"}.

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-1.png)

1. 「**[!UICONTROL LaunchPoint]**」を選択します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-2.png)

1. 「**[!UICONTROL 新規]**」ドロップダウンをクリックして、「**[!UICONTROL 新規サービス]**」を選択します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-3.png)

1. を入力します。 **[!UICONTROL 表示名]** を選択し、 **[!UICONTROL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-4.png)

1. 「**[!UICONTROL Marketo を承認]**」を選択します。

   >[!NOTE]
   >
   >個人からログアウトするようにしてください [!DNL Gmail] アカウントを作成し、ポップアップを有効にします。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-5.png)

1. 次に関連するアカウントを選択 **[!DNL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-6.png)

1. 「**[!UICONTROL 確定]**」をクリックします。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-7.png)

1. ステータスは「**[!UICONTROL 成功]**」と表示されます。「**[!UICONTROL 次へ]**」を選択します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-8.png)

1. Marketoからへのオフライン変換のアップロード [!DNL Google AdWords] **[!UICONTROL 毎週]** または **[!UICONTROL 毎日]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-9.png)

1. 属性コンバージョンで、「**[!UICONTROL 最初のクリック]**」または「**[!UICONTROL 最後のクリック]**」を選択します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-10.png)

   | タイプ | 定義 |
   |---|---|
   | [!UICONTROL 最初のクリック] | オフラインコンバージョンは最初の [!DNL AdWords] 過去 90 日間にクリックした人 |
   | [!UICONTROL 最後のクリック] | オフラインコンバージョンは、最後の [!DNL AdWords] 人がクリックした広告 |

   >[!NOTE]
   >
   >この機能を使用するには、[自動タグ付け](https://support.google.com/adwords/answer/1752125?hl=ja){target="_blank"}を選択する必要があります。内で有効化する必要があります [!DNL AdWords].

1. 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-11.png)

1. 更新しないアカウントの選択を解除します。「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-12.png)

   マッピング方法については、以下の関連記事を参照してください。 [!DNL AdWords] オフラインコンバージョンを売上高モデルで使用できます。

   >[!MORELIKETHIS]
   >
   >[ [!DNL Google AdWords] マネージャーアカウントを使用した収益モデルでの コンバージョンの設定](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md){target="_blank"}
