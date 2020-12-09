---
unique-page-id: 11375827
description: MarketorをDynamics - Marketto Docs — 製品ドキュメントと同期するための必須フィールド
title: マーケティングとDynamicsを同期するための必須フィールド
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---


# マーケティングとDynamicsを同期するための必須フィールド {#required-fields-for-syncing-marketo-with-dynamics}

Sales Insightが機能するに *は* 、これらのフィールドをMarketorと同期する必要があります。

* 優先度
* 緊急度
* 相対スコア

これらのフィールドのいずれかが見つからない場合は、Marketorに、見つからないフィールドの名前のエラーメッセージが表示されます。 この問題を修正するには、インスタンスをチェックインして、 **Lead** と **Contactの両方でフィールドが同期されていることを確認します**。 そうでない場合は、追加します。

次に、同期フィールドを検証および追加する方法を示します。

1. [管理者]に移動し、[Microsoft Dynamics]をクリックします。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 「フィールドの同期の詳細」で「編集」をクリックします。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 「Lead」で、「Priority」チェックボックスをオンにします。

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. 下にスクロールして「緊急性」チェックボックスをオンにします。

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...と「相対スコア」チェックボックスを選択します。

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. 次に、「優先度」、「緊急度」、「連絡先の相対スコア」のチェックボックスをオンにします。

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. 「保存」をクリックします。

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>同期が実行されるまで少なくとも10分待ってから、問題が修正されたことを確認してください。

>[!MORELIKETHIS]
>
>[リード/接触レコードの星と炎の設定](http://docs.marketo.com/x/BICMAg)

