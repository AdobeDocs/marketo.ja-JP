---
unique-page-id: 2953243
description: 通知のタイプ - Marketo ドキュメント - 製品ドキュメント
title: 通知のタイプ
exl-id: 384cea0a-6252-4600-9211-aa5d6a7e875c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '246'
ht-degree: 100%

---

# 通知のタイプ {#notification-types}

通知のタイプにはいくつかあります。

## キャンペーン失敗  {#campaign-failure}

キャンペーン失敗では、スマートキャンペーンのエラーが通知されます。

## CRM 同期 {#crm-sync}

CRM 同期通知は、誤った権限や同期の停止など、CRM 同期で検出された重要な問題に対して警告します。

**Microsoft Dynamics**

Dynamics 通知は 24 時間に 1 回送信され、その期間に同期できなかったリードが含まれます。障害の一般的な原因は、重複リード（上記）またはフィールド長の不一致エラーです。

![](assets/image2016-1-20-11-3a19-3a58.png)

**Salesforce**

Salesforce を使用する場合、同期エラー通知は次のようになります。一般的なエラーには、期限切れの資格情報や、API の制限を超えたものが含まれます。

![](assets/salesforcesyncerror.png)

エンゲージメント

ストリームでリードが使い果たされると、通知が送信されます。通知には、使い果たされたリードの数やその他の情報が含まれます。

![](assets/image2014-10-14-10-3a57-3a9.png)

Facebook

利用規約に同意せずに Facebook にリードを送信しようとした場合、または Marketo アプリを削除した後で Facebook にリードを送信しようとした場合。

アイドルトリガーキャンペーンクリーンアップ

アクティビティがなくなったスマートキャンペーンのトリガーを非アクティブ化します。[自動トリガーキャンペーンクリーンアップ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md)の詳細をご覧ください。

LinkedIn

3 回試行した後に Marketo が LinkedIn に新しいオーディエンス、ログインまたはプッシュメールを作成できない場合。

![](assets/linkedin.png)

Web サービス

1 日の割り当てに達すると通知が届きます。割り当ては、毎晩午前 0 時（米中部時間）にリセットされます。

>[!NOTE]
>
>受け取る可能性のあるエラーコードの一部は、アドビの[デベロッパー向けドキュメント](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes)で説明されています。
