---
description: セルフビューを防ぐ方法 — Marketoドキュメント — 製品ドキュメント
title: セルフビューを防ぐ方法
hide: true
hidefromtoc: true
source-git-commit: 3b7cc0c855221f6fd0fba6dca08ccbe361ca9758
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# セルフビューを防ぐ方法 {#how-do-i-prevent-self-views}

ビュートラッキングで偽陽性を取得すると、レポートの不整合が生じる可能性があります。 これは、Marketo Sales のユーザーが誤って電子メールクライアントからトラッキングピクセルを呼び出した場合に発生します（これをセルフビューと呼びます）。 以下に、大幅に減らし、さらにはセルフビューを削除するためのいくつかのヒントを示します。

## Web （Outlook Web App および Gmail） {#web-outlook-web-app-and-gmail}

Marketoセールスは、Outlook Web App および Gmail からメールを開いた際に表示が追跡されないように、ブラウザーに cookie を保存します。 まだセルフビューを受け取っている場合は、次の操作をお勧めします。

* お使いのコンピューターで Cookie が有効になっていることを確認します。

* 新しいコンピューターまたはモバイルデバイスを使用している場合は、Web アプリケーションにログインしていることを確認してください。 これにより、お使いのコンピューター/デバイスが今後認識されるようになります。

## デスクトップ (Windows) {#desktop-windows}

ビューは、電子メールクライアントで小さな非表示の画像ピクセルをダウンロードすることで追跡されます。 画像を自動的にダウンロードしないようにすると、Outlook でのセルフビューの量を大幅に減らすことができます。 手順を次に示します。

1. Outlook で、 **ファイル** をクリックします。

   ![](assets/how-do-i-prevent-self-views-1.png)

1. クリック **オプション**.

   ![](assets/how-do-i-prevent-self-views-2.png)

1. [Outlook のオプション ] ダイアログボックスで、 **トラストセンター**.

   ![](assets/how-do-i-prevent-self-views-3.png)

1. Microsoft Outlook Trust Center で、 **セキュリティセンターの設定**.

   ![](assets/how-do-i-prevent-self-views-4.png)

1. 左側のメニューで「自動ダウンロード」をクリックし、 **HTMLメールや RSS アイテムで画像を自動的にダウンロードしない** チェックボックスをオンにします。

   ![](assets/how-do-i-prevent-self-views-5.png)

1. クリック **OK** をクリックします。

   ![](assets/how-do-i-prevent-self-views-6.png)

1. クリック **OK** [Outlook のオプション ] ダイアログボックスの

   ![](assets/how-do-i-prevent-self-views-7.png)

## デスクトップ (Mac) {#desktop-mac}

ビューは、電子メールクライアントで小さな非表示の画像ピクセルをダウンロードすることで追跡されます。 画像を自動的にダウンロードしないようにすると、Outlook でのセルフビューの量を大幅に減らすことができます。 手順を次に示します。

1. Outlook で、 **Outlook** をクリックし、 **環境設定**.

   ![](assets/how-do-i-prevent-self-views-8.png)

1. 「電子メール」で、を選択します。 **読み上げ**.

   ![](assets/how-do-i-prevent-self-views-9.png)

1. 「セキュリティ」で、 **なし** ラジオボタン。

   ![](assets/how-do-i-prevent-self-views-10.png)
