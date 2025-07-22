---
description: セルフビューを防ぐ方法 - Marketo ドキュメント - 製品ドキュメント
title: セルフビューを防ぐ方法
exl-id: 52de102f-6c6c-4663-9725-aae2f620d5bb
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 48%

---

# セルフビューを防ぐには {#how-do-i-prevent-self-views}

ビュートラッキングで偽陽性を取得すると、レポートの不整合が生じる可能性があります。これは、[!DNL Marketo Sales] のユーザーが誤ってメールクライアントからトラッキングピクセルを呼び出した場合によく発生します（これをセルフビューと呼びます）。 以下に、セルフビューを大幅に減らし、さらには削除するためのいくつかのヒントを示します。

## Web （[!DNL Outlook] Web アプリおよび Gmail） {#web-outlook-web-app-and-gmail}

[!DNL Marketo Sales] は、web アプリや Gmail からメールを開く際にビューが追跡されないように、ブラウザー [!DNL Outlook]cookie を保存します。 まだセルフビューを受け取っている場合は、次の操作をお勧めします。

* お使いのコンピューターで cookie が有効になっていることを確認します。

* 新しいコンピューターまたはモバイルデバイスを使用している場合は、web アプリケーションにログインしていることを確認してください。これにより、お使いのコンピューター／デバイスが今後認識されるようになります。

## デスクトップ（Windows） {#desktop-windows}

ビューは、メールクライアントで小さな非表示の画像ピクセルをダウンロードすることでトラックされます。自動的にダウンロードされる画像を無効にすることで、[!DNL Outlook] でのセルフビューの量を大幅に減らすことができます。 手順を次に示します。

1. Outlook で、「**[!UICONTROL ファイル]**」をクリックします。

   ![](assets/how-do-i-prevent-self-views-1.png)

1. 「**[!UICONTROL オプション]**」をクリックします。

   ![](assets/how-do-i-prevent-self-views-2.png)

1. [[!DNL Outlook] のオプション ] ダイアログ ボックスで、[**[!UICONTROL セキュリティ センター]**] をクリックします。

   ![](assets/how-do-i-prevent-self-views-3.png)

1. Microsoft[!DNL Outlook] セキュリティ センターで、[**[!UICONTROL セキュリティ センターの設定]**] をクリックします。

   ![](assets/how-do-i-prevent-self-views-4.png)

1. 左側のメニューの [!UICONTROL  自動ダウンロード ] をクリックし、[**[!UICONTROL HTML E メールまたは RSS アイテムの画像を自動的にダウンロードしない]**] チェック ボックスをオンにします。

   ![](assets/how-do-i-prevent-self-views-5.png)

1. **[!UICONTROL セキュリティ センター]** ダイアログ ボックスの [!UICONTROL OK] をクリックします。

   ![](assets/how-do-i-prevent-self-views-6.png)

1. [**[!UICONTROL オプション ] ダイアログ ボックスで []** OK[!DNL Outlook]] をクリックします。

   ![](assets/how-do-i-prevent-self-views-7.png)

## デスクトップ（Mac） {#desktop-mac}

ビューは、メールクライアントで小さな非表示の画像ピクセルをダウンロードすることでトラックされます。自動的にダウンロードされる画像を無効にすることで、[!DNL Outlook] でのセルフビューの量を大幅に減らすことができます。 手順を次に示します。

1. [!DNL Outlook] で、メニューバーの **[!UICONTROL Outlook]** をクリックし、**[!UICONTROL 環境設定]** を選択します。

   ![](assets/how-do-i-prevent-self-views-8.png)

1. [!UICONTROL  電子メール ] の下で **[!UICONTROL 読み取り]** を選択します。

   ![](assets/how-do-i-prevent-self-views-9.png)

1. [!UICONTROL  セキュリティ ] の下の **[!UICONTROL なし]** ラジオボタンをクリックします。

   ![](assets/how-do-i-prevent-self-views-10.png)
