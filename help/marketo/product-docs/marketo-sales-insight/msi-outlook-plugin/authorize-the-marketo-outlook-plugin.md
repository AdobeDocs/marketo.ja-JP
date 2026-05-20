---
unique-page-id: 11377640
description: Marketo Outlook プラグインを認証する方法について説明します。 OAuthを完了して、ユーザーがOutlookからメールを送信および追跡できるようにします。
title: Marketo  [!DNL Outlook]  プラグインの認証
exl-id: 4eeed6db-2d28-4ec9-8aa0-1c599f68b2bf
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/IQv2V0dX-p2RE5zfco8s8Q5hSaD35mpQyuWGPpxcITE
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 217
ht-degree: 91%

---

# Marketo [!DNL Outlook] プラグインの認証 {#authorize-the-marketo-outlook-plugin}

[!DNL Outlook] で Marketo MSI プラグインを使用するには、認証する必要があります。

>[!PREREQUISITES]
>
>プラグインが既にインストールされている必要があり、Marketo 管理者によってプラグインユーザとしての認証が必要です。

>[!IMPORTANT]
>
>Microsoft は、[Outlook for Windows の新しいバージョン &#x200B;](https://techcommunity.microsoft.com/t5/outlook-blog/new-outlook-for-windows-now-available/ba-p/3932068){target="_blank"}をリリースしました。 この新しいバージョンは、既存の MSI Outlook プラグインをサポートしていません。 MSI Outlook プラグインは、Outlook のクラシックバージョンを実行している Windows デスクトップで引き続き機能します。 組織向けの新しい Outlook for Windows の詳細については、[こちらをクリック](https://techcommunity.microsoft.com/t5/outlook-blog/the-new-outlook-for-windows-for-organization-admins/ba-p/3929169){target="_blank"}してください。

1. 「Marketo メッセージ」ボタンのいずれかをクリックします。

   ![](assets/image2016-8-24-16-3a4-3a28.png)

1. [!UICONTROL Marketo プラグインを認証]ダイアログが表示されたら、「**[!UICONTROL リクエストコード]**」をクリックします。

   ![](assets/image2016-8-24-16-3a6-3a51.png)

1. コードは、デフォルトの [!DNL Outlook] アカウントのメールアドレスに送信されます。

   ![](assets/image2016-8-24-16-3a8-3a36.png)

1. デフォルトの [!DNL Outlook] アカウントのメールアドレスがチェックアウトされると、登録キーが送信されます。 ポップアップに入力し、「**[!UICONTROL 送信]**」をクリックします。

   ![](assets/image2016-8-24-16-3a12-3a48.png)

   >[!NOTE]
   >
   >登録コードは **14 日後に有効期限が切れます**。

1. メールアドレスが認証されていない場合は、次のメッセージが表示されます。 この問題を解決するには、Marketo 管理者にお問い合わせください。

   ![](assets/image2016-8-24-16-3a25-3a27.png)
