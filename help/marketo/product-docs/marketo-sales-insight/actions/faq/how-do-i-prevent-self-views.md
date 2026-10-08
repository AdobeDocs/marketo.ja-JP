---
description: 電子メールトラッキングでセルフビューがカウントされないようにする方法について説明します。 独自の電子メールを表示する際に、開封数を増やさないようにしましょう。
title: セルフビューを防ぐ方法
exl-id: 52de102f-6c6c-4663-9725-aae2f620d5bb
feature: Sales Insight Actions
TQID: 'https://experienceleague.adobe.com/6AN3CB0CoDTRPBerpKPzg94dpsvbsk5-r-DRhdePvMo'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
    internal-label: Reporting
  - id: 412786a7-b8da-5b9d-8c3f-2539a3faad9f
    internal-label: Sales Insight Actions
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 87%
---
# セルフビューを防ぐには {#how-do-i-prevent-self-views}

ビュートラッキングで偽陽性を取得すると、レポートの不整合が生じる可能性があります。 これは、多くの場合、[!DNL Marketo Sales] のユーザが自分のメールクライアントから誤ってトラッキングピクセルを呼び出した場合に発生します（これをセルフビューと呼びます）。 以下に、セルフビューを大幅に減らし、さらには削除するヒントを示します。

## Web（[!DNL Outlook] web アプリおよび Gmail） {#web-outlook-web-app-and-gmail}

[!DNL Marketo Sales] は、[!DNL Outlook] web アプリおよび Gmail からメールを開いた際に表示がトラックされないように、ブラウザーに cookie を保存します。 まだセルフビューを受け取っている場合は、次の操作をお勧めします。

* お使いのコンピューターで cookie が有効になっていることを確認します。

* 新しいコンピューターまたはモバイルデバイスを使用している場合は、Web アプリケーションにログインしていることを確認してください。 これにより、お使いのコンピューター／デバイスが今後認識されるようになります。

## デスクトップ（Windows） {#desktop-windows}

メールクライアントで小さな非表示の画像ピクセルをダウンロードすることで、開封がトラッキングされます。 画像を自動的にダウンロードしないようにすると、[!DNL Outlook] でのセルフビューの量を大幅に減らすことができます。 手順を次に示します。

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

メールクライアントで小さな非表示の画像ピクセルをダウンロードすることで、開封がトラッキングされます。 画像を自動的にダウンロードしないようにすると、[!DNL Outlook] でのセルフビューの量を大幅に減らすことができます。 手順を次に示します。

1. [!DNL Outlook] で、メニューバーの「**[!UICONTROL Outlook]**」をクリックし、「**[!UICONTROL 環境設定]**」を選択します。

   ![](assets/how-do-i-prevent-self-views-8.png)

1. 「[!UICONTROL メール]」で、「**[!UICONTROL 読み上げ]**」を選択します。

   ![](assets/how-do-i-prevent-self-views-9.png)

1. 「[!UICONTROL セキュリティ]」で、「**[!UICONTROL なし]**」ラジオボタンをクリックします。

   ![](assets/how-do-i-prevent-self-views-10.png)
