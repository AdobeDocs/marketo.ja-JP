---
unique-page-id: 3571838
description: Microsoft Dynamics 同期 - フィールドの同期 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 同期 - フィールドの同期
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 100%

---

# [!DNL Microsoft Dynamics] 同期：フィールドの同期 {#microsoft-dynamics-sync-field-sync}

Marketo と [!DNL Dynamics] の同期は非常に強力です。以下に詳細を示します。

## 2 つのシステム間でのフィールドの詳細の同期方法 {#how-are-field-details-kept-in-sync-between-the-two-systems}

リードおよび連絡先エンティティについては、同期は双方向です。[!DNL Dynamics] でリードや取引先責任者に、または Marketo で人物に変更を加えると、更新内容が両方のシステムに反映されます。

アカウント、ユーザ、商談、チームおよびカスタムエンティティについては、同期は、[!DNL Dynamics] から Marketo への一方向です。[!DNL Dynamics] でこれらのエンティティに変更を加えると、更新内容が Marketo に反映されます。

## 両方のシステムの同じフィールドに同時に変更が加えられた場合の動作（データの競合） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

まれなことですが、人物（リード）では Marketo が、取引先責任者では [!DNL Dynamics] が優先されます。これは、人物についてはマーケティング部門が権限を持ち、取引先責任者についてはセールス（CRM）部門が公式な記録システムを持っていると考えているからです。一方的な同期エンティティについては、常に [!DNL Dynamics] が優先されます。

## Marketo を使用して [!DNL Dynamics] のフィールドを作成できますか？ {#can-i-create-a-field-in-dynamics-using-marketo}

いいえ、現在これはサポートされていません。

## [!DNL Dynamics] でフィールドを作成しました。これを Marketo に同期できますか？ {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

はい、同期ユーザが [!DNL Dynamics] でアクセス権を持っている限り、[フィールドを同期](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync)できます。

## Marketo に同期されるフィールド {#what-fields-will-sync-to-marketo}

設定の際に、[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"}できます。

## Marketo と [!DNL Dynamics] が同期された後に、カスタムフィールドを追加する必要がある場合 {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

いつでもフィールドを追加でき、[!DNL Dynamics] から Marketo にデータが更新されます。詳しくは、[新しいカスタムフィールドに対する  [!DNL Microsoft Dynamics]  とのクイック同期の使用](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md)を参照してください。

## 同期するフィールドが追加された後に、[!DNL Dynamics] のフィールドを削除する場合 {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo は、同期するフィールドへの参照を保存します。[!DNL Dynamics] でフィールドを削除する場合は、[同期無効](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)の状態で実行することをお勧めします。次に、「[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)」を編集および保存して、Marketo のスキーマを更新します。
