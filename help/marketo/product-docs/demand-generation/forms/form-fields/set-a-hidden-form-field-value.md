---
unique-page-id: 2359663
description: 非表示フォームフィールド値の設定 —Marketoドキュメント — 製品ドキュメント
title: 非表示フォームフィールド値の設定
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 2%

---

# 非表示フォームフィールド値の設定{#set-a-hidden-form-field-value}

非表示のフィールドは通常、動的に入力されます。 フォームの入力者には表示されません。 値の設定方法を次に示します。

>[!PREREQUISITES]
>
>[フォームフィールドを非表示に設定](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## フィールドを選択{#select-the-field}

1. フォームで、非表示のフィールドを選択し、「**編集**」（**自動入力**）をクリックします。

   ![](assets/autofill.png)

## デフォルト値の使用 {#use-default-value}

「デフォルト値を使用」を選択すると、このフォームが送信されたときに常に使用される特定の値をハードコードできます。 デフォルト値を入力し、「保存」をクリックします。

![](assets/image2014-9-15-13-3a5-3a27.png)

## URL パラメータ {#url-parameter}

ユーザーがフォームの入力時に閲覧しているページからURLパラメーター(クエリ文字列)を取り込む場合は、**URLパラメーター**&#x200B;を使用して、非表示フィールドに値を埋め込むことができます。

>[!NOTE]
>
>パラメーターはテクニーなんでしょ？ 一度手に入れれば、それらは強力です。 [クエリ文字列](https://en.wikipedia.org/wiki/Query_string)のWikipediaページはいくぶん役に立ちます。

1. 「**値の型を取得**」に「**URLパラメーター**」を選択します。

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. **パラメータ名**&#x200B;を入力し、**保存**&#x200B;をクリックします。

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>URLパラメーターが見つからない場合は、デフォルト値を入力できます。

## Cookie 値 {#cookie-value}

Cookieにデータを格納している場合、フォームの送信時に&#x200B;**Cookie値**&#x200B;を使用してデータを取得できます。

1. 「**Get Value From**」に「**Cookie値**」を選択します。

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. 目的のCookieパラメーター名を入力し、「**保存**」をクリックします。

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >パラメーターまたはcookieが見つからない場合に備えて、デフォルト値を入力できます。

## 参照元パラメータ {#referrer-parameter}

訪問者がフォームに入力する前に、転送者の送信元のページからデータを取得する場合は、**パラメータ**&#x200B;を使用できます。

1. **Get Value From**&#x200B;を&#x200B;**転送者パラメーター**&#x200B;に設定します。

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. 転送者URLから取り込む&#x200B;**パラメータ名**&#x200B;を入力し、「**保存**」をクリックします。

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >転送者パラメーターが見つからない場合は、**デフォルト値**&#x200B;を入力できます。

1. 「**完了**」をクリックします。

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. 「**承認して**&#x200B;を閉じる」をクリックします。

   ![](assets/image2014-9-15-13-3a10-3a43.png)
