---
unique-page-id: 2953188
description: 推測フィルター - Marketo ドキュメント - 製品ドキュメント
title: 推測フィルター
exl-id: 6db4ff4d-7fab-4722-94b1-1bf92ba4651d
source-git-commit: e9a89fb17ca55961c1ee7962d5466b6cb76a9550
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 66%

---

# 推測フィルター {#inferred-filters}

Web サイトの訪問者には、[Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) Cookie が作成され、訪問者はシステムに格納されます。IP は特別なデータベースで調べられ、あらゆる情報が推測されます。

>[!NOTE]
>
>推測されるフィールド値が常に最新の状態に保たれるよう、IP アドレスの検索に使用されるデータベースを定期的に更新します。 データベースの更新により、スマートリストフィルター定義に追加する必要が生じる可能性のある、新しい推測されるフィールド値が追加される場合があります。
>
>データベースの更新は、 [Marketo Engage製品リリース](/help/marketo/release-notes/release-schedule.md){target=&quot;_blank&quot;}。 更新が発生すると、 [Marketo Engageリリースノート](/help/marketo/release-notes/current.md){target=&quot;_blank&quot;} には、推測されるフィールド値に対する変更の説明が含まれます。

![](assets/image2015-4-27-13-3a25-3a46.png)

![](assets/image2015-4-27-16-3a58-3a53.png)

![](assets/image2015-4-27-16-3a59-3a35.png)

![](assets/image2015-4-27-17-3a0-3a12.png)

![](assets/image2015-4-27-13-3a36-3a9.png)

![](assets/image2015-4-27-13-3a30-3a48.png)

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
>詳しくは、[匿名のアクティビティとリード](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/understanding-anonymous-activity-and-people.md)を参照してください。
