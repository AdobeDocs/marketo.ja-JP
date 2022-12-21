---
description: セルフビューを防ぐ方法 - Marketo ドキュメント - 製品ドキュメント
title: セルフビューを防ぐ方法
exl-id: 52de102f-6c6c-4663-9725-aae2f620d5bb
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 100%

---

# セルフビューを防ぐには {#how-do-i-prevent-self-views}

ビュートラッキングで偽陽性を取得すると、レポートの不整合が生じる可能性があります。これは、Marketo Sales のユーザが誤ってメールクライアントからトラッキングピクセルを呼び出した場合に発生します（これをセルフビューと呼びます）。以下に、セルフビューを大幅に減らし、さらには削除するためのいくつかのヒントを示します。

## Web（Outlook web アプリおよび Gmail） {#web-outlook-web-app-and-gmail}

Marketo Sales は、Outlook web アプリおよび Gmail からメールを開いた際に表示がトラックされないように、ブラウザーに cookie を保存します。まだセルフビューを受け取っている場合は、次の操作をお勧めします。

* お使いのコンピューターで cookie が有効になっていることを確認します。

* 新しいコンピューターまたはモバイルデバイスを使用している場合は、web アプリケーションにログインしていることを確認してください。これにより、お使いのコンピューター／デバイスが今後認識されるようになります。

## デスクトップ（Windows） {#desktop-windows}

ビューは、メールクライアントで小さな非表示の画像ピクセルをダウンロードすることでトラックされます。画像を自動的にダウンロードしないようにすると、Outlook でのセルフビューの量を大幅に減らすことができます。手順を次に示します。

1. Outlook で、「**ファイル**」をクリックします。

   ![](assets/how-do-i-prevent-self-views-1.png)

1. 「**オプション**」をクリックします。

   ![](assets/how-do-i-prevent-self-views-2.png)

1. Outlook のオプションダイアログボックスで、「**トラストセンター**」をクリックします。

   ![](assets/how-do-i-prevent-self-views-3.png)

1. Microsoft Outlook トラストセンターで、「**セキュリティセンターの設定**」をクリックします。

   ![](assets/how-do-i-prevent-self-views-4.png)

1. 左側のメニューで「自動ダウンロード」をクリックし、「**HTML メールや RSS アイテムで画像を自動的にダウンロードしない**」チェックボックスをオンにします。

   ![](assets/how-do-i-prevent-self-views-5.png)

1. トラストセンターダイアログボックスの「**OK**」をクリックします。

   ![](assets/how-do-i-prevent-self-views-6.png)

1. Outlook のオプションダイアログボックスの「**OK**」をクリックします。

   ![](assets/how-do-i-prevent-self-views-7.png)

## デスクトップ（Mac） {#desktop-mac}

ビューは、メールクライアントで小さな非表示の画像ピクセルをダウンロードすることでトラックされます。画像を自動的にダウンロードしないようにすると、Outlook でのセルフビューの量を大幅に減らすことができます。手順を次に示します。

1. Outlook で、メニューバーの **Outlook** をクリックし、「**環境設定**」を選択します。

   ![](assets/how-do-i-prevent-self-views-8.png)

1. 「電子メール」で、「**閲覧**」を選択します。

   ![](assets/how-do-i-prevent-self-views-9.png)

1. 「セキュリティ」で、「**なし**」ラジオボタンをクリックします。

   ![](assets/how-do-i-prevent-self-views-10.png)
