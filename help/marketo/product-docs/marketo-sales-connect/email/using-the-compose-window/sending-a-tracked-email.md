---
unique-page-id: 37356565
description: Sales Connectでトラッキング対象メールを送信する方法を説明します。 作成ウィンドウから送信し、開封数、クリック数、返信数を追跡します。
title: トラッキングするメールの送信
exl-id: 9a2a53a5-93b9-4254-8540-510c83a6c083
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/TBEuqnKhnaJuZaNivU36NNZJ6cV7-13Stp8SwSdNY78
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 207
ht-degree: 76%

---

# トラッキングするメールの送信 {#sending-a-tracked-email}

[!DNL Marketo Sales Connect] を使用してメールを送信する際に、表示数（メール開封数）とクリック数（クリックされたリンク数）が追跡されます。

>[!PREREQUISITES]
>
>トラッキングするメールを送信する前に、ID を認証し、メール配信チャネルを設定する必要があります。
>
>* [メールアドレスの確認](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md)
>* [[!DNL Outlook]](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) または [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) の配信チャネルの設定

1. メールの下書きを作成します（複数の方法があります。この例では、ヘッダーの「**[!UICONTROL 作成]**」を選択しています）。

   ![](assets/one.png)

1. 受信者の名前またはメールアドレスを「**[!UICONTROL 宛先]**」フィールドに入力します。

   ![](assets/two.png)

   >[!NOTE]
   >
   >「**[!UICONTROL 宛先]**」フィールドに入力できるのは 1 人だけです。

1. CC または BCC を送信する受信者を各フィールドに追加します。

   ![](assets/three.png)

   >[!NOTE]
   >
   >CCまたはBCCのユーザーが電子メールを開くと、その開封率は&#x200B;**[!UICONTROL から]** フィールドのユーザーのレコードにビューとして記録されます。

1. 件名を入力します。

   ![](assets/four.png)

   >[!NOTE]
   >
   >メールの送信には、件名と受信者が必要です。 件名行と受信者が追加されると、**ドラフトが自動的に保存されます**。

1. エディターを使用してメールを作成します。 完了したら、「**[!UICONTROL 送信]**」（または必要に応じて「[スケジュール](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/scheduling-an-email.md)」）をクリックします

   ![](assets/five.png)

   >[!MORELIKETHIS]
   >
   >* [メールのスケジュール設定](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/scheduling-an-email.md)
   >* [テンプレート](/help/marketo/product-docs/marketo-sales-connect/templates/manage-templates.md)
