---
unique-page-id: 14352514
description: メールの重複排除をセールスコネクトがどのように処理するかを理解します。 同期時に重複する連絡先を結合または処理する方法について説明します。
title: Sales Connect でのメールの重複排除の処理方法
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
source-git-commit: 240b78561db11e169188698880d4707a5c1f64de
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 63%

---

# [!DNL Sales Connect] でのメールの重複排除の処理方法 {#how-sales-connect-handles-email-de-duping}

[CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) ファイルを[!DNL Sales Connect]にアップロードする場合、インポートが行われる前に、CSV内のすべての同様の連絡先を結合します。

これは、同じメールアドレスに基づいて行われます。 つまり、2 つの同じメールアドレスがある場合、それらを 1 つの取引先責任者に結合します。

後から同じ取引先責任者を手動で追加／アップロードしようとしても、結合されません。

既にデータベースにある取引先責任者を追加しようとしても、追加できないようにします。
