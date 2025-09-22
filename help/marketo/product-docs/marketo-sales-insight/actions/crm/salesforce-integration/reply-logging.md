---
description: 返信ログ - Marketo ドキュメント — 製品ドキュメント
title: 返信ログ
hide: true
hidefromtoc: true
exl-id: a89e8212-83cb-4987-abc9-76c5fd74c152
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 100%

---

# 返信ログ {#reply-logging}

Sales Insight Actions は、見込み客の [!DNL Salesforce] への返信を自動的に記録する機能を備えています。これを行うための構造は、メール返信トラッキングに基づいています。見込み客の返信を追跡できる場合は、その返信を [!DNL Salesforce] に記録できます。

## 要件 {#requirements}

* API ログを使用してメールを記録する必要がある
* [返信を追跡できる](/help/marketo/product-docs/marketo-sales-insight/actions/send-a-sales-email/email-tracking-overview.md#how-reply-tracking-works)
* [!DNL Salesforce] との接続が必要
* [!DNL Salesforce] [API 呼び出し](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm)を使用可能にする必要がある

## 返信ログを有効にする {#enable-reply-logging}

1. 返信ログを有効にするには、[!DNL Salesforce] 設定ページに移動します。API ログがオフになると、_返信をログに記録_&#x200B;するオプションが表示されます。

   >[!NOTE]
   >
   >返信ログは、送信されたメールのログに記録する際に指定したのと同じルールに従います。ログには、メールのログ記録方法、リードと取引先責任者、重複する記録がある場合、一致するレコードが見つからない場合が含まれます。

## [!DNL Salesforce] でタイプを返信に設定 {#setting-type-to-reply-in-salesforce}

[!DNL Salesforce] レポートから意味のあるデータを取得することが重要です。「タイプ」フィールドに「返信」と入力する機能を使用すると、レポートからデータを取得できます。`[!DNL Salesforce] admin` と連携して、この設定を取得します。

1. **[!UICONTROL セットアップ]**／**[!UICONTROL カスタマイズ]**／**[!UICONTROL アクティビティ]**／**[!UICONTROL タスクフィールド]**&#x200B;に移動します。
1. 「**[!UICONTROL タイプ]**」をクリックします。
1. 「[!UICONTROL タスクタイプ選択リストの値]」で、「**[!UICONTROL 新規]**」をクリックします。
1. 空のボックスに「Reply」と入力します。必ず「R」を大文字にして、「**[!UICONTROL 保存]**」をクリックします。

   >[!NOTE]
   >
   >「タイプ」選択リストで「デフォルト」を選択する必要はありません。[!DNL Sales Insight Actions] では、このアクティビティタイプが [!DNL Salesforce] インスタンスで使用できることが確認され、それに応じて、受信するアクティビティのタスクフィールドに値を入力します。
