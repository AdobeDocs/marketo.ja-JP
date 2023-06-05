---
description: Outlook に接続 — Marketoドキュメント — 製品ドキュメント
title: Outlook に連携
source-git-commit: 2538bd5973eb3372352c3ddbada6521911f9fc33
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 58%

---

# Outlook に連携 {#connect-to-outlook}

Sales Insight Actions アカウントを Outlook と連携する方法を説明します。

>[!NOTE]
>
>各ユーザーは、Marketo Sales アカウントから Outlook に接続する必要があります。

## Outlook オンラインへの接続 {#connecting-to-outlook-online}

Outlook に接続すると、返信トラッキング、Outlook 配信チャネルへのアクセス、Outlook でのメールのスケジュール設定、コンプライアンスの送信が可能になります。

1. Marketo Sales で、歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/connect-to-outlook-1.png)

1. マイアカウントで、「**メール設定**」を選択します。

   ![](assets/connect-to-outlook-2.png)

1. 「**メール接続**」タブをクリックします。

   ![](assets/connect-to-outlook-3.png)

1. 「**開始する**」をクリックします。

   ![](assets/connect-to-outlook-4.png)

1. 「**Outlook を使用してメールを送信する**」を選択し、「**次へ**」をクリックします。

   ![](assets/connect-to-outlook-5.png)

1. 使用している Outlook のバージョンを選択し、「**次へ**」をクリックします。この例では、Outlook オンラインを選択しています。

   ![](assets/connect-to-outlook-6.png)

   <table> 
    <tbody>
     <tr>
      <td><strong>Outlook オンライン</strong></td> 
      <td>Exchange オンラインとも呼ばれます</td> 
     </tr>
     <tr>
      <td><strong>Exchange オンプレミス</strong></td> 
      <td>Exchange 2013 および 2016 を含む</td> 
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >現在、Marketo は Exchange Hybrid アカウントをサポートしていません。

1. 「**OK**」をクリックします。

   ![](assets/connect-to-outlook-7.png)

1. Outlook にログインしていない場合は、ログイン情報を入力し、「**次へ**」をクリックします。接続したいアカウントを選択し、 **次へ**. この例では、既にログインしています。

   ![](assets/connect-to-outlook-8.png)

1. 「**確定**」をクリックします。

   ![](assets/connect-to-outlook-9.png)

   この接続を使用してメールをトラッキングし、配信チャネルとしてもトラッキングできます。

   >[!NOTE]
   >
   >Outlook オンライン（Office365）では、独自の送信制限が適用されます。[詳細はこちら](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md#email-provider-limits)を参照してください。

## Exchange オンプレミスへの接続 {#connecting-to-exchange-on-premise}

Exchange オンプレミスに接続すると、返信トラッキング、Outlook 配信チャネルへのアクセス、Outlook でのメールのスケジュール設定、コンプライアンスの送信が可能になります。

1. Marketo Sales で、歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/connect-to-outlook-10.png)

1. マイアカウントで、「**メール設定**」を選択します。

   ![](assets/connect-to-outlook-11.png)

1. 「**メール接続**」タブをクリックします。

   ![](assets/connect-to-outlook-12.png)

1. 「**開始する**」をクリックします。

   ![](assets/connect-to-outlook-13.png)

1. 「**Outlook を使用してメールを送信する**」を選択し、「**次へ**」をクリックします。

   ![](assets/connect-to-outlook-14.png)

1. 使用している Outlook のバージョンを選択し、「**次へ**」をクリックします。この例では、Exchange オンプレミスを選択しています。

   ![](assets/connect-to-outlook-15.png)

   <table> 
    <tbody>
     <tr>
      <td><strong>Outlook オンライン</strong></td> 
      <td>Exchange オンラインとも呼ばれます</td> 
     </tr>
     <tr>
      <td><strong>Exchange オンプレミス</strong></td> 
      <td>Exchange 2013 および 2016 を含む</td> 
     </tr>
    </tbody>
   </table>

1. 資格情報を入力し、「**接続**」をクリックします。

   ![](assets/connect-to-outlook-16.png)

   >[!NOTE]
   >
   >「Exchange のバージョン」ドロップダウンで「自動検出」をオフにした場合は、Exchange の URL を IT 部門に問い合わせる必要があります。

   この接続を使用してメールをトラッキングし、配信チャネルとしてもトラッキングできます。

   >[!NOTE]
   >
   >Exchange オンプレミスを使用する場合、IT チームがメール送信制限を設定します。

## Outlook Online に接続するためのアクセス許可を取得しています {#getting-permission-to-connect-to-outlook-online}

Marketo Sales が Outlook Online アカウント (Microsoft 365) に接続できるよう、IT チームと協力する必要が生じる場合があります。

>[!NOTE]
>
>Microsoft 365 アカウントを管理する IT チームに、アクセスが必要なアプリケーションが「Marketo Sales Connect」であることを伝えます。

IT チームの環境設定と現在の設定に応じて、アクセス権の付与方法について相談することをお勧めします。 会話のガイドに役立つ記事を以下に示します。

* グローバル同意： [Microsoft 365 管理者向けの統合アプリと Azure AD](https://learn.microsoft.com/en-us/microsoft-365/enterprise/integrated-apps-and-azure-ads?view=o365-worldwide){target="_blank"}
* ユーザーの同意： [アプリケーションに対するユーザーの同意方法の設定](https://learn.microsoft.com/en-us/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal&amp;pivots=portal){target="_blank"}
* 管理者の同意： [管理者同意ワークフローの設定](https://learn.microsoft.com/en-us/microsoft-365/admin/misc/user-consent?source=recommendations&amp;view=o365-worldwide){target="_blank"}
* ユーザーの同意をオンまたはオフにする： [Microsoft 365 でのアプリに対するユーザーの同意の管理](https://learn.microsoft.com/en-us/microsoft-365/admin/misc/user-consent?source=recommendations&amp;view=o365-worldwide){target="_blank"}
* Microsoft Defender を使用した管理： [OAuth アプリを管理](https://learn.microsoft.com/en-us/defender-cloud-apps/manage-app-permissions){target="_blank"}
