---
unique-page-id: 14352540
description: セルフビューの防止 - Marketo ドキュメント - 製品ドキュメント
title: セルフビューの防止
exl-id: c18715fc-4ca2-4a6b-8f63-a9406f30c0d8
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 100%

---

# セルフビューの防止 {#preventing-self-views}

## 概要 {#overview}

表示のトラッキングに偽陽性があると、レポートの不整合が生じる可能性があります。これは、多くの場合、MSC のユーザーが自分のメールクライアントから誤ってトラッキングピクセルを呼び出した場合に発生します（これをセルフビューと呼びます）。以下に、セルフビューを大幅に減らし、さらには削除するヒントを示します。

## Web（[!DNL Outlook Web App] および Gmail） {#web-outlook-web-app-and-gmail}

[!DNL Sales Connect] は、Outlook Web App および Gmail からメールを開く際に表示が追跡されないように、ブラウザーに cookie を保存します。まだセルフビューを受け取っている場合は、次の操作をお勧めします。

* お使いのコンピューターで cookie が有効になっていることを確認します。

* 新しいコンピューターまたはモバイルデバイスを使用している場合は、web アプリケーションにログインしていることを確認してください。これにより、お使いのコンピューター／デバイスが今後認識されるようになります。

## デスクトップ（Windows） {#desktop-windows}

ビューは、メールクライアントで小さな非表示の画像ピクセルをダウンロードすることでトラックされます。画像を自動的にダウンロードしないようにすると、[!DNL Outlook] でのセルフビューの量を大幅に減らすことができます。手順を次に示します。

1. [!DNL Outlook] のメニューバーで「**[!UICONTROL ファイル]**」をクリックします。

   ![](assets/win-1.png)

1. 「**[!UICONTROL オプション]**」をクリックします。

   ![](assets/win-2.png)

1. [!DNL Outlook] のオプションダイアログボックスで、「**[!UICONTROL Trust Center]**」をクリックします。

   ![](assets/win-3.png)

1. [!UICONTROL Microsoft Outlook Trust Center] で、「**[!UICONTROL Trust Center の設定]**」をクリックします。

   ![](assets/win-4.png)

1. 左側のメニューで「[!UICONTROL 自動ダウンロード]」をクリックし、「**[!UICONTROL HTML メールや RSS アイテムで画像を自動的にダウンロードしない]**」チェックボックスをオンにします。

   ![](assets/win-5.png)

1. [!UICONTROL Trust Center] ダイアログボックスの「**[!UICONTROL OK]**」をクリックします。

   ![](assets/win-6.png)

1. [!DNL Outlook] のオプションダイアログボックスの「**[!UICONTROL OK]**」をクリックします。

   ![](assets/win-6.png)

## デスクトップ（Mac） {#desktop-mac}

ビューは、メールクライアントで小さな非表示の画像ピクセルをダウンロードすることでトラックされます。画像を自動的にダウンロードしないようにすると、[!DNL Outlook] でのセルフビューの量を大幅に減らすことができます。手順を次に示します。

1. [!DNL Outlook] で、メニューバーの「**[!UICONTROL Outlook]**」をクリックし、「**[!UICONTROL 環境設定]**」を選択します。

   ![](assets/mac-1.png)

1. 「[!UICONTROL メール]」で、「**[!UICONTROL 読み上げ]**」を選択します。

   ![](assets/mac-2.png)

1. 「[!UICONTROL セキュリティ]」で、「**[!UICONTROL なし]**」ラジオボタンをクリックします。

   ![](assets/mac-3.png)
