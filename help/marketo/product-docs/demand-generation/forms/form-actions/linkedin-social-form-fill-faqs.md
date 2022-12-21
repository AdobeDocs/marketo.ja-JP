---
unique-page-id: 10098238
description: LinkedIn ソーシャルフォーム入力に関する FAQ - Marketo ドキュメント - 製品ドキュメント
title: LinkedIn ソーシャルフォーム入力に関する FAQ
exl-id: ce87b918-5b45-418f-9b42-8e8275f2e60a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 100%

---

# LinkedIn ソーシャルフォーム入力に関する FAQ {#linkedin-social-form-fill-faqs}

LinkedIn の改訂された API ポリシーにより、製品から LinkedIn ソーシャルフォーム入力を削除する必要がありました。

## 留意事項 {#important-things-to-know}

* 2016 年 4 月 28 日に、「LinkedIn ソーシャルフォーム入力」ボタンを Marketo に追加するオプションがなくなりました

* 「LinkedIn ソーシャルフォーム入力」ボタンが、有効になっているすべてのフォームから削除されました

## この機能が Marketo 配信登録から削除されたのはなぜですか？ {#why-was-this-functionality-removed-from-my-marketo-subscription}

LinkedIn は、デベロッパープログラムに大きな変更を加えました。これらの変更の一環として、Marketo では、顧客に対してこの機能をサポートできなくなりました。

## ソーシャルフォームが有効になっているフォームから「LinkedIn ソーシャルフォーム入力」ボタンを削除しなかった場合、どうなりますか？ {#what-happened-if-i-didnt-remove-the-linkedin-social-form-fill-buttons-from-my-forms-that-had-social-form-enabled}

2016 年 4 月 28 日に、ソーシャルフォームが有効になっているフォームから「LinkedIn ソーシャルフォーム入力」ボタンを削除しました。

## Marketo の顧客になってから、フォームにこの機能を挿入しています。どのフォームが LinkedIn ソーシャルフォーム入力を使用しるかを知るにはどうすればよいですか？ {#i-have-been-inserting-this-functionality-on-forms-since-we-became-a-marketo-customer-how-do-i-know-which-forms-were-using-linkedin-social-form-fill}

この変更を加える前に、LinkedIn ソーシャルフォーム入力に使用したフォームのリストと共に、毎週の通知をインボックスに送信しました。これらのアラートは、この機能の使用場所を特定するのに役立ちます。

## LinkedIn ソーシャル共有ボタンは機能しますか？ {#do-linkedin-social-sharing-buttons-still-work}

はい。変更は、LinkedIn ソーシャルフォーム入力機能にのみ影響します。

## Facebook と Twitter のソーシャルフォームの入力は、引き続き機能しますか？ {#do-facebook-and-twitter-social-form-fill-still-work}

はい。Facebook と Twitter のソーシャルフォームの入力は変更されていません。

## LinkedIn ソーシャルフォーム入力で既に取り込んだデータに影響はありましたか？ {#did-anything-happen-to-the-data-we-already-captured-via-linkedin-social-form-fill}

いいえ、このデータは既に Marketo のユーザーレコードに保存されており、この変更による影響はありませんでした。

## LinkedIn API ポリシーの詳細はどこで確認できますか？ {#where-can-i-find-more-information-about-linkedin-s-api-policy}

LinkedIn API ポリシーに加えられた変更について詳しくは、[https://developer.linkedin.com/blog/posts/2015/developer-program-changes](https://developer.linkedin.com/blog/posts/2015/developer-program-changes) を参照してください。

## LinkedIn に問い合わせるにはどうすればよいですか？ {#how-can-i-contact-linkedin-with-questions}

LinkedIn のマーケティングソリューションに関して問い合わせるには、[https://business.linkedin.com/marketing-solutions/contact-us](https://business.linkedin.com/marketing-solutions/contact-us) にアクセスしてください。

## Marketo が 4 月 28 日にフォームからこの機能を削除した場合、フォームと影響を受けるランディングページはドラフトモードになっていましたか？ {#if-marketo-removed-this-functionality-from-my-forms-on-april-were-my-forms-and-the-affected-landing-pages-put-into-draft-mode}

いいえ、この機能を削除したフォームは、引き続き発行されます。

## LinkedIn だけが選択したネットワークの場合、フォームの外観は変わりますか？ {#if-linkedin-was-my-only-selected-network-will-this-change-the-appearance-of-my-form}

いいえ、フォームから削除されるのは LinkedIn ボタンだけです。ソーシャルフォームの入力がフォームに適用されると、その上に作成されるコンテナに「ソーシャルフォーム入力」ボタンが含まれます。2016 年 4 月 28 日以前は、LinkedIn が唯一のオプションであった場合、コンテナの外観は次の画像に似ていました。

![--](assets/one.png)

2016 年 4 月 28 日以降、LinkedIn ソーシャルフォーム入力が削除されたフォームの上部に空のコンテナが残るようになりました。

![--](assets/two.png)

>[!NOTE]
>
>上記の画像は例のみです。ソーシャルフォームの入力ボタンのコンテナのレンダリング方法が多少異なる場合があります（フォントの色、スタイルなど）。コンテナの外観に影響を与える設定を選択しました。

## LinkedIn だけが選択したネットワークの場合、フォームの上にある空のコンテナを削除するにはどうすればよいですか？ {#if-linkedin-was-my-only-selected-network-how-can-i-remove-the-empty-container-above-my-form}

空のコンテナを削除するには、フォームを編集し、「ソーシャルフォーム入力」のオプションとして「Facebook」または「Twitter」を選択してから、「ソーシャルフォーム入力」のオプションとして「Facebook」または「Twitter」を選択解除します。これにより、フォーム入力コンテナ内のソーシャルオプションがリセットされ、フォームから削除されます。
