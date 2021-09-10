---
description: Salesforce 同期エラー — Marketo ドキュメント — 製品ドキュメント
title: Salesforce 同期エラー
exl-id: 4819f423-30c6-48e3-8cec-5d298ceb7b56
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '181'
ht-degree: 100%

---

# Salesforce 同期エラー {#salesforce-sync-errors}

同期処理中に発生したエラーの概要を表示します。これには、互換性のないデータの同期に対する失敗によるエラーも含まれます。

>[!NOTE]
>
>**管理者権限が必要**

## 同期エラーの表示 {#view-sync-errors}

1. 「**管理**」をクリックします。

   ![](assets/salesforce-sync-errors-1.png)

1. 「統合」で、「**Salesforce**」をクリックして、「**同期エラー**」タブをクリックします。

   ![](assets/salesforce-sync-errors-2.png)

>[!NOTE]
>
>表示されるエラーの範囲は、現在の時刻から現在の同期の 5 日前までです。

| フィールド | 説明 |
|---|---|
| 失敗 | レコードレベル&#x200B;_または_&#x200B;ジョブレベル |
| 失敗の日時 | エラーの詳細 |
| エラータイプ | SFDC から返されるメッセージ |

>[!TIP]
>
>レコードレベルのレコードをクリックすると、関連オブジェクトの Marketo ID および Salesforce ID が表示されます。場合によっては、レコードレベルおよびジョブレベルのエラーのメッセージは、Salesforce から直接送信されます。オンラインで検索すると、追加の詳細が表示される場合があります。

## 同期エラーのフィルタリング {#filter-sync-errors}

1. データをフィルタリングするには、ページの右端にあるフィルターアイコンをクリックします。

   ![](assets/salesforce-sync-errors-3.png)

1. 日付と時間の範囲を選択して、エラータイプ（ジョブレベルまたはレコードレベル）でフィルタリングします。終了したら「**適用**」をクリックします。

   ![](assets/salesforce-sync-errors-4.png)

**オプションの手順**：同期エラーをエクスポートするには、「**エクスポート**」をクリックします。データは CSV としてエクスポートされます。

![](assets/salesforce-sync-errors-5.png)
