---
unique-page-id: 14352514
description: Sales Connect でのメールの重複排除の処理方法 - Marketo ドキュメント - 製品ドキュメント
title: Sales Connect でのメールの重複排除の処理方法
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 100%

---

# Sales Connect でのメールの重複排除の処理方法 {#how-sales-connect-handles-email-de-duping}

Sales Connect に [CSV ファイルをアップロード](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md)する場合、インポートが実行される前に、CSV に含まれるすべての類似の連絡先がマージされます。

これは、同じメールアドレスに基づいて行われます。つまり、2 つの同じメールアドレスがある場合、それらを 1 つの取引先責任者に統合します。

後から同じ取引先責任者を手動で追加／アップロードしようとしても、マージされません。

既にデータベースにある取引先責任者を追加しようとしても、追加できないようにします。
