---
description: Marketo EngageとVeeva CRM間の個人アカウントの同期に関するヘルプを参照してください。 個人アカウントが会社と個人として同期され、個人アカウントフィルターを使用する方法について説明します。
title: 人物アカウントの同期 FAQ
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
feature: Veeva CRM
TQID: 'https://experienceleague.adobe.com/7RgVxWE7cvIimLpEMPcBr-DEL2QHVQuDkHR-Tl-ZrcE'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
    internal-label: Implementation
subfeature_v2:
  - id: f141b8e0-5812-4581-b47d-7322a93e7f28
    internal-label: Veeva CRM
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 91%
---
# 人物アカウントの同期 FAQ {#person-account-sync-faq}

Marketo Engage は、レコードの個人取引先タイプに対して、データベース全体を [!DNL Veeva] と同期します。 同期後、5 分待ってから、1 日中、毎日再同期します。

組織のニーズに合わせて、[!DNL Veeva] で個人取引先を設定できます。

>[!NOTE]
>
>「人物アカウント」として「職業」ティアアカウントのみを同期します。

**個人取引先とは**

個人取引先は、[!DNL Veeva] CRM のアカウントオブジェクトと非常に似ています。 ただし、人物アカウントは、アカウントフィールドと取引先責任者フィールドの両方にアクセスできます。

**個人取引先が Marketo に同期されるとどうなりますか？**

人物アカウントは、会社としておよび個人として Marketo に同期されます。

>[!NOTE]
>
>人物アカウントのカスタムフィールドは、Marketo の会社と個人の両方にコピーされます。

**ビジネスアカウントと個人取引先を区別する方法を教えてください。**

スマートリストで「人物」アカウントフィルターを使用して、個人アカウントを標準のビジネスアカウントと区別します。

**個人取引先に使用する必要があるメールフィールドは何ですか？**

1 つの人物アカウントには 2 つのメールフィールドがあります。 Marketo の重複排除やその他のメール処理が正しく機能するよう、フォームでは「メールアドレス」フィールド（「人物メールアドレス」ではなく）を使用します。

## 同期の方向 {#sync-direction}

人物アカウントの取引先責任者関連フィールドの同期は双方向です。 [!DNL Veeva] CRM または Marketo で取引先責任者に変更を加えると、更新内容が両方のシステムに反映されます。 アカウントのフィールドは、[!DNL Veeva] CRM から Marketo への一方向にのみ同期します。

**両方のシステムで、個人取引先の「取引先責任者」フィールドに同時に変更が加えられた場合はどうなりますか？**

[!DNL Veeva]件のCRMが成功しました。 しかし、このようなデータの衝突が起こることは稀です。

**[!DNL Veeva] CRM と同期されるレコードのリードまたは取引先責任者のタイプはありますか？**

[!DNL Veeva] CRM は実際には個人取引先オブジェクトのみを扱い、ビジネスアカウントも持っています。 従来のリード、取引先責任者、商談の CRM タイプは、従来の [!DNL Veeva] CRM システムでは実際には使用されていません。 これらは [!DNL Veeva] CRM で作成できますが、このコネクタの使用は正式にはサポートされていません。

**人物を Marketo の取引先責任者に変換できますか？**

いいえ。リードと取引先責任者は [!DNL Veeva] CRM との同期でサポートされていないタイプです。 そのため、変換はサポートされません。

**取引先責任者の同期を手動で強制できますか？**

いいえ、取引先責任者は独立したレコードではないので、[!DNL Veeva] への人物の同期はサポートされていません。

**すべての標準フィールドが Marketo に同期されるのですか？**

いいえ。すべての標準フィールドが有用というわけではありません。 カスタムフィールドはすべて同期に含めることができます。

>[!NOTE]
>
>Marketo は、Marketo 同期ユーザーがアクセスできるフィールドのみを同期します。

**Marketo は [!DNL Veeva] の検証ルールを遵守しますか？**

はい。競合が発生した場合、その結果はリードのアクティビティログに記録されます。

>[!MORELIKETHIS]
>
>* [デフォルトの  [!DNL Veeva]  フィールドマッピング](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target="_blank"}
>* [通話と通話の主要メッセージの同期](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
