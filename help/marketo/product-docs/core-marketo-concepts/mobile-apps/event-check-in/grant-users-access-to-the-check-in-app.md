---
unique-page-id: 7516639
description: イベントチェックインアプリへのアクセス権をユーザーに付与する方法について説明します。 参加者をチェックインできるように、モバイルイベントチェックインの役割を割り当てます。
title: チェックインアプリに対するアクセス権をユーザーに付与する
exl-id: 898ac49f-a708-4cdf-b341-58582740a45b
feature: Mobile Marketing
TQID: 'https://experienceleague.adobe.com/GKLCTK-Wc-rwTfbcNIEzferpYBJDvpKjelUm5-89WIU'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: 44b89f75-c1af-5353-8094-79b278102d46
    internal-label: Mobile Marketing
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 79%
---
# チェックインアプリに対するアクセス権をユーザーに付与する {#grant-users-access-to-the-check-in-app}

Marketo Engage には、イベントチェックインアプリ用の特別なユーザロールがあります。 次の手順に従って、アプリを使用する権限を持つ新しい役割を作成します。

>[!IMPORTANT]
>
>2023年10月2日（PT）に、アドビは Marketo イベントアプリをすべてのアプリストアから削除しました。 タブレット／モバイルデバイスにアプリが既にインストールされている場合は、当面は引き続き使用できます。 Marketo Engage インスタンスが、Marketo の認証に Adobe Identity を使用するように移行されると、アプリにアクセスできなくなります。 [詳細情報](https://nation.marketo.com/t5/product-discussions/marketo-events-app-and-marketo-moments-app-end-of-life/m-p/340712/highlight/true#M193869){target="_blank"}。

## モバイル用の新しいユーザーロールを作成する {#create-a-new-user-role-for-mobile}

1. 「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/image2015-6-2-10-3a39-3a31.png)

1. 「**[!UICONTROL ユーザーと役割]**」をクリックします。

   ![](assets/image2015-6-2-10-3a56-3a0.png)

1. 「**[!UICONTROL 役割]**」タブをクリックし、「**[!UICONTROL 新しい役割]**」をクリックします。

   ![](assets/image2015-6-2-11-3a3-3a23.png)

1. 新しいロールの名前と説明（オプション）を入力します。 「**[!UICONTROL モバイルアプリケーションにアクセス]**」ボックスをオンにして、「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/image2015-6-2-11-3a4-3a58.png)

   タブレットアプリにユーザを招待できるようになると、新しいロールを割り当てる準備が整います。

## チェックインアプリ用の新しいユーザを招待する {#invite-new-users-for-the-check-in-app}

1. 「**[!UICONTROL ユーザー]**」タブをクリックします。

   ![](assets/image2015-6-2-11-3a10-3a42.png)

1. 「**[!UICONTROL 新しいユーザーを招待]**」をクリックします。

   ![](assets/image2015-6-2-11-3a11-3a32.png)

1. 新しいユーザーの情報を入力します。 すべての適切なロールのチェックボックスと、モバイルアプリへのアクセス権限を持つ新しいロールを選択します。 完了したら、**[!UICONTROL 招待]**&#x200B;をクリックします。

   ![](assets/image2015-6-2-11-3a16-3a26.png)

   >[!CAUTION]
   >
   >データベースにアクセスできないユーザーは、アプリ内の人物を表示できません。

   >[!TIP]
   >
   >既存のユーザの場合は、新しいロールを作成するか、現在のロールに[!UICONTROL モバイルアプリケーションへのアクセス]権限を追加できます。

ユーザーには、チェックインアプリへのアクセス権を持っていることを知らせるメールが届きます。
