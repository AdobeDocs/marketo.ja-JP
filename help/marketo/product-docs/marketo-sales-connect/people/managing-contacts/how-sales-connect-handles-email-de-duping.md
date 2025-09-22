---
unique-page-id: 14352514
description: Sales Connect でのメールの重複排除の処理方法 - Marketo ドキュメント - 製品ドキュメント
title: Sales Connect でのメールの重複排除の処理方法
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '96'
ht-degree: 100%

---

# [!DNL Sales Connect] でのメールの重複排除の処理方法 {#how-sales-connect-handles-email-de-duping}

[!DNL Sales Connect] に [CSV ファイルをアップロード](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md)する場合、読み込みが実行される前に、CSV に含まれるすべての類似の取引先責任者がマージされます。

これは、同じメールアドレスに基づいて行われます。つまり、2 つの同じメールアドレスがある場合、それらを 1 つの取引先責任者に統合します。

後から同じ取引先責任者を手動で追加／アップロードしようとしても、マージされません。

既にデータベースにある取引先責任者を追加しようとしても、追加できないようにします。
