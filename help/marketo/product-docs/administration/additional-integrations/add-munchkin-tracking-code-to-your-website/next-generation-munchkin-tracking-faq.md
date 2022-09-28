---
unique-page-id: 10096583
description: 次世代 Munchkin トラッキングに関する FAQ - Marketo ドキュメント - 製品ドキュメント
title: 次世代 Munchkin トラッキングに関する FAQ
exl-id: 283189ac-c817-479a-b896-91233980608c
source-git-commit: 813bab6169a121e90919f9a02505ccde5167cda4
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 64%

---

# 次世代 Munchkin トラッキングに関する FAQ {#next-generation-munchkin-tracking-faq}

当社ではまもなく、次世代の web トラッキング技術の段階的な展開を開始する予定です。

最も重要なポイントは次のとおりです。

* 第 1 四半期のリリースで「Is Anonymous」スマートリストフィルターを削除します（既に完了しています）
* 取り込み可能な web イベント（Web ページへのアクセス、Web ページでリンクをクリック）の数を増やしています
* Munchkin のコードは変更されないので、web サイトの更新は不要です

## Marketo サブスクリプションはいつ Munchkin V2 になりますか。 {#when-will-my-marketo-subscription-be-on-munchkin-v}

正確な日付はまだ決まっていませんが、こちらで最新情報を確認してください。

## Web サイト上の Munchkin トラッキングに変更を加える必要はありますか。 {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

いいえ。Munchkin トラッキングコードは変わりません。Web サイトに変更を加える必要はありません。

>[!NOTE]
>
>この変更は、web パーソナライゼーション（リアルタイムパーソナライゼーション）には影響しません。匿名および既知の web 訪問者を引き続き識別し、これらの訪問者に合わせてリアルタイムでコンテンツをパーソナライズします。

## Marketoがスマートリストから「匿名」フィルターを削除したのはなぜですか？ {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

当社では、匿名ユーザーがスマートキャンペーンとやり取りする方法を変更しました。以前は、これらのユーザーも既知のユーザーも、スマートキャンペーンの流れは同じでした。「匿名」フィルターは、既知の人または匿名の人のみがキャンペーンを流れるように指定するために使用しました。

Munchkin V2 では引き続き、匿名アクティビティのトラッキングします。ただし、匿名ユーザーにフィルターを適用することはできなくなります。コンバージョンの時点（Marketo でユーザーが既知となった時点）で、ユーザーが匿名であった間に発生したすべてのアクティビティがそのユーザーのアクティビティログに追加され、その時点から、対象となるキャンペーンが適用されます。

スマートリストで既にこのフィルターを（スマートキャンペーンやレポートなどに）使用中の場合、スマートリストからは自動的に削除されません。詳しくは、以下を参照してください。

>[!NOTE]
>
>**トリガー**：Web ページへの訪問、Web ページが料金ページ\
>**フロー**：変更スコア 10 以上と注目のアクション
>**Web**：料金ページを閲覧した
>
>Munchkin V2 では、匿名のユーザーが料金ページを訪問しても、すぐにはキャンペーンは開始しません。匿名ユーザーが既知のユーザーとなった時点から、その人物にこのキャンペーンが適用されます。次の処理がおこなわれます。
>
>* スコア 10 ポイントを取得する
>
>* Web ページアクティビティが適切な日付（実際に訪問した日）に設定される
>
>* 注目のアクションをログに記録する（既知となった時点ではなく、実際にページを訪問した日付）
>
>* 「新規担当者」アクティビティを今日の状態でログに記録する


## 「匿名」フィルターが既に設定されているスマートリストはどうなりますか？ {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

2016 年冬リリースの後、「匿名」フィルターが設定されたスマートリストを持つ古いスマートキャンペーンがある場合は、次の 2 つのうち 1 つが発生します。

1. スマートリストに「Is Anonymous = False」というフィルターがある場合、何も起こりません。 無視されます。
1. スマートリストに「Is Anonymous = True」というフィルターがある場合、このキャンペーンは失敗し、通知が送信されます。

## 私はしばらく Marketo を使っています。「匿名」フィルターを使用しているキャンペーンを知るには、どうすればよいですか？ {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

この変更を行う前に、スマートリスト、スマートキャンペーン、および「匿名」フィルターを使用するレポートのリストと共に、お客様の通知インボックスに毎週数通の通知を送信しました。 これらのリストは、現在このフィルターがどこで使用されているかを特定するのに役立ちます。

影響を受けるキャンペーンなので、匿名を設定した場所を確認し、True に設定しておく必要がある場所を特定してください。 ほとんどの場合、顧客は何らかのスコアリングにこの設定を使用します。上記の例を参照して、現在これらのキャンペーンの仕組みがどうなったかを理解してください。

## 詳細なドキュメントをいただきたいのですが。どこで見つけることができますか。 {#id-like-more-detailed-documentation-where-can-i-find-it}

次のリンクを確認してください。

[匿名リードのアップグレードの概要](https://nation.marketo.com/docs/DOC-2937){target=&quot;_blank&quot;}

[匿名リードのアップグレード — Marketo UI 内の変更](https://nation.marketo.com/docs/DOC-2938){target=&quot;_blank&quot;}

[匿名リードのアップグレード — お客様のアクションが必要](https://nation.marketo.com/docs/DOC-2939){target=&quot;_blank&quot;}

[匿名リードのアップグレード — Analytics レポート](https://nation.marketo.com/docs/DOC-2940){target=&quot;_blank&quot;}

[匿名リードのアップグレード — リリーススケジュール](https://nation.marketo.com/docs/DOC-2961){target=&quot;_blank&quot;}

[匿名のリードのアップグレード — 内部](https://nation.marketo.com/docs/DOC-2962){target=&quot;_blank&quot;}

[匿名リードの既知リードへのプロモーション — Munchkin V2 の動作](https://nation.marketo.com/docs/DOC-2963){target=&quot;_blank&quot;}

## まだ質問があります。どのようにしたら回答を得ることができますか？ {#i-have-more-questions-how-do-i-get-them-answered}

詳しくは、 [コミュニティ](https://nation.marketo.com/){target=&quot;_blank&quot;}。 また、 [Marketoサポート](https://nation.marketo.com/t5/Support/ct-p/Support){target=&quot;_blank&quot;}。 喜んで回答させていただきます。
