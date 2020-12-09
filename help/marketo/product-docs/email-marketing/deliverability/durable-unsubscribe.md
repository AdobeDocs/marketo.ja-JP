---
unique-page-id: 10094576
description: 永続的な登録解除 — Marketto Docs — 製品ドキュメント
title: 永続的な登録解除
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---


# 永続的な登録解除 {#durable-unsubscribe}

Marketorは、購読解除機能の動作を強化し、「耐久性」を向上しました。 マスター電子メールのステータスが追加されました。これは、個人の詳細レコードに表示される登録解除フラグとは別のものです。

unsubscribeフラグがfalseからtrueに設定されている場合、マスター電子メールのステータスが更新され、変更が同じ電子メールアドレスを持つ他のユーザーに反映されます。 ユーザーを削除して再作成した場合、または同じ電子メールアドレスを使用して新しいレコードが作成された場合、登録解除フラグは **上書きされません** 。

>[!NOTE]
>
>永続的な登録解除は、Marketoデータベース全体のすべてのパーティションで機能します。

## UnsubscribeフラグをTrueからFalseに更新する（例：人物の再登録） {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

登録を再登録する方法はいくつかあります。

Salesforceで、リード/連絡先のレコードの「電子メール」オプトアウトフィールドを **** クリアします。 これはMarketoと同期されます。

![](assets/one.png)

Marketorで、ユーザーのレコードの「情報」タブの **「登録解除済み」ボックスを** クリアします。

![](assets/two.png)

1人または複数のユーザーに対して、次に示すように、 **** データ値の変更フロー手順を実行します。

![](assets/three.png)

SOAP APIを使用して既存のユーザーを更新します。

## 新しい人物の作成 {#creating-a-new-person}

新しいユーザーが作成されると、Marketorはそのユーザーをマスター電子メールステータステーブルと照合してチェックします。 既に登録が取り消されていた場合は、登録を取り消すレコードを更新します。

## 電子メールアドレスの変更 {#changing-an-email-address}

ユーザーの電子メールアドレスを登録解除された電子メールアドレスに変更すると、そのユーザーは登録解除されます。 この変更は、MarketorまたはSalesforceで発生できます。

登録解除された電子メールアドレスを、登録解除された電子メールアドレスに変更すると、そのユーザーは登録されます。

## 再登録 {#re-subscribing}

登録解除すると、同じ電子メールアドレスを持つすべてのユーザーが登録解除されるのと同じように、再登録すると、実際には同じ電子メールアドレスを持つすべてのユーザーが再登録されます。

## アクティビティログ {#activity-log}

updateLeadEmailStatusと *resetLeadEmailStatusのデータ値の変更定義は* 、 *このコミュニティの記事* で確認できます [](http://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688)。

>[!MORELIKETHIS]
>
>[登録解除](understanding-unsubscribe.md)

