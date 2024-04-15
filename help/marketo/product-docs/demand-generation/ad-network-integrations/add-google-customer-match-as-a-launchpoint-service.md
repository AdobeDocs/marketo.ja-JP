---
unique-page-id: 12980661
description: Google カスタマーマッチを LaunchPoint サービスとして追加 - Marketo ドキュメント - 製品ドキュメント
title: Google カスタマーマッチを LaunchPoint サービスとして追加
exl-id: c780bde0-3044-4c89-a2ac-88398cbc3425
feature: Integrations
source-git-commit: 136707304350be59918716233f5d6e2a6438be4e
workflow-type: ht
source-wordcount: '226'
ht-degree: 100%

---

# Google カスタマーマッチを LaunchPoint サービスとして追加 {#add-google-customer-match-as-a-launchpoint-service}

この統合により、Marketo Engage オーディエンスを Google に送信し、Google AdWords を使用してターゲットを設定したり、YouTube、検索、Gmail 全体でオーディエンスを再ターゲットしたりすることができます。

>[!IMPORTANT]
>
>Google Ads API の最近のアップデートにより、アドビと Google の間の同期機能が一時的に無効になっています。アドビは、現在、このアップデートに関連する Google の要件を確認中です。

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
