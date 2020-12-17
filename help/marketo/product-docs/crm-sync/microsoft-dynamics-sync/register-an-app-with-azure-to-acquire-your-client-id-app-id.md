---
unique-page-id: 12983390
description: Azureにアプリを登録して、クライアントID/アプリIDを取得します — Marketto Docs — 製品ドキュメント
title: Azureにアプリを登録して、クライアントID/アプリIDを取得する
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---


# Azureにアプリを登録して、クライアントID/アプリID {#register-an-app-with-azure-to-acquire-your-client-id-app-id}を取得します

Azure Active Directoryは、オンプレミスのディレクトリをクラウドに拡張し、オンプレミスのADFS認証でMS Dynamics 365 CRMをサポートします。

## 新しいアプリの登録{#registering-a-new-app}

1. [管理者権限を持つアカウント](http://manage.windowsazure.com/) を使用してMicrosoft Azure管理ポータルにログインします。Office 365 Admin Centerを通じてMicrosoft Azureポータルにアクセスするには、左側のナビゲーションウィンドウで&#x200B;**管理者**&#x200B;項目を展開し、**Azure AD**&#x200B;を選択します。

   >[!CAUTION]
   >
   >アプリの登録先と同じOffice 365購読のアカウントを使用する必要があります。

   >[!NOTE]
   >
   >Azureアカウントをお持ちでない場合は、[サインアップ](https://azure.microsoft.com/en-us/free/)をお持ちの方にお願いします。 詳細については、Microsoftのドキュメントを参照するか、Microsoftの担当者にお問い合わせください。 Azureアカウントを作成したら、以下に説明する手順を使用して1つ以上のアプリを登録できます。
   >
   >
   >Azureアカウントをお持ちで、Microsoft Dynamics 365とのOffice 365購読がAzure購読で使用できない場合は、[次の手順](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription)に従って、2つのアカウントを関連付けます。

1. 左側のナビゲーションウィンドウで、**Azure Active Directory**&#x200B;を探してクリックします。

   ![](assets/two.png)

1. 「管理」で、「**アプリ登録**」をクリックします。

   ![](assets/three.png)

1. ページ上部の「**新規登録**」をクリックします。

   ![](assets/four.png)

1. アプリの名前を入力し、該当するアカウントタイプを選択して、リダイレクトURLを入力します。 次に、ページの下部にある「**登録**」をクリックします。

   ![](assets/five.png)

1. これで、「**アプリ登録**」タブにアプリが表示されます。

   ![](assets/six.png)

## アプリの権限の設定{#configuring-app-permissions}

1. Active Directoryの「**アプリ登録**」タブで、権限を設定するアプリをクリックします。

   ![](assets/seven.png)

1. 「管理」で、「**API権限**」をクリックします。

   ![](assets/eight.png)

1. **権限追加**&#x200B;ボタンをクリックします。

   ![](assets/nine.png)

1. **Dynamics CRM**&#x200B;を選択します。

   ![](assets/ten.png)

1. 「**Access Common Data Service as organization user***s**」ボックスをオンにし、「**追加権限」をクリックします。**

   ![](assets/eleven.png)

1. 権限が正常に追加されたら、少なくとも10秒待ちます。

   ![](assets/twelve.png)

1. 「**管理者の同意を許可**」ボタンをクリックします。

   ![](assets/thirteen.png)

1. 「**はい**」をクリックして確認します。

   ![](assets/fourteen.png)

   終わった！

   ![](assets/fifteen.png)

