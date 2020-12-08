---
unique-page-id: 2953243
description: 通知タイプ — Marketto Docs — 製品ドキュメント
title: 通知タイプ
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---


# 通知タイプ {#notification-types}

通知の種類はいくつかあります。

## キャンペーンエラー  {#campaign-failure}

キャンペーンの失敗により、スマートキャンペーンのエラーが通知されます。

## CRM同期 {#crm-sync}

CRM同期通知では、権限の誤りや同期の停止など、CRM同期で見つかった重要な問題について警告します。

**Microsoft Dynamics**

Dynamics通知は24時間に1回送信され、その期間に同期に失敗したリードを含みます。 エラーの一般的な原因は、重複のリード（上記の例）またはフィールド長の不一致エラーです。

![](assets/image2016-1-20-11-3a19-3a58.png)

**Salesforce**

Salesforceを使用している場合、同期エラー通知は次のようになります。 一般的なエラーには、期限切れの資格情報やAPIの制限を超えたものが含まれます。

![](assets/salesforcesyncerror.png)

関与

リードがストリーム内で使い果たされると、通知を送信します。  通知には、使い果たされたリードの数や他の情報が含まれます。

![](assets/image2014-10-14-10-3a57-3a9.png)

Facebook

利用規約に同意せずにFacebookにリードを送信しようとする場合、またはMarketoアプリを削除した後でFacebookにリードを送信しようとする場合。

アイドルトリガーキャンペーンのクリーンアップ

アクティビティを取得しなくなったトリガー済みスマートキャンペーンを非アクティブ化します。 自動トリガーキャンペーンのク [リーンアップの詳細](../../../../product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md)。

LinkedIn

3回試行した後に、Marketing Inで新しいオーディエンスを作成できない場合、新しい電子メール、ログインまたはLinkedInへの電子メールのプッシュができない場合。

![](assets/linkedin.png)

Webサービス

1日の割り当てに達すると、通知が送信されます。 クォータは毎夜、中部標準時の午前0時にリセットされます。

>[!NOTE]
>
>表示される可能性のあるエラーコードの一部は、 [開発者用ドキュメントで概要を説明しています](http://developers.marketo.com/rest-api/error-codes/#response_level_error_codes)。

