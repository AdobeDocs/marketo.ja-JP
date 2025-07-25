---
unique-page-id: 10096583
description: 次世代  [!DNL Munchkin]  トラッキングに関する FAQ - Marketo ドキュメント - 製品ドキュメント
title: 次世代  [!DNL Munchkin]  トラッキングに関する FAQ
exl-id: 283189ac-c817-479a-b896-91233980608c
feature: Administration, Munchkin Tracking Code
hide: true
hidefromtoc: true
source-git-commit: ea07c5c83c51fef4eb454562f041db685cf13775
workflow-type: ht
source-wordcount: '698'
ht-degree: 100%

---

# 次世代 [!DNL Munchkin] トラッキングに関する FAQ {#next-generation-munchkin-tracking-faq}

当社ではまもなく、次世代の web トラッキング技術の段階的な展開を開始する予定です。

最も重要なポイントは以下のとおりです。

* 第 1 四半期のリリースで「匿名」スマートリストフィルターを削除します（完了済み）
* 取り込み可能な web イベント（Web ページにアクセス、Web ページのリンクをクリック済み）の数を増やしています
* [!DNL Munchkin] のコードは変更されないので、web サイトの更新は不要です

## Marketo サブスクリプションはいつ [!DNL Munchkin] V2 になりますか？ {#when-will-my-marketo-subscription-be-on-munchkin-v}

正確な日付はまだ決まっていませんが、こちらで最新情報を確認してください。

## Web サイト上の [!DNL Munchkin] トラッキングに変更を加える必要はありますか？ {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

いいえ。[!DNL Munchkin] トラッキングコードは変わりません。Web サイトに変更を加える必要はありません。

>[!NOTE]
>
>この変更は、web パーソナライゼーション（リアルタイムパーソナライゼーション）には影響しません。匿名および既知の web 訪問者を引き続き識別し、これらの訪問者に合わせてリアルタイムでコンテンツをパーソナライズします。

## Marketo でスマートリストから「匿名」フィルターが削除されたのはなぜですか。 {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

当社では、匿名の人物がスマートキャンペーンとやり取りする方法を変更しました。以前は、これらのユーザーも既知のユーザーも、スマートキャンペーンの流れは同じでした。「匿名」フィルターは、キャンペーンで既知の人物のみまたは匿名の人物のみを対象に指定するために使用されていました。

[!DNL Munchkin] V2 では、引き続き匿名アクティビティをトラッキングします。ただし、匿名の人物にフィルターを適用することはできなくなります。コンバージョンの時点（Marketo でユーザーが既知となった時点）で、ユーザーが匿名であった間に発生したすべてのアクティビティがそのユーザーのアクティビティログに追加され、その時点から、対象となるキャンペーンが適用されます。

スマートリストで既にこのフィルターを（スマートキャンペーンやレポートなどに）使用中の場合、スマートリストからは自動的に削除されません。詳しくは、以下を参照してください。

>[!NOTE]
>
>**トリガー**：Web ページへの訪問、Web ページが料金ページ\
>**フロー**：変更スコア 10 以上と注目のアクション
>>**Web**：料金ページを閲覧した
>
>[!DNL Munchkin] V2 では、匿名ユーザーが料金ページを訪問しても、すぐにはキャンペーンは開始しません。匿名ユーザーが既知のユーザーとなった時点から、その人物にこのキャンペーンが適用されます。以下の処理が行われます。
>
>* スコア 10 ポイントを取得する
>
>* Web ページアクティビティが適切な日付（実際に訪問した日）に設定される
>
>* 注目のアクションをログに記録する（既知となった時点ではなく、実際にページを訪問した日付）
>
>* 現在と同様、「新規ユーザー」アクティビティをログに記録する

## 既に「匿名」フィルターが設定されているスマートリストはどうなりますか。 {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

2016年冬リリース以降、古いスマートキャンペーンのスマートリストで「匿名」フィルターが設定されている場合は、以下の 2 つのうちいずれかの処理が行われます。

1. スマートリストで「Is Anonymous（匿名） = False」というフィルターが設定されている場合は、何も起こりません。無視されます。
1. スマートリストに「Is Anonymous（匿名） = True」というフィルターがある場合、このキャンペーンは失敗し、通知が送信されます。

## 私はしばらく Marketo を使っています。どのキャンペーンで「匿名」フィルターを使用しているか確認するには、どうすればよいですか。 {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

アドビではこの変更を加える前に、「匿名」フィルターを設定しているスマートリスト、スマートキャンペーン、レポートのリストを記載した週次通知をお客様の「通知」インボックスに送信しました。これらのリストは、現在このフィルターがどこで使用されているかを特定するのに役立ちます。

これらのキャンペーンは変更の影響を受けるので、通知を確認し、「匿名」が「True」に設定されているキャンペーンを特定してください。ほとんどの場合、顧客は何らかのスコアリングにこの設定を使用します。上記の例を参照して、現在これらのキャンペーンの仕組みがどうなったかを理解してください。

## 詳細なドキュメントをいただきたいのですが。どこで見つけることができますか。 {#id-like-more-detailed-documentation-where-can-i-find-it}

以下のリンクを確認してください。

[匿名リードのアップグレードの概要](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[匿名リードのアップグレード - Marketo UI 内の変更点](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[匿名リードのアップグレード - 顧客の対応が必要](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[匿名リードのアップグレード - Analytics レポート](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[匿名リードのアップグレード - リリーススケジュール](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[匿名リードのアップグレード - 調査対象](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[匿名リードを既知のリードに昇格 -  [!DNL Munchkin]  V2 の動作](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## まだ質問があります。どのようにしたら回答を得ることができますか？ {#i-have-more-questions-how-do-i-get-them-answered}

[コミュニティ](https://nation.marketo.com/){target="_blank"}に連絡してください。また、[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}に問い合わせることもできます。喜んで回答させていただきます。
