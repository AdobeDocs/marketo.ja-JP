---
unique-page-id: 11385020
description: 電子メール —Marketoドキュメント — 製品ドキュメントで予測コンテンツを有効にする
title: 電子メールの予測コンテンツを有効にする
exl-id: 7eaefee1-23e8-47ee-afff-adcf49096aa7
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# 電子メールでの予測コンテンツの有効化{#enable-predictive-content-in-emails}

電子メールの予測に1つ以上の画像を作成し、各受信者のエクスペリエンスに合わせて調整します。

>[!NOTE]
>
>予測コンテンツをテストして使用する前に、カテゴリあたり5つ以上のコンテンツを有効にし、ソースあたり（電子メール、リッチメディア、バー）を有効にすることをお勧めします。 コンテンツが多いほど、より適切な予測結果が得られます。

>[!PREREQUISITES]
>
>予測コンテンツを有効にする前に、次の操作を行う必要があります。
>
>* **予測コンテンツの準備**
   >
   >   
   * [電子メールの予測コンテンツの](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md) 編集
   >   * [リッチ](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md) メディアの予測コンテンツの編集
   >   * [レコメンデーションバーの予測コンテンツの編集](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md)
>
>* [予測コンテンツのタイトルの承認](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## Email 2.0 Editorを使用した予測コンテンツの追加{#adding-predictive-content-using-the-email-editor}

1. 「**マーケティングアクティビティ**」をクリックします。

   ![](assets/one.png)

1. 電子メールを選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/two.png)

1. 予測を行う画像をクリックします。 歯車アイコンが表示されたら、アイコンをクリックし、「ContentAIを有効にする」を選択します。****&#x200B;を選択します（ContentAIは予測コンテンツの旧名です）。

   ![](assets/three.png)

1. 1つ以上のカテゴリを選択するには、**カテゴリ**&#x200B;ドロップダウンをクリックし、選択を行い、**適用**&#x200B;をクリックします。

   ![](assets/four.png)

   >[!NOTE]
   >
   >特定のカテゴリの選択や予測レイアウトの変更は任意です。

1. 画像が予測できるようになりました。 追加の画像に対して手順3と4を繰り返します（必要な場合）。

   ![](assets/five.png)

1. 電子メールをプレビューするには、右上隅の&#x200B;**プレビュー**&#x200B;をクリックします。

   ![](assets/six.png)

1. 様々な画像を表示するには、**更新**&#x200B;をクリックします。

   ![](assets/seven.png)

   >[!NOTE]
   >
   >受信者が電子メール&#x200B;_**を開くまで、画像は**_&#x200B;選択されません。 プレビューに見えるのは単なる例で受信者が見るイメージとは限りません

1. 電子メールのプレビューが完了したら、**プレビューアクション**&#x200B;ドロップダウンをクリックし、**承認して閉じる**&#x200B;を選択します。 まだ編集が必要な場合は、右側の「**ドラフトを編集**」をクリックします。

   ![](assets/eight.png)

   >[!NOTE]
   >
   >サンプルを送信する際に、ランダムな画像が選択されます。

電子メールを承認すると、予測コンテンツが提供され、送信できる状態になります。

>[!CAUTION]
>
>受信者が電子メールを開くと、予測画像はロックされます。 コンテンツが後で削除されると、受信者には、コンテンツが存在する場所に壊れた画像が表示されます。

## 電子メール2.0エディターを使用しない場合の予測コンテンツの追加{#adding-predictive-content-when-not-using-the-email-editor}

[電子メール2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md)テンプレートを使用していない場合は、テンプレート内の画像をMarketo編集可能な画像要素としてタグ付けするだけで、予測コンテンツを電子メールに追加できます。

[Marketo固有の構文については、](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md#elements)を参照してください。

次に、コードの例を示します（これは例に過ぎず、下のコードを正確にコピーしないでください）。

**例**

```example
<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com">  
<a><img style="border:10px solid red;"></a>  
</div>
```
