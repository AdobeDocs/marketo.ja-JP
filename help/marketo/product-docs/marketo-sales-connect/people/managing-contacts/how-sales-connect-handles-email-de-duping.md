---
unique-page-id: 14352514
description: Sales Connect がメールの重複除外をどのように処理するかを理解します。 同期時の重複する連絡先の結合方法または処理方法を説明します。
title: Sales Connect でのメールの重複排除の処理方法
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
source-git-commit: 15427eacd2fc42a02f6a4c59d9102bacba02e57b
workflow-type: tm+mt
source-wordcount: '103'
ht-degree: 83%

---

# [!DNL Sales Connect] でのメールの重複排除の処理方法 {#how-sales-connect-handles-email-de-duping}

[!DNL Sales Connect] に [CSV ファイルをアップロード](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md)する場合、読み込みが実行される前に、CSV に含まれるすべての類似の取引先責任者が結合されます。

これは、同じメールアドレスに基づいて行われます。つまり、2 つの同じメールアドレスがある場合、それらを 1 つの取引先責任者に結合します。

後から同じ取引先責任者を手動で追加／アップロードしようとしても、結合されません。

既にデータベースにある取引先責任者を追加しようとしても、追加できないようにします。
