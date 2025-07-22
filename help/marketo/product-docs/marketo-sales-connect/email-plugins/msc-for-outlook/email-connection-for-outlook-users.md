---
unique-page-id: 17727591
description: Outlook ユーザーのメール接続 - Marketo ドキュメント - 製品ドキュメント
title: Outlook ユーザーのメール接続
exl-id: e694915c-39a6-4476-a643-080acb758de7
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 39%

---

# [!DNL Outlook] ユーザー用の E メール接続 {#email-connection-for-outlook-users}

[!DNL Sales Connect] アカウントを [!DNL Outlook] に接続する方法を説明します。

>[!NOTE]
>
>各ユーザーは、[!DNL Outlook] アカウントから [!DNL Sales Connect] に接続する必要があります。

## [!DNL Outlook] Online への接続 {#connecting-to-outlook-online}

[!DNL Outlook] に接続すると、返信トラッキングの受信、[!DNL Outlook] 配信チャネルへのアクセス、[!DNL Outlook] でのメールのスケジュール設定、コンプライアンスの送信ができるようになります。

1. [!DNL Sales Connect] で、歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/one.png)

1. マイアカウントで、「**[!UICONTROL メール設定]**」を選択します。

   ![](assets/two.png)

1. 「**[!UICONTROL メール接続]**」タブをクリックします。

   ![](assets/three.png)

1. 「**[!UICONTROL 開始する]**」をクリックします。

   ![](assets/four.png)

1. 「**[!UICONTROL Outlook を使用してメールを送信する]**」を選択し、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/five-a.png)

1. 使用している [!DNL Outlook] のバージョンを選択し、「**[!UICONTROL 次へ]**」をクリックします。 この例では、「[!DNL Outlook Online]」を選択します。

   ![](assets/six-a.png)

   <table> 
    <tbody>
     <tr>
      <td><strong>[!DNL Outlook Online]</strong></td> 
      <td>別名 [!DNL Exchange Online]</td> 
     </tr>
     <tr>
      <td><strong>[!DNL Exchange On-premise]</strong></td> 
      <td>[!DNL Exchange] 2013 および 2016 を含む</td> 
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >現時点では、Marketoは [!DNL Exchange Hybrid] アカウントをサポートしていません。

1. 「**[!UICONTROL OK]**」をクリックします。

   ![](assets/seven-a.png)

1. [!DNL Outlook] にログインしていない場合は、ログイン情報を入力して [**[!UICONTROL 次へ]**] をクリックします。 接続したいアカウントを選択し、「**[!UICONTROL 次へ]**」をクリックします。この例では、既にログインしています。

   ![](assets/eight-a.png)

1. 「**[!UICONTROL 確定]**」をクリックします。

   ![](assets/nine-a.png)

   この接続を使用してメールをトラッキングし、配信チャネルとしてもトラッキングできます。

   >[!NOTE]
   >
   >[!DNL Outlook Online (Office365)] では、独自の送信制限を適用します。 詳しくは、[こちらを参照](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md#email-provider-limits)してください。

## [!DNL Exchange On-Premise] への接続  {#connecting-to-exchange-on-premise}

[!DNL Exchange On-Premise] に接続すると、返信トラッキングの受信、[!DNL Outlook] 配信チャネルへのアクセス、[!DNL Outlook] でのメールのスケジュール設定、コンプライアンスの送信ができるようになります。

1. [!DNL Sales Connect] で、歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/one.png)

1. [!UICONTROL  マイアカウント ] で **[!UICONTROL メール設定]** を選択します。

   ![](assets/two.png)

1. 「**[!UICONTROL メール接続]**」タブをクリックします。

   ![](assets/three.png)

1. 「**[!UICONTROL 開始する]**」をクリックします。

   ![](assets/four.png)

1. 「**[!UICONTROL Outlook を使用してメールを送信する]**」を選択し、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/five-a.png)

1. 使用している [!DNL Outlook] のバージョンを選択し、「**[!UICONTROL 次へ]**」をクリックします。 この例では、「[!DNL Exchange On-premise]」を選択します。

   ![](assets/six-b.png)

   <table> 
    <tbody>
     <tr>
      <td><strong>[!DNL Outlook Online]</strong></td> 
      <td>別名 [!DNL Exchange Online]</td> 
     </tr>
     <tr>
      <td><strong>[!DNL Exchange On-premise]</strong></td> 
      <td>[!DNL Exchange] 2013 および 2016 を含む</td> 
     </tr>
    </tbody>
   </table>

1. 資格情報を入力し、「**[!UICONTROL 接続]**」をクリックします。

   ![](assets/seven-b.png)

   >[!NOTE]
   >
   >[[!DNL Exchange] Version] ドロップダウンで [Autodiscover] をオフにした場合は、IT 部門に [!DNL Exchange] の URL を問い合わせる必要があります。

   この接続を使用してメールをトラッキングし、配信チャネルとしてもトラッキングできます。

   >[!NOTE]
   >
   >[!DNL Exchange On-prem] を使用する場合、IT チームはメール送信制限を確立します。
