---
unique-page-id: 4719302
description: 英語以外のカスタムオブジェクトの同期を有効にする — Marketto Docs — 製品ドキュメント
title: 英語以外のカスタムオブジェクトの同期を有効にする
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# 英語以外のカスタムオブジェクトの同期を有効にする {#enable-non-english-custom-object-sync}

Marketoの同期ユーザーが英語以外の言語に設定されている場合、カスタムオブジェクトの同期を有効にしようとするとエラーが発生する場合があります。

## エラー {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## 取り組み {#getting-around-it}

1. ユーザーを同期するマーケティングツールを使用してSalesforceにログインします。

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. ユーザー名の下で、「 **設定**」に移動します。

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. 「 **個人情報**」で、「 **個人情報**」をクリックします。

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. 「 **編集**」をクリックします。

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. 言語 **を** 英語に変更します ****。

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. 「 **保存**」をクリックします。

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. Marketoに戻るには、 **管理者/Salesforce/オブジェクト** (スキーマの **更新)をクリックします**。

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. これは英語でオブジェクトリストを引き出します。 次に、選択するオブジェクトを選択し、「同期を **有効にする**」をクリックします。

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. カスタムオブジェクトが有効になり、同期が行われていることに注意してください。

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. 次に、Salesforceに戻り、上記の手順を使用して、同期ユーザーを希望の言語に戻します。

>[!NOTE]
>
>**Reminder**
>
>最後にスキーマを更新して、オブジェクトを再び使用するのを忘れないでください。

