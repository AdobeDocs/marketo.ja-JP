---
unique-page-id: 2359663
description: 非表示フォームフィールド値の設定 — Marketto Docs — 製品ドキュメント
title: 非表示フォームフィールド値の設定
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---


# 非表示フォームフィールド値の設定{#set-a-hidden-form-field-value}

非表示のフィールドは通常、動的に入力されます。 フォームの入力者には表示されません。 値の設定方法を次に示します。

>[!PREREQUISITES]
>
>[フォームフィールドを非表示に設定](set-a-form-field-as-hidden.md)

## フィールドを選択{#select-the-field}

1. フォームで、非表示のフィールドを選択し、「**編集**（**自動入力**）」をクリックします。

   ![](assets/autofill.png)

## デフォルト値を使用{#use-default-value}

「デフォルト値を使用」を選択すると、このフォームが送信されたときに常に使用される特定の値をハードコードできます。 デフォルト値を入力し、「保存」をクリックします。

![](assets/image2014-9-15-13-3a5-3a27.png)

## URLパラメータ{#url-parameter}

ユーザーがフォームの入力時に閲覧しているページからURLパラメーター(クエリ文字列)を取り込む場合は、**URL** **Parameters**&#x200B;を使用して、非表示フィールドに値を埋め込むことができます。

>[!NOTE]
>
>パラメーターはテクニーなんでしょ？ 一度手に入れれば、それらは強力です。 [クエリ文字列](http://en.wikipedia.org/wiki/Query_string)のWikipediaページはいくぶん役に立ちます。

1. 「**値の型を取得**」に「**URLパラメーター**」を選択します。

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. **パラメータ名**&#x200B;を入力し、**保存**&#x200B;をクリックします。

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>URLパラメーターが見つからない場合は、デフォルト値を入力できます。

## Cookie値{#cookie-value}

Cookieにデータを格納している場合は、**Cookie** **値**&#x200B;を使用して、フォームの送信時にデータを取得できます。

1. **Get** **Value** **From**&#x200B;に対して「Cookie ****&#x200B;値&#x200B;**」を選択します。**

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. 目的のCookieパラメーター名を入力し、「**保存**」をクリックします。

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >パラメーターまたはcookieが見つからない場合に備えて、デフォルト値を入力できます。

## 転送者パラメータ{#referrer-parameter}

訪問者がフォームに入力する前に、転送者の送信元のページからデータを取り込む場合は、**パラメータ** **パラメータ**&#x200B;を使用できます。

1. **Get** **Value** **From**&#x200B;を&#x200B;**転送者** **Parameter**&#x200B;に設定します。

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. 転送者URLから取り込む&#x200B;**パラメータ名**&#x200B;を入力し、「**保存**」をクリックします。

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >転送者パラメーターが見つからない場合は、**デフォルト** **値**&#x200B;を入力できます。

1. 「**完了**」をクリックします。

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. 「**承認して**&#x200B;を閉じる」をクリックします。

   ![](assets/image2014-9-15-13-3a10-3a43.png)

甘い！ お元気ですね。 [forms](http://docs.marketo.com/display/docs/forms)については、もっと学ぶべきことがあります。
