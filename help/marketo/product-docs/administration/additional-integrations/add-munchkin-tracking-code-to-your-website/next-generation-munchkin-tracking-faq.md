---
unique-page-id: 10096583
description: 次世代 [!DNL Munchkin]  トラッキング ロールアウトと匿名フィルターの変更に関するFAQ。
title: 次世代  [!DNL Munchkin]  トラッキングに関する FAQ
exl-id: 283189ac-c817-479a-b896-91233980608c
feature: Administration, Munchkin Tracking Code
hide: true
source-git-commit: 689773f0d6f87b65d5299ecc11f3de11f7e66775
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 48%

---

# 次世代 [!DNL Munchkin] トラッキングに関する FAQ {#next-generation-munchkin-tracking-faq}

Marketoは、次世代のweb トラッキングテクノロジーを段階的に導入しています。

最も重要なポイントは以下のとおりです。

* 「Is Anonymous」スマートリストフィルターが削除されました
* Marketoが取り込むことができるweb イベント（Web ページにアクセス、Web ページでクリックしたリンク）の数が増えています
* [!DNL Munchkin] のコードは変更されないので、web サイトの更新は不要です

## Marketo サブスクリプションはいつ [!DNL Munchkin] V2 になりますか？ {#when-will-my-marketo-subscription-be-on-munchkin-v}

正確な日付はまだ利用できません。 更新については、このページを参照してください。

## Web サイト上の [!DNL Munchkin] トラッキングに変更を加える必要はありますか？ {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

いいえ。 [!DNL Munchkin] トラッキングコードは変わりません。 Web サイトに変更を加える必要はありません。

>[!NOTE]
>
>この変更は、web パーソナライゼーション（リアルタイムパーソナライゼーション）には影響しません。 匿名および既知の web 訪問者を引き続き識別し、これらの訪問者に合わせてリアルタイムでコンテンツをパーソナライズします。

## Marketo でスマートリストから「匿名」フィルターが削除されたのはなぜですか。 {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Marketoは、匿名ユーザーのスマートキャンペーンへの関わり方を一変させました。 以前は、これらのユーザーも既知のユーザーも、スマートキャンペーンの流れは同じでした。 「匿名」フィルターは、キャンペーンで既知の人物のみまたは匿名の人物のみを対象に指定するために使用されていました。

[!DNL Munchkin] V2では、Marketoはすべての匿名アクティビティを引き続き追跡します。ただし、匿名ユーザーにフィルターを適用することはできません。 コンバージョンの時点（Marketo でユーザーが既知となった時点）で、ユーザーが匿名であった間に発生したすべてのアクティビティがそのユーザーのアクティビティログに追加され、その時点から、対象となるキャンペーンが適用されます。

スマートリストで既にこのフィルターを（スマートキャンペーンやレポートなどに）使用中の場合、スマートリストからは自動的に削除されません。 詳しくは、以下を参照してください。

>[!NOTE]
>
>**トリガー**：Web ページへの訪問、Web ページが料金ページ&#x200B;>**フロー**: スコア +10と興味深い瞬間の変更&#x200B;>**Web**：料金ページを閲覧した
>
>[!DNL Munchkin] V2では、匿名ユーザーが価格ページにアクセスした場合、すぐにキャンペーンに参加することはありません。 匿名ユーザーが判明した時点で、Marketoは匿名ユーザーに対してこのキャンペーンを実行します。 次のことを行います。
>
>* スコア 10 ポイントを取得する
>
>* Web ページアクティビティを適切な日付（実際に訪問した日付）に設定する
>
>* 興味を引く瞬間をログに記録する（顧客が既知になった日付ではなく、実際にページを訪問した日付を記録する）
>
>* 現在と同様、「新規ユーザー」アクティビティをログに記録する

## 既に「匿名」フィルターが設定されているスマートリストはどうなりますか。 {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Winter &#39;16 リリースの後、スマートリストに「Is Anonymous」フィルターが含まれている古いスマートキャンペーンがある場合、次の2つのいずれかが発生します。

1. スマートリストで「Is Anonymous（匿名） = False」というフィルターが設定されている場合は、何も起こりません。 無視されます。
1. スマートリストに「Is Anonymous = True」というフィルターがある場合、このキャンペーンは失敗し、通知が送信されます。

## しばらくMarketoを使っています。 どのキャンペーンで「匿名」フィルターを使用しているか確認するには、どうすればよいですか。 {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

この変更の前に、Marketoは「匿名です」フィルターを使用するスマートリスト、スマートキャンペーンおよびレポートのリストを含む通知インボックスに毎週数通の通知を送信しました。 これらのリストは、現在このフィルターがどこで使用されているかを特定するのに役立ちます。

それらを確認し、影響を受けるキャンペーンがあるので、「匿名です」がTrueに設定されている場所を特定します。 多くの場合、この設定は何らかのスコアリングに使用されます。 これらのキャンペーンが現在どのように機能するかを理解するには、上記の例を参照してください。

## より詳細なドキュメントが必要です。 どこで見つけることができますか。 {#id-like-more-detailed-documentation-where-can-i-find-it}

以下のリンクを確認してください。

[匿名リードアップグレードの概要](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[匿名リードアップグレード - Marketo UI内の変更](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[匿名リードのアップグレード – 顧客行動が必要](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[匿名リードのアップグレード – 分析レポート](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[匿名リードアップグレード – リリーススケジュール](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[匿名リードのアップグレード - Under The Hood](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[匿名リードの既知のリードへの昇格 –  [!DNL Munchkin] V2の行動](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## まだ質問があります。 どのようにしたら回答を得ることができますか？ {#i-have-more-questions-how-do-i-get-them-answered}

[Marketo コミュニティ ](https://experienceleaguecommunities.adobe.com/?profile.language=ja){target="_blank"}にアクセスします。 また、Marketo サポートにお問い合わせください。 喜んで質問に答えてくれます。
