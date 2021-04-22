---
description: Salesforce同期エラー —Marketoドキュメント — 製品ドキュメント
title: Salesforce同期エラー
exl-id: 4819f423-30c6-48e3-8cec-5d298ceb7b56
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 3%

---

# Salesforce同期エラー{#salesforce-sync-errors}

表示：同期プロセス中に発生したエラーの概要。 これには、互換性のないデータを同期できないことが原因で発生するエラーが含まれます。

>[!NOTE]
>
>**必要な管理者権限**

## 表示同期エラー{#view-sync-errors}

1. 「**管理者**」をクリックします。

   ![](assets/salesforce-sync-errors-1.png)

1. 「統合」の下の「**Salesforce**」をクリックし、「**同期エラー**」タブをクリックします。

   ![](assets/salesforce-sync-errors-2.png)

>[!NOTE]
>
>表示されるエラーは、現在の時刻から現在の同期の5日前までです。

| フィールド | 詳細 |
|---|---|
| 失敗： | レコードレベル&#x200B;_または_&#x200B;ジョブレベル |
| 失敗の日時 | エラーの詳細 |
| エラータイプ | SFDC返信メッセージ |

>[!TIP]
>
>レコードレベルのレコードをクリックすると、関連オブジェクトのMarketoIDとSalesforce IDが表示されます。 レコードおよびジョブレベルのエラーに関するメッセージが、Salesforceから直接送信される場合があります。 オンラインで検索すると、詳細が表示される場合があります。

## フィルター同期エラー{#filter-sync-errors}

1. データをフィルターするには、ページの右端にあるフィルターアイコンをクリックします。

   ![](assets/salesforce-sync-errors-3.png)

1. 日付と時間の範囲を選択し、「エラーのタイプ」（「ジョブレベル」または「レコードレベル」）でフィルターします。 終了したら「**適用**」をクリックします。

   ![](assets/salesforce-sync-errors-4.png)

**オプションの手順**:同期エラーを書き出すには、「 **書き出し**」をクリックします。データはCSVとしてエクスポートされます。

![](assets/salesforce-sync-errors-5.png)
