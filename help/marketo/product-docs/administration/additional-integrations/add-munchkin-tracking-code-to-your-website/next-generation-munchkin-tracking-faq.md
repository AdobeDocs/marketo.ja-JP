---
unique-page-id: 10096583
description: 次世代マンチキントラッキングFAQ - Marketto Docs — 製品ドキュメント
title: 次世代マンチキントラッキングFAQ
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 0%

---


# 次世代マンチキントラッキングFAQ {#next-generation-munchkin-tracking-faq}

次世代のウェブトラッキングテクノロジーの段階的な展開を間もなく開始する予定です。

次に、最も重要な知識を示します。

* Q1リリースで「匿名」スマートリストフィルターを削除します（既に完了しています）
* 取り込むことのできるWebイベント（Webページにアクセス、Webページでのリンクのクリック）の数が増えています。
* Munchkinコードは変更されないので、Webサイトの更新は必要ありません

## Munchkin V2には、マーケティング購読はいつ配置されますか。{#when-will-my-marketo-subscription-be-on-munchkin-v}

正確な日付がまだありませんが、更新情報については、こちらを参照してください。

## ウェブサイトでのマンチキンの追跡に変更を加える必要がありますか。{#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

いいえ。 マンチキンのトラッキングコードは変わりません。 Webサイトに変更を加える必要はありません。

>[!NOTE]
>
>この変更は、ウェブパーソナライゼーション（リアルタイムパーソナライゼーション）には影響しません。 匿名で既知のWeb訪問者を引き続き識別し、これらの訪問者にリアルタイムでコンテンツをパーソナライズします。

## スマートリストから「匿名」フィルターが削除されたのはなぜですか？{#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

私たちは匿名の人々がスマートキャンペーンとやり取りする方法を変えました 以前は、知られている人と同じように、賢いキャンペーンを通って流れていました。 「匿名」フィルターは、既知の人または匿名の人のみがキャンペーンを流れることを指定するために使用されました。

Munchkin V2を使って、匿名アクティビティを追跡し続ける。しかし、匿名の人にフィルターを申し込むことはできなくなりました。 コンバージョンの時点（個人がマーケティング担当者についての情報が得られた時点）で、その個人が匿名であったときに発生したすべてのアクティビティが個人アクティビティログに追加され、この時点で、対象となるキャンペーンをフローします。

このフィルターをスマートリスト(スマートキャンペーンやレポートなど)で既に使用している場合、スマートリストから自動的に削除されるわけではありません。 詳しくは、以下を参照してください。

>[!NOTE]
>
>**例**
>
>**トリガー**:訪問回数Webページ、Webページの価格設定ページ\
>**フロー**:Score +10 and Ofterist Moment、 **Web**:表示された価格ページ
>
>Munchkin V2では、匿名の人が価格ページを訪問した場合、キャンペーンにすぐには入りません。 匿名の人が知られたら、このキャンペーンを彼女に対して実行します。 彼女は以下のことを行う。
>
>* 10のスコアを得る
   >
   >
* Webページアクティビティを適切な日付（実際に訪問した場合）に設定する
   >
   >
* 興味深い瞬間をログに記録してください（興味深い瞬間は、その時点が知られた時点ではなく、実際にそのページを訪問した日付を含む）
   >
   >
* 「新しい人」アクティビティを現在の状態でログに記録する

>



## 「匿名」フィルターが既に設定されているスマートリストはどうなりますか？{#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

2016年冬のリリース後、「匿名」フィルターを含むスマートリストを持つ古いスマートキャンペーンがいる場合は、次の2つが発生します。

1. スマートリストに「Is Anonymous = False」というフィルターがある場合、何も起こりません。 無視する。
1. スマートリストに「Is Anonymous = True」というフィルターがある場合、このキャンペーンは失敗し、通知が送信されます。

## 私はしばらくマーケットを使っています。 「匿名」フィルターを使用しているキャンペーンを知る方法を教えてください。{#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

この変更を行う前に、「匿名」フィルターを使用するスマートリスト、スマートキャンペーン、レポートのリストを含む週次通知を通知受信トレイに送信しました。 これらは、このフィルターを現在使用している場所の特定に役立ちます。

それらを確認し、「匿名」がTrueに設定されている場所を特定してください。これは影響を受けるキャンペーンです。 ほとんどの場合、顧客はこの設定を何らかのスコアリングに使用します。 上の例を参照して、これらのキャンペーンが今どのように機能するかを確認してください。

## もっと詳しい文書をお願いします。 どこで見つけられる？{#id-like-more-detailed-documentation-where-can-i-find-it}

次のリンクを確認します。

[匿名リードアップグレードの概要](https://nation.marketo.com/docs/DOC-2937)

[匿名リードのアップグレード — Marketto UI内の変更点](https://nation.marketo.com/docs/DOC-2938)

[匿名リードのアップグレード — お客様の対応が必要](https://nation.marketo.com/docs/DOC-2939)

[匿名リードのアップグレード — Analyticsレポート](https://nation.marketo.com/docs/DOC-2940)

[匿名リードのアップグレード — リリーススケジュール](https://nation.marketo.com/docs/DOC-2961)

[匿名リードアップグレード — 内部](https://nation.marketo.com/docs/DOC-2962)

[既知のリードへの匿名リードのプロモーション — Munchkin V2の動作](https://nation.marketo.com/docs/DOC-2963)

## もっと質問がある！ どうやって答えを？{#i-have-more-questions-how-do-i-get-them-answered}

[コミュニティ](https://nation.marketo.com/welcome)にご連絡ください。 [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#4c3f393c3c233e380c212d3e27293823622f232162)宛てに電子メールを送信することもできます。
