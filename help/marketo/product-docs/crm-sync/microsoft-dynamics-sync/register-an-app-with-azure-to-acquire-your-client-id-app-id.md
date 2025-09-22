---
unique-page-id: 12983390
description: アプリを Azure に登録してクライアント ID／アプリ ID を取得 - Marketo ドキュメント - 製品ドキュメント
title: アプリを Azure に登録してクライアント ID／アプリ ID を取得
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 100%

---

# アプリを Azure に登録してクライアント ID／アプリ ID を取得 {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory は、オンプレミスのディレクトリをクラウドに拡張し、オンプレミスの ADFS 認証を備えた [!DNL MS Dynamics 365] CRM をサポートします。

## 新しいアプリの登録 {#registering-a-new-app}

1. 管理権限を持つアカウントを使用して、Microsoft Azure 管理ポータルに[ログイン](https://login.microsoftonline.com/){target="_blank"}します。また、左側のナビゲーションパネルの「**[!UICONTROL 管理者]**」項目を展開し、「**[!UICONTROL Azure AD]**」を選択して、Office 365 Admin Center から Microsoft Azure ポータルにアクセスすることもできます。

   >[!CAUTION]
   >
   >アプリの登録先と同じ [!DNL Office 365] サブスクリプションのアカウントを使用する必要があります。

   >[!NOTE]
   >
   >Azure アカウントをお持ちでない場合は、[新規登録](https://azure.microsoft.com/ja-jp/free/){target="_blank"}できます。詳しくは、Microsoft のドキュメントを参照するか、Microsoft の担当者にお問い合わせください。Azure アカウントを作成したら、以下の手順を使用して 1 つ以上のアプリを登録できます。
   >
   >
   >Azure アカウントがあっても、[!DNL Microsoft Dynamics 365] を使用した [!DNL Office 365] サブスクリプションが Azure サブスクリプションで利用できない場合は、[こちらの手順](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription){target="_blank"}に従って、2 つのアカウントを関連付けます。

1. 左側のナビゲーションパネルで、「**[!UICONTROL Azure Active Directory]**」を検索してクリックします。

   ![](assets/two.png)

1. 「[!UICONTROL 管理]」で、「**[!UICONTROL アプリの登録]**」をクリックします。

   ![](assets/three.png)

1. ページの上部にある「**[!UICONTROL 新規登録]**」をクリックします。

   ![](assets/four.png)

1. アプリ名を入力し、適切なアカウントタイプを選択して、リダイレクト URL を入力します。次に、ページの下部にある「**[!UICONTROL 登録]**」をクリックします。

   ![](assets/five.png)

1. これで、アプリが「**[!UICONTROL アプリの登録]**」タブに表示されます。

   ![](assets/six.png)

## アプリの権限の設定 {#configuring-app-permissions}

1. Active Directory の「**[!UICONTROL アプリの登録]**」タブで、権限を設定するアプリをクリックします。

   ![](assets/seven.png)

1. 「[!UICONTROL 管理]」で、「**[!UICONTROL API 権限]**」をクリックします。

   ![](assets/eight.png)

1. 「**[!UICONTROL 権限を追加]**」ボタンをクリックします。

   ![](assets/nine.png)

1. 「**[!UICONTROL Dynamics CRM]**」を選択します。

   ![](assets/ten.png)

1. 「**[!UICONTROL 組織ユーザとして共通データサービスにアクセスする]**」チェックボックスにチェックを入れ、「**[!UICONTROL 権限を追加]」をクリックします。**

   ![](assets/eleven.png)

1. 権限が正常に追加されたら、少なくとも 10 秒待ちます。

   ![](assets/twelve.png)

1. 「**[!UICONTROL 管理者の同意を付与]**」ボタンをクリックします。

   ![](assets/thirteen.png)

1. 「**[!UICONTROL はい]**」をクリックして確認します。

   ![](assets/fourteen.png)

   これで完了です。

   ![](assets/fifteen.png)
