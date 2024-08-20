---
unique-page-id: 2953188
description: 推測フィルター - Marketo ドキュメント - 製品ドキュメント
title: 推測フィルター
exl-id: 6db4ff4d-7fab-4722-94b1-1bf92ba4651d
feature: Smart Lists
source-git-commit: ac7d6b222ca561c88e0bf10aba7736c1b2eee3f7
workflow-type: ht
source-wordcount: '209'
ht-degree: 100%

---

# 推測フィルター {#inferred-filters}

web サイトの訪問者には、[Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} Cookie が作成され、システムに格納されます。IP は特別なデータベースで調べられ、あらゆる情報が推測されます。

>[!NOTE]
>
>推測されるフィールド値が常に最新の状態に保たれるよう、IP アドレスの検索に使用されるデータベースを定期的に更新します。データベースの更新により、スマートリストフィルター定義への追加が必要になる可能性がある、推測されるフィールド値が新たに追加される場合があります。
>
>データベースの更新は、[Marketo Engage 製品のリリース](/help/marketo/release-notes/release-schedule.md){target="_blank"}中に行われる場合があります。更新が行われると、[Marketo Engage リリースノート](/help/marketo/release-notes/current.md){target="_blank"}に、推測されるフィールド値の変更に関する説明が含まれます。

![](assets/inferred-filters-1.png)

![](assets/inferred-filters-2.png)

![](assets/inferred-filters-3.png)

![](assets/inferred-filters-4.png)

![](assets/inferred-filters-5.png)

![](assets/inferred-filters-6.png)

スマートリストでこれらのフィルターのいずれかを使用すると、推測される情報を持つ人物が表示されます。

>[!TIP]
>
>これらのフィルターを web アクティビティレポートで使用します。セールス担当の担当地域を使用して、過去 24 時間以内に web サイトの訪問者を含むカスタム日次レポートに登録します。きっと気に入ることでしょう。
>
>* Web ページにアクセス - 過去 24 時間
>* 推測される都道府県／地域に、[担当地域を選択]します。

匿名の訪問者は、メールリンクをクリックしたりフォームに入力したりすると、自動的に人物に変換されます。ただし、推測される情報はすべて保持されます。

>[!NOTE]
>
>詳しくは、[匿名のアクティビティとリード](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/understanding-anonymous-activity-and-people.md){target="_blank"}を参照してください。
