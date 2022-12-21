---
unique-page-id: 15695874
description: BrightTALK の Marketo 接続 - Marketo ドキュメント - 製品ドキュメント
title: BrightTALK の Marketo 接続
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 100%

---

# BrightTALK の Marketo 接続 {#connect-brighttalk-to-marketo}

BrightTALK チャネルを Marketo インスタンスに接続する方法を説明します。これを行うには、両方の管理者である必要があります。

>[!NOTE]
>
>**管理者権限が必要**

## BrightTALK での手順 {#steps-in-brighttalk}

1. [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target=&quot;_blank&quot;} にログインし、「**今すぐ接続**」をクリックします。
1. 「Marketo コネクタの詳細設定」で、「**接続**」をクリックします。
1. 資格情報画面が表示され、次の情報が求められます。クライアント ID、クライアントシークレット、ID サービス URL、REST サービス URL。この情報を取得するには、Marketo にログインします。

## Marketo での手順 {#steps-in-marketo}

>[!NOTE]
>
>この時点で、BrightTALK が Marketo インスタンスに持つ権限を制限するために、API のみのユーザロールと API 専用ユーザを設定する必要があります。これらの手順に関する記事が既にあり、以下が記事のリンクです。

1. [API 専用ユーザロールを作成する](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target=&quot;_blank&quot;}。

1. 手順 4 で作成した BrightTALK API のロールを使用して、[API ユーザを作成](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target=&quot;_blank&quot;}します。

1. 管理領域に戻ります。

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. 「統合」で、「**LaunchPoint**」をクリックします。

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. 「**新規**」ドロップダウンをクリックして、「**新規サービス**」を選択します。

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. 任意の表示名を入力します。「サービス」ドロップダウンをクリックし、「**カスタム**」を選択します（BrightTALK は&#x200B;_選択しません_）。

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >ドロップダウンの「BrightTALK」は選択しないでください。これは削除中のフィールドで、選択すると、Marketo／BrightTALK 統合に重大な問題が発生する可能性があります。

1. 任意の「説明」を入力します。「API のみのユーザ」ドロップダウンをクリックし、手順 5 で作成した BrightTALK API ユーザを選択します。「**作成**」をクリックします。

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. 先ほど作成したカスタムサービスの「**詳細を表示**」をクリックします。

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. **クライアント ID** および&#x200B;**クライアントシークレット**&#x200B;をコピー（および保存）します。「**閉じる**」をクリックします。

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. 「統合」で、「**Web サービス**」を選択します。

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. Rest API で、**エンドポイント**&#x200B;および **ID** をコピー（および保存）します。

   ![](assets/connect-brighttalk-to-marketo-9.png)

## BrightTALK での追加手順 {#additional-steps-in-brighttalk}

1. 手順 3 の BrightTALK コネクタの設定画面に戻り、手順 12 および 14 で保存した資格情報を入力します。

   資格情報が認証されたら、BrightTALK が Marketo に正式に接続されます。次の手順では、[同期するデータフィールド](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync){target=&quot;_blank&quot;}を定義します。
