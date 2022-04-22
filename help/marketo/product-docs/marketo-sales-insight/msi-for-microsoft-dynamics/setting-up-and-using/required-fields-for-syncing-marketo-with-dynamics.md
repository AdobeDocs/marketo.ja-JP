---
unique-page-id: 11375827
description: Marketo を Dynamics と同期するための必須フィールド - Marketo ドキュメント - 製品ドキュメント
title: Marketo と Dynamics を同期するための必須フィールド
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '174'
ht-degree: 100%

---

# Marketo と Dynamics を同期するための必須フィールド {#required-fields-for-syncing-marketo-with-dynamics}

Sales Insight でリードと連絡先の両方を機能させるには、次のフィールドを Marketo と同期する&#x200B;*必要があります*。

* 優先度
* 緊急度
* 相対スコア

これらのフィールドのいずれかが見つからない場合は、見つからないフィールドの名前のエラーメッセージが Marketo に表示されます。この問題を修正するには、ご自身のインスタンスで、**リード**&#x200B;および&#x200B;**連絡先**&#x200B;フィールドが両方とも同期されていることを確認してください。同期されていない場合は、追加します。

同期フィールドを確認して追加する方法を次に示します。

1. 「管理者」に移動し、「**Microsoft Dynamics**」をクリックします。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 「フィールド同期の詳細」で「**編集**」をクリックします。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 「リード」で「優先度」チェックボックスをオンにします。

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. 下にスクロールし、「緊急度」チェックボックスをオンにして...

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...「相対スコア」チェックボックスもオンにします。

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. 次に、連絡先の「優先度」、「緊急度」、「相対スコア」のチェックボックスをオンにします。

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. 「**保存**」をクリックします。

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>同期が実行されるまで 10 分以上待ってから、問題が修正されたことを確認してください。

>[!MORELIKETHIS]
>
>[リード／連絡先レコードの星と炎の設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
