---
description: Sales Insight Actions でのメールの重複排除の処理方法 - Marketo ドキュメント - 製品ドキュメント
title: Sales Insight Actions でのメールの重複排除の処理方法
exl-id: 40b01f7f-df50-4bd2-ac35-4c4e4f80915e
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 100%

---

# Sales Insight Actions でメールの重複排除はどのように処理されますか？ {#how-does-sales-insight-actions-handle-email-de-duping}

Sales Insight Actions に [CSV ファイルをアップロード](/help/marketo/product-docs/marketo-sales-insight/actions/people/managing-contacts/import-contacts-via-csv.md)する場合、インポートが実行される前に、CSV に含まれるすべての類似の取引先責任者がマージされます。

これは、同じメールアドレスに基づいて行われます。つまり、2 つの同じメールアドレスがある場合、それらを 1 つの取引先責任者に統合します。

後から同じ取引先責任者を手動で追加／アップロードしようとしても、マージされません。

既にデータベースにある取引先責任者を追加しようとしても、追加できないようにします。
