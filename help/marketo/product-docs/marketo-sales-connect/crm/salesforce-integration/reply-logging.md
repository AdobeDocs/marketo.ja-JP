---
unique-page-id: 14352480
description: 返信ログ（SFDC） - Marketo ドキュメント — 製品ドキュメント
title: 返信ログ（SFDC）
exl-id: 11f84157-55b7-42a7-81d0-f5848adbb9f4
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '276'
ht-degree: 100%

---

# 返信ログ（SFDC） {#reply-logging-sfdc}

Sales Connect は、見込み客の Salesforce への返信を自動的に記録する機能を備えています。これをおこなうための構造は、アドビのメール返信トラッキングに基づいています。見込み客の返信を追跡できる場合は、その返信を Salesforce に記録できます。

## 要件 {#requirements}

* API ログを使用してメールを記録する必要がある
* [返信を追跡できる](/help/marketo/product-docs/marketo-sales-connect/email/common-tracking-questions/how-reply-tracking-works.md)
* Salesforce との接続が必要
* Salesforce [API 呼び出し](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm)を使用可能にする必要がある

## 返信ログを有効にする {#enable-reply-logging}

1. 返信ログを有効にするには、Salesforce 設定ページに移動します。API ログがオフになると、_返信をログに記録_&#x200B;するオプションが表示されます。

   >[!NOTE]
   >
   >返信ログは、送信されたメールのログに記録する際に指定したのと同じルールに従います。これには、メールのログ記録方法が含まれます。リードと連絡先重複する記録がある時一致するレコードが見つからない場合。

## Salesforce でタイプを返信に設定 {#setting-type-to-reply-in-salesforce}

Salesforce レポートから意味のあるデータを取得することが重要です。「タイプ」フィールドに「返信」と入力する機能を使用すると、レポートからデータを取得できます。`Salesforce admin` と連携して、この設定を取得します。

1. **セットアップ**／**カスタマイズ**／**アクティビティ**／**タスクフィールド**&#x200B;に移動します。
1. 「**タイプ**」をクリックします。
1. 「タスクタイプ選択リストの値」で、「**新規**」をクリックします。
1. 空のボックスに「Reply」と入力します。必ず「R」を大文字にして、「**保存**」をクリックします。

   >[!NOTE]
   >
   >「タイプ」選択リストで「デフォルト」を選択する必要はありません。Sales Connect では、このアクティビティタイプが Salesforce インスタンスで使用可能であることが確認され、それに応じて、受信するアクティビティのタスクフィールドに値を入力します。
