---
unique-page-id: 14352480
description: 返信ログ（SFDC） - Marketo ドキュメント — 製品ドキュメント
title: 返信ログ（SFDC）
exl-id: 11f84157-55b7-42a7-81d0-f5848adbb9f4
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 78%

---

# 返信ログ（SFDC） {#reply-logging-sfdc}

Sales Connect は、見込み客の Salesforce への返信を自動的に記録する機能を備えています。これをおこなうための構造は、アドビのメール返信トラッキングに基づいています。見込み客の返信を追跡できる場合は、その返信を Salesforce に記録できます。

## 要件 {#requirements}

* API ログを使用してメールを記録する必要がある
* [返信を追跡できる](/help/marketo/product-docs/marketo-sales-connect/email/common-tracking-questions/how-reply-tracking-works.md)
* [!DNL Salesforce] に接続する必要があります
* [!DNL Salesforce] [API 呼び出し ](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) を使用可能にする必要があります

## 返信ログを有効にする {#enable-reply-logging}

1. 返信ログを有効にするには、[!DNL Salesforce] 設定ページに移動します。 API ログがオフになると、_返信をログに記録_&#x200B;するオプションが表示されます。

   >[!NOTE]
   >
   >返信ログは、送信されたメールのログに記録する際に指定したのと同じルールに従います。ログには、メールのログ記録方法、リードと取引先責任者、重複する記録がある場合、一致するレコードが見つからない場合が含まれます。

## [!DNL Salesforce] で返信するタイプの設定 {#setting-type-to-reply-in-salesforce}

[!DNL Salesforce] レポートから有意義なデータを取得することは重要です。 「タイプ」フィールドに「返信」と入力する機能を使用すると、レポートからデータを取得できます。`[!DNL Salesforce] admin` と連携して、この設定を取得します。

1. **[!UICONTROL セットアップ]**／**[!UICONTROL カスタマイズ]**／**[!UICONTROL アクティビティ]**／**[!UICONTROL タスクフィールド]**&#x200B;に移動します。
1. 「**[!UICONTROL タイプ]**」をクリックします。
1. 「タスクタイプ選択リストの値」で、「**[!UICONTROL 新規]**」をクリックします。
1. 空のボックスに「Reply」と入力します。必ず「R」を大文字にして、「**[!UICONTROL 保存]**」をクリックします。

   >[!NOTE]
   >
   >「タイプ」選択リストで「デフォルト」を選択する必要はありません。[!DNL Sales Connect] のアクティビティタイプが [!DNL Salesforce] インスタンスで使用可能になり、それに応じて、受信アクティビティのタスクフィールドに入力されます。
