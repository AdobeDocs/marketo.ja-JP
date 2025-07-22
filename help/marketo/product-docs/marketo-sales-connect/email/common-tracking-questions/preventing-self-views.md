---
unique-page-id: 14352540
description: セルフビューの防止 - Marketo ドキュメント - 製品ドキュメント
title: セルフビューの防止
exl-id: c18715fc-4ca2-4a6b-8f63-a9406f30c0d8
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 51%

---

# セルフビューの防止 {#preventing-self-views}

## 概要 {#overview}

表示のトラッキングに偽陽性があると、レポートの不整合が生じる可能性があります。これは、多くの場合、MSC のユーザーが自分のメールクライアントから誤ってトラッキングピクセルを呼び出した場合に発生します（これをセルフビューと呼びます）。以下に、セルフビューを大幅に減らし、さらには削除するためのいくつかのヒントを示します。

## Web （[!DNL Outlook Web App] および Gmail） {#web-outlook-web-app-and-gmail}

[!DNL Sales Connect] は、Outlook Web App および Gmail から電子メールを開く際にビューが追跡されないように、ブラウザーに Cookie を保存します。 まだセルフビューを受け取っている場合は、次の操作をお勧めします。

* お使いのコンピューターで cookie が有効になっていることを確認します。

* 新しいコンピューターまたはモバイルデバイスを使用している場合は、web アプリケーションにログインしていることを確認してください。これにより、お使いのコンピューター／デバイスが今後認識されるようになります。

## デスクトップ（Windows） {#desktop-windows}

ビューは、メールクライアントで小さな非表示の画像ピクセルをダウンロードすることでトラックされます。自動的にダウンロードされる画像を無効にすることで、[!DNL Outlook] でのセルフビューの量を大幅に減らすことができます。 手順を次に示します。

1. [!DNL Outlook] で、メニューバーの **[!UICONTROL ファイル]** をクリックします。

   ![](assets/win-1.png)

1. 「**[!UICONTROL オプション]**」をクリックします。

   ![](assets/win-2.png)

1. [[!DNL Outlook] のオプション ] ダイアログ ボックスで、[**[!UICONTROL セキュリティ センター]**] をクリックします。

   ![](assets/win-3.png)

1. [[!UICONTROL Microsoft Outlook のセキュリティ センター &#x200B;]] で、[**[!UICONTROL セキュリティ センターの設定]**] をクリックします。

   ![](assets/win-4.png)

1. 左側のメニューの [!UICONTROL &#x200B; 自動ダウンロード &#x200B;] をクリックし、[**[!UICONTROL HTML E メールまたは RSS アイテムの画像を自動的にダウンロードしない]**] チェック ボックスをオンにします。

   ![](assets/win-5.png)

1. **[!UICONTROL セキュリティ センター]** ダイアログ ボックスの [!UICONTROL OK] をクリックします。

   ![](assets/win-6.png)

1. [**[!UICONTROL オプション &#x200B;] ダイアログ ボックスで []** OK[!DNL Outlook]] をクリックします。

   ![](assets/win-6.png)

## デスクトップ（Mac） {#desktop-mac}

ビューは、メールクライアントで小さな非表示の画像ピクセルをダウンロードすることでトラックされます。自動的にダウンロードされる画像を無効にすることで、[!DNL Outlook] でのセルフビューの量を大幅に減らすことができます。 手順を次に示します。

1. [!DNL Outlook] で、メニューバーの **[!UICONTROL Outlook]** をクリックし、**[!UICONTROL 環境設定]** を選択します。

   ![](assets/mac-1.png)

1. [!UICONTROL &#x200B; 電子メール &#x200B;] の下で **[!UICONTROL 読み取り]** を選択します。

   ![](assets/mac-2.png)

1. [!UICONTROL &#x200B; セキュリティ &#x200B;] の下の **[!UICONTROL なし]** ラジオボタンをクリックします。

   ![](assets/mac-3.png)
