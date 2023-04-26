---
unique-page-id: 1147066
description: スマートキャンペーンでのリード制限数の上書き - Marketo ドキュメント - 製品ドキュメント
title: スマートキャンペーンでのリード制限数の上書き
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
source-git-commit: bb628e5211601bd8b424c78cae887c2eeb0614cf
workflow-type: ht
source-wordcount: '138'
ht-degree: 100%

---

# スマートキャンペーンでのリード制限数の上書き {#override-person-restrictions-in-a-smart-campaign}

Marketo では、スマートキャンペーンに振り分けられる最大リード数を設定できます。これにより、データベース全体に誤ってメールを送信するのを防ぐことができます。この制限を&#x200B;_上書き_&#x200B;する場合は、次の手順に従います。

>[!PREREQUISITES]
>
>Marketo 管理で、[スマートキャンペーンに対するリード制限を有効](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md)にします。

1. 「マーケティング活動」で、スマートキャンペーンに移動し、「**スケジュール**」をクリックします。

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. スマートキャンペーン設定で、「**編集**」をクリックします。

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >デフォルトの制限は、管理で設定された制限です。

1. 新しい制限を入力し、「**保存**」をクリックします。

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   適合するリード数が設定された制限を超えると、スマートキャンペーンは実行されません。

   >[!CAUTION]
   >
   >誤って多くのリードを含めすぎないように、この機能を活用してください。
