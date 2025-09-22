---
description: セルフビューを防ぐ方法 - Marketo ドキュメント - 製品ドキュメント
title: セルフビューを防ぐ方法
exl-id: 52de102f-6c6c-4663-9725-aae2f620d5bb
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 100%

---

# セルフビューを防ぐには {#how-do-i-prevent-self-views}

ビュートラッキングで偽陽性を取得すると、レポートの不整合が生じる可能性があります。これは、多くの場合、[!DNL Marketo Sales] のユーザが自分のメールクライアントから誤ってトラッキングピクセルを呼び出した場合に発生します（これをセルフビューと呼びます）。以下に、セルフビューを大幅に減らし、さらには削除するヒントを示します。

## Web（[!DNL Outlook] web アプリおよび Gmail） {#web-outlook-web-app-and-gmail}

[!DNL Marketo Sales] は、[!DNL Outlook] web アプリおよび Gmail からメールを開いた際に表示がトラックされないように、ブラウザーに cookie を保存します。まだセルフビューを受け取っている場合は、次の操作をお勧めします。

* お使いのコンピューターで cookie が有効になっていることを確認します。

* 新しいコンピューターまたはモバイルデバイスを使用している場合は、web アプリケーションにログインしていることを確認してください。これにより、お使いのコンピューター／デバイスが今後認識されるようになります。

## デスクトップ（Windows） {#desktop-windows}

ビューは、メールクライアントで小さな非表示の画像ピクセルをダウンロードすることでトラックされます。画像を自動的にダウンロードしないようにすると、[!DNL Outlook] でのセルフビューの量を大幅に減らすことができます。手順を次に示します。

1. Outlook で、「**[!UICONTROL ファイル]**」をクリックします。

   ![](assets/how-do-i-prevent-self-views-1.png)

1. 「**[!UICONTROL オプション]**」をクリックします。

   ![](assets/how-do-i-prevent-self-views-2.png)

1. [!DNL Outlook] のオプションダイアログボックスで、「**[!UICONTROL トラストセンター]**」をクリックします。

   ![](assets/how-do-i-prevent-self-views-3.png)

1. Microsoft [!DNL Outlook] トラストセンターの下で、「**[!UICONTROL トラストセンターの設定]**」をクリックします。

   ![](assets/how-do-i-prevent-self-views-4.png)

1. 左側のメニューで「[!UICONTROL 自動ダウンロード]」をクリックし、「**[!UICONTROL HTML メールや RSS アイテムで画像を自動的にダウンロードしない]**」チェックボックスをオンにします。

   ![](assets/how-do-i-prevent-self-views-5.png)

1. [!UICONTROL Trust Center] ダイアログボックスの「**[!UICONTROL OK]**」をクリックします。

   ![](assets/how-do-i-prevent-self-views-6.png)

1. [!DNL Outlook] のオプションダイアログボックスの「**[!UICONTROL OK]**」をクリックします。

   ![](assets/how-do-i-prevent-self-views-7.png)

## デスクトップ（Mac） {#desktop-mac}

ビューは、メールクライアントで小さな非表示の画像ピクセルをダウンロードすることでトラックされます。画像を自動的にダウンロードしないようにすると、[!DNL Outlook] でのセルフビューの量を大幅に減らすことができます。手順を次に示します。

1. [!DNL Outlook] で、メニューバーの「**[!UICONTROL Outlook]**」をクリックし、「**[!UICONTROL 環境設定]**」を選択します。

   ![](assets/how-do-i-prevent-self-views-8.png)

1. 「[!UICONTROL メール]」で、「**[!UICONTROL 読み上げ]**」を選択します。

   ![](assets/how-do-i-prevent-self-views-9.png)

1. 「[!UICONTROL セキュリティ]」で、「**[!UICONTROL なし]**」ラジオボタンをクリックします。

   ![](assets/how-do-i-prevent-self-views-10.png)
