---
unique-page-id: 14352480
description: 返信ログ(SFDC) — マーケティング担当者向けドキュメント — 製品ドキュメント
title: 返信ログ(SFDC)
translation-type: tm+mt
source-git-commit: f28ff1acb0090892bdb92b75ef90d489db7abf20
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---


# 返信ログ(SFDC) {#reply-logging-sfdc}

Sales Connectは、Salesforceに対する見込み客の返信を自動的に記録する機能を備えています。 これを行うための構造は、アドビの電子メール返信追跡に基づいています。 見込み客の返信を追跡できる場合は、その返信をSalesforceに記録できます。

## 要件 {#requirements}

* APIログを使用して電子メールを記録する必要がある
* 返信を [追跡できる必要がある](http://docs.marketo.com/x/BYPS)
* Salesforceに接続する必要がある
* Salesforce [API呼び出しを使用可能にする必要がある](http://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm)

## 返信ログを有効にする {#enable-reply-logging}

1. 返信ログを有効にするには、 [Salesforce設定](http://docs.marketo.com/pages/assets/external-link.jspa) ページに移動します。 APIログのチェックマークを消すと、「*ログの返信」をチェックするオプションが表示されます。\
   *

   >[!NOTE]
   >
   >返信ログは、送信された電子メールのログ記録に使用したのと同じルールに従います。 これには、電子メールのログ記録方法も含まれます。リードと連絡先へ重複記録がある時一致するレコードが見つからない場合。

## Salesforceで返信するタイプの設定 {#setting-type-to-reply-in-salesforce}

Salesforceレポートから意味のあるデータを取得することは重要です。 「タイプ」フィールドに「返信」と入力する機能を持つと、レポートからそのデータを取得できます。 この設定を取得するには、お客様 `Salesforce admin` と提携してください。

1. 「**セットアップ**> **カスタマイズ**> **アクティビティ**> **タスクフィールド**」に移動します。
1. 「 **タイプ**」をクリックします。
1. 「タスクタイプ選択リストの値」で、「 **新規**」をクリックします。
1. 空のボックスに「返信」と入力します。 「R」を大文字にして、「 **保存**」をクリックします。

   >[!NOTE]
   >
   >「タイプ」(Type)ピックリストで「デフォルト」(Default)を選択する必要はありません。 Sales Connectでは、このアクティビティタイプがSalesforceインスタンスで使用可能であることが確認され、それに応じて着信アクティビティのタスクフィールドにデータを入力します。

