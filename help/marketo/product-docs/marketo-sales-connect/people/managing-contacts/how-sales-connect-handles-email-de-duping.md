---
unique-page-id: 14352514
description: Sales Connect でのメールの重複排除の処理方法 - Marketo ドキュメント - 製品ドキュメント
title: Sales Connect でのメールの重複排除の処理方法
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '100'
ht-degree: 100%

---

# Sales Connect でのメールの重複排除の処理方法 {#how-sales-connect-handles-email-de-duping}

Sales Connect に [CSV ファイルをアップロード](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md)する場合、インポートが実行される前に、CSV に含まれるすべての類似の連絡先がマージされます。

これは、同じメールアドレスに基づいて行われます。つまり、2 つの同じメールアドレスがある場合、それらを 1 つの連絡先に統合します。

後から同じ連絡先を手動で追加／アップロードしようとしても、マージされません。

既にデータベースにある連絡先を追加しようとしても、追加できないようにします。
