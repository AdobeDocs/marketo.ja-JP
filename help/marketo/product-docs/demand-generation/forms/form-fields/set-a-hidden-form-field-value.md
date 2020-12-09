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


# 非表示フォームフィールド値の設定 {#set-a-hidden-form-field-value}

非表示のフィールドは通常、動的に入力されます。 フォームの入力者には表示されません。 値の設定方法を次に示します。

>[!PREREQUISITES]
>
>[フォームフィールドを非表示に設定](set-a-form-field-as-hidden.md)

## フィールドの選択 {#select-the-field}

1. フォームで、非表示のフィールドを選択し、「 **編集** 」をクリックして **自動入力します**。

   ![](assets/autofill.png)

## デフォルト値を使用 {#use-default-value}

「デフォルト値を使用」を選択すると、このフォームが送信されたときに常に使用される特定の値をハードコードできます。 デフォルト値を入力し、「保存」をクリックします。

![](assets/image2014-9-15-13-3a5-3a27.png)

## URLパラメータ {#url-parameter}

ユーザーがフォームの入力時に閲覧しているページからURLパラメーター(クエリ文字列)を取り込む場合は、 **URL****パラメーター** (非表示フィールドにデータを埋め込むことができます。

>[!NOTE]
>
>パラメーターはテクニーなんでしょ？ 一度手に入れれば、それらは強力です。 クエリ文字列の [Wikipediaページは](http://en.wikipedia.org/wiki/Query_string) 、いくぶん役に立ちます。

1. 「 **Get Value Type** 」で「 **URL Parameter**」を選択します。

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. 「 **パラメータ名** 」を入力し、「 **保存**」をクリックします。

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>URLパラメーターが見つからない場合は、デフォルト値を入力できます。

## Cookieの値 {#cookie-value}

Cookieにデータを格納している場合、 **Cookie** Value **(** Cookie値)を使用して、フォームが送信されるときにデータを取得できます。

1. Get **Cookie****** Value **(** Get **Cookie** Value **)Value(Get Get** Value)From Nothics(Get Cookie Value)

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. 目的のCookieパラメータ名を入力し、「 **保存**」をクリックします。

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >パラメーターまたはcookieが見つからない場合に備えて、デフォルト値を入力できます。

## 転送者パラメータ {#referrer-parameter}

訪問者がフォームに入力する前に指定したページのデータを取得する場合は、 **転送者****パラメーターを使用できます**。

1. Get **Get** **Value** From ******** 転送者Parameter **nothis parameter** nothに設定します。

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. 転送者URLから取り込む **パラメータ名** (Parameter Name **)を入力し、「**&#x200B;保存」をクリックします。

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >転送者パラメーターが見つからない場合は、 **デフォルト****値** (Default Value)を入力できます。

1. 「 **完了**」をクリックします。

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. 「 **承認して閉じる**」をクリックします。

   ![](assets/image2014-9-15-13-3a10-3a43.png)

甘い！ お元気ですね。 フ [ォームについては、さらに学ぶべきことがあります](http://docs.marketo.com/display/docs/forms)。
