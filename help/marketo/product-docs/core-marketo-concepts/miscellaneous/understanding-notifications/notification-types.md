---
unique-page-id: 2953243
description: 通知タイプ —Marketoドキュメント — 製品ドキュメント
title: 通知タイプ
exl-id: 384cea0a-6252-4600-9211-aa5d6a7e875c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 6%

---

# 通知の種類{#notification-types}

通知の種類はいくつかあります。

## キャンペーン失敗  {#campaign-failure}

キャンペーンの失敗により、スマートキャンペーンのエラーが通知されます。

## CRM 同期 {#crm-sync}

CRM同期通知では、権限の誤りや同期の停止など、CRM同期で見つかった重要な問題について警告します。

**Microsoft Dynamics**

Dynamics通知は24時間に1回送信され、その期間に同期に失敗したリードを含みます。 エラーの一般的な原因は、重複のリード（上記の例）またはフィールド長の不一致エラーです。

![](assets/image2016-1-20-11-3a19-3a58.png)

**Salesforce**

Salesforceを使用している場合、同期エラー通知は次のようになります。 一般的なエラーには、期限切れの資格情報やAPIの制限を超えたものが含まれます。

![](assets/salesforcesyncerror.png)

エンゲージメント

リードがストリーム内で使い果たされると、通知を送信します。  通知には、使い果たされたリードの数や他の情報が含まれます。

![](assets/image2014-10-14-10-3a57-3a9.png)

Facebook

利用規約に同意せずにFacebookにリードを送信しようとする場合、またはMarketoアプリを削除した後でFacebookにリードを送信しようとする場合。

アイドルトリガーキャンペーン・クリーンアップ

アクティビティを取得しなくなったトリガー済みスマートキャンペーンを非アクティブ化します。 [トリガーキャンペーンの自動クリーンアップ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md)の詳細を表示します。

LinkedIn

Marketoが3回試行した後に、新しいオーディエンス、ログイン、またはLinkedInへの電子メールのプッシュを作成できない場合。

![](assets/linkedin.png)

ウェブサービス

1日の割り当てに達すると、通知が送信されます。 クォータは毎夜、中部標準時の午前0時にリセットされます。

>[!NOTE]
>
>表示される可能性のあるエラーコードの一部は、アドビの[開発者向けドキュメント](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes)で概要を説明しています。
