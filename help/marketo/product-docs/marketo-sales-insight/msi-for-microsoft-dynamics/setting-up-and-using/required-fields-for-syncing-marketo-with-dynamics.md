---
unique-page-id: 11375827
description: MarketoをDynamicsと同期するための必須フィールド —Marketoドキュメント — 製品ドキュメント
title: Marketoとダイナミクスを同期するための必須フィールド
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 2%

---

# MarketoとDynamicsを同期するための必須フィールド{#required-fields-for-syncing-marketo-with-dynamics}

Sales Insightが機能するためには、これらのフィールド&#x200B;*は* Marketoと同期する必要があります。

* 優先順位
* 緊急度
* 相対スコア

これらのフィールドのいずれかが見つからない場合は、Marketoに、見つからないフィールドの名前のエラーメッセージが表示されます。 この問題を修正するには、インスタンスをチェックインして、**リード**&#x200B;と&#x200B;**連絡先**&#x200B;の両方でフィールドが同期されていることを確認してください。 そうでない場合は、追加します。

次に、同期フィールドを検証および追加する方法を示します。

1. 管理者に移動し、**Microsoft Dynamics**&#x200B;をクリックします。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 「フィールドの同期の詳細」で「**編集**」をクリックします。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 「Lead」で、「Priority」チェックボックスをオンにします。

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. 下にスクロールして「緊急性」チェックボックスをオンにします。

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...と「相対スコア」チェックボックスを選択します。

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. 次に、「優先度」、「緊急度」、「連絡先の相対スコア」のチェックボックスをオンにします。

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. 「**保存**」をクリックします。

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>同期が実行されるまで少なくとも10分待ってから、問題が修正されたことを確認してください。

>[!MORELIKETHIS]
>
>[リード/接触レコードの星と炎の設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
