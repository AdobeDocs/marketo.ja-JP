---
description: Sales Insight のアクションでメールの重複排除を処理する方法 — Marketoドキュメント — 製品ドキュメント
title: Sales Insight のアクションがメールの重複排除をどのように処理するか
exl-id: 40b01f7f-df50-4bd2-ac35-4c4e4f80915e
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 52%

---

# Sales Insight のアクションは、メールの重複排除をどのように処理しますか？ {#how-does-sales-insight-actions-handle-email-de-duping}

次の場合 [CSV のアップロード](/help/marketo/product-docs/marketo-sales-insight/actions/people/managing-contacts/import-contacts-via-csv.md) ファイルを Sales Insight アクションに取り込むと、インポートが実行される前に、CSV 内の連絡先と同様の連絡先がすべて結合されます。

これは、同じメールアドレスに基づいて行われます。つまり、2 つの同じメールアドレスがある場合、それらを 1 つの連絡先に統合します。

後から同じ連絡先を手動で追加／アップロードしようとしても、マージされません。

既にデータベースにある連絡先を追加しようとしても、追加できないようにします。
