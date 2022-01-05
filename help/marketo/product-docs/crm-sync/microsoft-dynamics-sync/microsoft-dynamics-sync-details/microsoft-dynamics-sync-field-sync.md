---
unique-page-id: 3571838
description: Microsoft Dynamics 同期 - フィールドの同期 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 同期 - フィールドの同期
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
source-git-commit: 17cacaa56a437a568bd0d2cc23020f3f880eaf52
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 100%

---

# Microsoft Dynamics 同期：フィールドの同期 {#microsoft-dynamics-sync-field-sync}

Marketo と Dynamics の同期は非常に強力です。以下に詳細を示します。

## 2 つのシステム間でのフィールドの詳細の同期方法 {#how-are-field-details-kept-in-sync-between-the-two-systems}

リードおよび連絡先エンティティについては、同期は双方向です。Dynamics でリードや連絡先に、または Marketo で人物に変更を加えると、更新内容が両方のシステムに反映されます。

アカウント、ユーザー、商談、チームおよびカスタムエンティティについては、同期は、Dynamics から Marketo への一方向です。Dynamics でこれらのエンティティに変更を加えると、更新内容が Marketo に反映されます。

## 両方のシステムの同じフィールドに同時に変更が加えられた場合の動作（データの競合） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

めったにないことですが、人物（リード）では Marketo が、連絡先では Dynamics  が優先されます。これは、人物についてはマーケティング部門が権限を持ち、連絡先についてはセールス（CRM）部門が公式な記録システムを持っていると考えているからです。一方的な同期エンティティについては、常に Dynamics が優先されます。

## Marketo を使用した Dynamics のフィールドの作成 {#can-i-create-a-field-in-dynamics-using-marketo}

これは、現在、サポートされていません。

## Dynamics で作成したフィールドの Marketo への同期 {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Dynamics で同期ユーザーがアクセス権を持っていれば、[フィールドを同期](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-4-of-4-connect.md#select-fields-to-sync)できます。

## Marketo に同期されるフィールド {#what-fields-will-sync-to-marketo}

設定の際に、[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-4-of-4-connect.md#select-fields-to-sync)できます。

## Marketo と Dynamics  が同期した後に、カスタムフィールドを追加する必要がある場合 {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

いつでもフィールドを追加でき、Dynamics から Marketo にデータが更新されます。詳しくは、[新しいカスタムフィールドに対する Microsoft Dynamics とのクイック同期の使用](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md)を参照してください。

## 同期するフィールドが追加された後に、Dynamics のフィールドを削除したい場合 {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo は、同期するフィールドへの参照を保存します。Dynamics でフィールドを削除する場合は、[同期無効](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)の状態で実行することをお勧めします。次に、[同期するフィールドの選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)を編集および保存して、Marketo のスキーマを更新します。
