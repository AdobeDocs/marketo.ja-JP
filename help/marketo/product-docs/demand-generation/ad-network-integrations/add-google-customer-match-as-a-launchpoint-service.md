---
unique-page-id: 12980661
description: Google カスタマーマッチを LaunchPoint サービスとして追加する方法を説明します。 AdWords、YouTube、検索および Gmail でのターゲティング用に、Marketo オーディエンスをGoogleに送信します。
title: Google カスタマーマッチを  [!DNL LaunchPoint]  サービスとして追加
exl-id: c780bde0-3044-4c89-a2ac-88398cbc3425
feature: Integrations
source-git-commit: 031eb5f3ff8aac185ce496664f984a4c745c6e44
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 87%

---

# Google カスタマーマッチを [!DNL LaunchPoint] サービスとして追加 {#add-google-customer-match-as-a-launchpoint-service}

この統合により、Marketo のオーディエンスを Google に送信して [!DNL Google AdWords] を使用してターゲットにしたり、YouTube、検索、[!DNL Gmail] を通じてオーディエンスをリターゲティングしたりすることができます。

>[!NOTE]
>
>**管理者権限が必要**

1. 「**[!UICONTROL 管理者]**」に移動します。

   ![](assets/admin.png)

1. **[!UICONTROL LaunchPoint]**.をクリックします。

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. 「**[!UICONTROL 新規]**」と「**[!UICONTROL 新規サービス]**」を選択します。

   ![](assets/image2014-12-5-14-3a37-3a33.png)

1. **[!UICONTROL 表示名]**&#x200B;を入力して&#x200B;**[!UICONTROL サービス]**&#x200B;ドロップダウンから「**[!UICONTROL Google カスタマーマッチ]**」を選択します。「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/chooseservice.png)

1. [!DNL Google AdWords] アカウントに接続するには、「**[!UICONTROL 認証]**」をクリックします。

   ![](assets/authorizeaccount-1.png)

1. Google が新しいタブで開きます。ここから、[!DNL Google AdWords] アカウントにログインします。

   >[!CAUTION]
   >
   >Marketo が複数の [!DNL AdWords] アカウント間でオーディエンスを送信するには、次の手順で認証する Google ユーザが、これらのアカウントの&#x200B;_すべて_&#x200B;にアクセスできる必要があります。

   ![](assets/chooseaccount.png)

1. 要求された権限を確認し、「**[!UICONTROL 許可]**」をクリックします。

   ![](assets/reviewpermissions.png)

1. これで、[!DNL Google AdWords] アカウントが Marketo に接続されました。「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/authorizesuccess.png)

   これで完了です。これで、「インストール済みのサービス」タブに [!DNL LaunchPoint] サービスとして「Google と一致するオーディエンス」が表示されます。

>[!NOTE]
>
>Google カスタマーマッチの統合には、1 つのマネージャーアカウントと、そのマネージャーアカウント内のサブアカウントすべてに対応できます。複数のマネージャーアカウントはサポートされていません。
