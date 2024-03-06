---
unique-page-id: 12980661
description: Google カスタマーマッチを LaunchPoint サービスとして追加 - Marketo ドキュメント - 製品ドキュメント
title: Google カスタマーマッチを LaunchPoint サービスとして追加
exl-id: c780bde0-3044-4c89-a2ac-88398cbc3425
feature: Integrations
source-git-commit: 3cb7e5ddef8ec05a7cf8d65dd9f3bafa5dcb7da1
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 74%

---

# Google カスタマーマッチを LaunchPoint サービスとして追加 {#add-google-customer-match-as-a-launchpoint-service}

この統合により、Google AdWords を使用してターゲット設定するMarketo EngageオーディエンスをGoogleに送信し、さらにYouTube、検索および Gmail 全体でオーディエンスのリターゲティングをおこなうことができます。

>[!IMPORTANT]
>
>Google Ads API の最近の更新により、AdobeとGoogleの間の同期機能が一時的に無効になっています。  Adobeは、現在、更新に関連するGoogleの要件を確認中です。

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

1. Google AdWords アカウントに接続するには、「****&#x200B;許可」をクリックします。

   ![](assets/authorizeaccount-1.png)

1. Google が新しいタブで開きます。ここから、Google AdWords アカウントにログインします。

   >[!CAUTION]
   >
   >Marketo が複数の AdWords アカウント間でオーディエンスを送信するには、次の手順で承認した Google ユーザが、これらのアカウントの&#x200B;_すべて_&#x200B;にアクセスできる必要があります。

   ![](assets/chooseaccount.png)

1. 要求された権限を確認し、「**[!UICONTROL 許可]**」をクリックします。

   ![](assets/reviewpermissions.png)

1. これで、Google AdWords アカウントが Marketo に接続されました。「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/authorizesuccess.png)

   これで完了です。これで、「インストール済みのサービス」タブに LaunchPoint サービスとして「Google 一致したオーディエンス」が表示されます。

>[!NOTE]
>
>Google カスタマーマッチの統合には、1 つのマネージャーアカウントと、そのマネージャーアカウント内のサブアカウントすべてに対応できます。複数のマネージャーアカウントはサポートされていません。
