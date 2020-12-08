---
unique-page-id: 14746470
description: 配信チャネルの設定 — Marketto Docs — 製品ドキュメント
title: 配信チャネルの設定
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---


# 配信チャネルの設定 {#setting-up-your-delivery-channel}

Marketo Sales Connectを使用して開始を行う場合、電子メールを送信するには、SMTPサーバーを設定する必要があります。

>[!NOTE]
>
>SMTPサーバーを設定するだけでなく、電子メールを送信する前に [電子メールIDを確認する必要があります](http://docs.marketo.com/x/ewPh) 。

カスタムSMTPサーバー、チームSMTPサーバー、またはGmailを配信チャネルとして使用して電子メールを送信するよう選択できます。 選択肢を一つ一つ見てみましょう。

## カスタムSMTP {#custom-smtp}

1. [Webアプリケーションにログインし](http://toutapp.com/login)、右上の歯車アイコンをクリックして、「 **設定**」を選択します。

   ![](assets/one.png)

1. 「マイアカウント」で、「 **電子メール設定**」をクリックします。

   ![](assets/two.png)

1. 「 **SMTP Server**」を選択します。

   ![](assets/three.png)

1. SMTP Serverの資格情報を入力し、「 **Connect**」をクリックします。

   ![](assets/four.png)

   >[!NOTE]
   >
   >これが唯一の配信チャネルの場合は、すべての電子メールIDに自動的に割り当てられ、ここで処理が完了します。 これが配信チャネル以外の場合は、手順5に進んでください。

1. 「電子メールの設定」に進んだまま、「 **アドレスと署名**」をクリックします。

   ![](assets/five.png)

1. 配信チャネルを選択する電子メールIDを探し、「配信チャネルを **選択**」をクリックします。

   ![](assets/six.png)

1. 「Deliverability Card」で、「 **Edit**」をクリックします。

   ![](assets/seven-new.png)

1. 「チャネル」ドロップダウンをクリックし、先ほど追加したカスタム配信チャネルを選択します。 「 **保存**」をクリックします。

   ![](assets/eight-new.png)

   >[!NOTE]
   >
   >チーム管理者がチームSMTPサーバーを設定すると、そのサーバーは自動的にデフォルトの電子メールIDにのみ適用され、他の電子メールIDのオプションとして使用できます。

   **ビデオの視聴**`<iframe width="630" height="470" src="//play.vidyard.com/YWKSgZvBEjUU8FrXZ5hdYR.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`

## チームSMTPサーバー {#team-smtp-server}

>[!NOTE]
>
>**必要な管理者権限**

1. [Webアプリケーションにログインし](http://toutapp.com/login)、右上の歯車アイコンをクリックして、「 **設定**」を選択します。

   ![](assets/nine.png)

1. 「管理者の設定」で、「 **チームSMTPサーバー**」をクリックします。

   ![](assets/ten.png)

1. SMTP Serverの資格情報を入力し、「 **Connect**」をクリックします。

   ![](assets/eleven.png)

   >[!NOTE]
   >
   >チームSMTPサーバーは、すべてのチームメンバーの既定の電子メールIDの既定の配信チャネルです。 さらに、他のすべての電子メールIDの配信チャネルオプションとしても使用できます。

   **ビデオを見る**`<iframe width="630" height="470" src="//play.vidyard.com/Ky9EwGmLcgvsMpFq3H8Y6n.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`

## Gmail {#gmail}

1. [Webアプリケーションにログインし](http://toutapp.com/login)、右上の歯車アイコンをクリックして、「 **設定**」を選択します。

   ![](assets/twelve.png)

1. 「マイアカウント」で、「 **電子メール設定**」をクリックします。

   ![](assets/thirteen.png)

1. 「 **電子メールの同期**」をクリックします。

   ![](assets/fourteen.png)

1. 「Google **に接続**」をクリックします。

   ![](assets/fifteen.png)

1. Googleの資格情報を使用してサインインします。
1. この画面が表示されたら、「 **許可**」をクリックします。

   ![](assets/sixteen.png)

   >[!NOTE]
   >
   >これが唯一の配信チャネルの場合は、すべての電子メールIDに自動的に割り当てられ、ここで処理が完了します。 配信チャネルがGmailだけでない場合は、手順7に進んでください。

1. 「 **アドレスと署名**」をクリックします。

   ![](assets/seventeen.png)

1. Gmailを配信チャネルにする電子メールIDをクリックします。

   ![](assets/eighteen.png)

1. スライドパネルが開いたら、「Deliverability Card」まで下にスクロールします。

   ![](assets/nineteen.png)

1. 「チャネル」ドロップダウンをクリックし、先ほど追加したGmail配信チャネルを選択します。 「 **保存**」をクリックします。

   ![](assets/twenty.png)

   >[!NOTE]
   >
   >チーム管理者がチームSMTPサーバーを設定すると、そのサーバーは自動的にデフォルトの電子メールIDにのみ適用され、他の電子メールIDのオプションとして使用できます。

