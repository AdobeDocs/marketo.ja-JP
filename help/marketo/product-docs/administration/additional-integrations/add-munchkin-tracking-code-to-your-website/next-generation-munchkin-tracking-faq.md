---
unique-page-id: 10096583
description: «次世代 [!DNL Munchkin] 追跡 FAQ - Marketoドキュメント — 製品ドキュメント»
title: «次世代 [!DNL Munchkin] トラッキングに関する FAQ»
exl-id: 283189ac-c817-479a-b896-91233980608c
feature: Administration, Munchkin Tracking Code
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 84%

---

# 次世代 [!DNL Munchkin] トラッキングに関する FAQ {#next-generation-munchkin-tracking-faq}

当社ではまもなく、次世代の web トラッキング技術の段階的な展開を開始する予定です。

最も重要なポイントは次のとおりです。

* 第 1 四半期のリリースで「匿名」スマートリストフィルターを削除します（完了済み）
* 取り込み可能な web イベント（Web ページへのアクセス、Web ページでリンクをクリック）の数を増やしています
* お使いの [!DNL Munchkin] コードは変更されないので、Web サイトの更新は不要です

## Marketoのサブスクリプションはいつ有効になるか [!DNL Munchkin] v2? {#when-will-my-marketo-subscription-be-on-munchkin-v}

正確な日付はまだ決まっていませんが、こちらで最新情報を確認してください。

## 自分の [!DNL Munchkin] 追跡していますか？ {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

いいえ。この [!DNL Munchkin] トラッキングコードは変わりません。 Web サイトに変更を加える必要はありません。

>[!NOTE]
>
>この変更は、web パーソナライゼーション（リアルタイムパーソナライゼーション）には影響しません。匿名および既知の web 訪問者を引き続き識別し、これらの訪問者に合わせてリアルタイムでコンテンツをパーソナライズします。

## Marketo でスマートリストから「匿名」フィルターが削除されたのはなぜですか。 {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

当社では、匿名ユーザがスマートキャンペーンとやり取りする方法を変更しました。以前は、これらのユーザも既知のユーザも、スマートキャンペーンの流れは同じでした。「匿名」フィルターは、キャンペーンで既知のユーザまたは匿名ユーザのみを対象に指定するために使用されていました。

を使用 [!DNL Munchkin] V2 では、匿名アクティビティを引き続き追跡します。ただし、匿名担当者にフィルターを適用することはできなくなります。 コンバージョンの時点（Marketo でユーザが既知となった時点）で、ユーザが匿名であった間に発生したすべてのアクティビティがそのユーザのアクティビティログに追加され、その時点から、対象となるキャンペーンが適用されます。

スマートリストで既にこのフィルターを（スマートキャンペーンやレポートなどに）使用中の場合、スマートリストからは自動的に削除されません。詳しくは、以下を参照してください。

>[!NOTE]
>
>**トリガー**：Web ページへの訪問、Web ページが料金ページ\
>**フロー**：変更スコア 10 以上と注目のアクション
>**Web**：料金ページを閲覧した
>
>を使用 [!DNL Munchkin] V2 では、匿名のユーザーが価格ページを訪問した場合、即座にキャンペーンに入ることはありません。 匿名ユーザが既知のユーザとなった時点から、その人物にこのキャンペーンが適用されます。次の処理がおこなわれます。
>
>* スコア 10 ポイントを取得する
>
>* Web ページアクティビティが適切な日付（実際に訪問した日）に設定される
>
>* 注目のアクションをログに記録する（既知となった時点ではなく、実際にページを訪問した日付）
>
>* 現在と同様、「新規ユーザ」アクティビティをログに記録する

## 既に「匿名」フィルターが設定されているスマートリストはどうなりますか。 {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

2016年冬リリース以降、古いスマートキャンペーンのスマートリストで「匿名」フィルターが設定されている場合は、次の 2 つのうちいずれかの処理がおこなわれます。

1. スマートリストで「Is Anonymous（匿名） = False」というフィルターが設定されている場合は、何も起こりません。無視されます。
1. スマートリストに「Is Anonymous（匿名） = True」というフィルターがある場合、このキャンペーンは失敗し、通知が送信されます。

## 私はしばらく Marketo を使っています。どのキャンペーンで「匿名」フィルターを使用しているか確認するには、どうすればよいですか。 {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

アドビではこの変更を加える前に、「匿名」フィルターを設定しているスマートリスト、スマートキャンペーン、レポートのリストを記載した週次通知をお客様の「通知」インボックスに送信しました。これらのリストは、現在このフィルターがどこで使用されているかを特定するのに役立ちます。

これらのキャンペーンは変更の影響を受けるため、通知を確認し、「匿名」が「True」に設定されているキャンペーンを特定してください。ほとんどの場合、顧客は何らかのスコアリングにこの設定を使用します。上記の例を参照して、現在これらのキャンペーンの仕組みがどうなったかを理解してください。

## 詳細なドキュメントをいただきたいのですが。どこで見つけることができますか。 {#id-like-more-detailed-documentation-where-can-i-find-it}

次のリンクを確認してください。

[匿名リードのアップグレードの概要](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[匿名リードのアップグレード - Marketo UI 内の変更点](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[匿名リードのアップグレード - 顧客の対応が必要](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[匿名リードのアップグレード - Analytics レポート](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[匿名リードのアップグレード - リリーススケジュール](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[匿名リードのアップグレード - 調査対象](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[匿名リードの既知リードへのプロモーション — [!DNL Munchkin] V2 の動作](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## まだ質問があります。どのようにしたら回答を得ることができますか？ {#i-have-more-questions-how-do-i-get-them-answered}

詳しくは、 [コミュニティ](https://nation.marketo.com/){target="_blank"}. You can also contact [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}. 喜んで質問に回答いたします。
