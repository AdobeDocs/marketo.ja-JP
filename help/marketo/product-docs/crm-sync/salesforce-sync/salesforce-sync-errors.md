---
description: MarketoでSalesforceの同期エラーを表示およびフィルタリングする方法について説明します。 レコードレベルおよびジョブレベルのエラーを参照し、エラーの詳細を使用して同期の問題をトラブルシューティングします。
title: Salesforce 同期エラー
exl-id: 4819f423-30c6-48e3-8cec-5d298ceb7b56
feature: Salesforce Integration
TQID: 'https://experienceleague.adobe.com/vEPgjXh8QKyzC1AiAhRqf4tF-MZpu9GETxrRAJHYVIo'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 86%
---
# [!DNL Salesforce] 同期エラー {#salesforce-sync-errors}

同期処理中に発生したエラーの概要を表示します。 これには、互換性のないデータを同期できなかったことによって発生したエラーも含まれます。

>[!NOTE]
>
>**管理者権限が必要**

## 同期エラーの表示 {#view-sync-errors}

1. 「**[!UICONTROL 管理]**」をクリックします。

   ![](assets/salesforce-sync-errors-1.png)

1. 「統合」で、「**Salesforce**」をクリックして、「**[!UICONTROL 同期エラー]**」タブをクリックします。

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
>レコードレベルのレコードをクリックすると、関連オブジェクトの Marketo ID および [!DNL Salesforce] ID が表示されます。 場合によっては、レコードレベルおよびジョブレベルのエラーのメッセージは、[!DNL Salesforce] から直接送信されます。 オンラインで検索すると、追加の詳細が表示される場合があります。

## 同期エラーのフィルタリング {#filter-sync-errors}

1. データをフィルタリングするには、ページの右端にあるフィルターアイコンをクリックします。

   ![](assets/salesforce-sync-errors-3.png)

1. 日付と時間の範囲を選択して、エラータイプ（ジョブレベルまたはレコードレベル）でフィルタリングします。 終了したら「**[!UICONTROL 適用]**」をクリックします。

   ![](assets/salesforce-sync-errors-4.png)

**オプションの手順**：同期エラーをエクスポートするには、「**[!UICONTROL エクスポート]**」をクリックします。 データは CSV としてエクスポートされます。

![](assets/salesforce-sync-errors-5.png)
