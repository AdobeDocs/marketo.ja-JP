---
unique-page-id: 3571838
description: Microsoft Dynamics 同期 - フィールドの同期 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 同期 - フィールドの同期
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 41%

---

# [!DNL Microsoft Dynamics] 同期：フィールド同期 {#microsoft-dynamics-sync-field-sync}

Marketoから [!DNL Dynamics] 同期は非常に強力です。 以下に詳細を示します。

## 2 つのシステム間でのフィールドの詳細の同期方法 {#how-are-field-details-kept-in-sync-between-the-two-systems}

リードおよび連絡先エンティティについては、同期は双方向です。Marketoのリードまたは連絡先、もしく [!DNL Dynamics] ある人物に変更を加えると、その変更は両方のシステムに反映されます。

アカウント、ユーザー、オポチュニティ、チームおよびカスタムエンティティの場合、同期は一方向です。つまり、Marketoに [!DNL Dynamics] 動します。 [!DNL Dynamics] でこれらのエンティティに変更を加えると、その変更内容がMarketoに反映されます。

## 両方のシステムの同じフィールドに同時に変更が加えられた場合の動作（データの競合） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

これはまれですが、Marketoは人物（リード）に勝ち、[!DNL Dynamics] は連絡先に勝ちます。 これは、人物についてはマーケティング部門が権限を持ち、連絡先についてはセールス（CRM）部門が公式な記録システムを持っていると考えているからです。一方向の同期エンティティの場合、[!DNL Dynamics] は常に勝ちます。

## Marketoを使用して [!DNL Dynamics] にフィールドを作成することはできますか？ {#can-i-create-a-field-in-dynamics-using-marketo}

これは、現在、サポートされていません。

## [!DNL Dynamics] でフィールドを作成しました。 Marketo への同期 {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

同期ユーザーが [ でアクセス権を持っている限り、](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) フィールドを同期 [!DNL Dynamics] できます。

## Marketo に同期されるフィールド {#what-fields-will-sync-to-marketo}

設定の際に、[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"}できます。

## Marketoと [!DNL Dynamics] が同期された後にカスタムフィールドを追加する必要がある場合は、どうすればよいですか？ {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

フィールドはいつでも追加でき、データが [!DNL Dynamics] からMarketoに更新されることが期待されます。 詳しくは [ 新しいカスタムフィールド用の  [!DNL Microsoft Dynamics]  クイック同期の使用 ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) を参照してください。

## 同期するフィールドが追加された後で [!DNL Dynamics] のフィールドを削除したい場合はどうすればよいですか？ {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo は、同期するフィールドへの参照を保存します。[!DNL Dynamics] でフィールドを削除する場合は、[ 同期を無効 ](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md) にして行うことをお勧めします。 次に、[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)を編集および保存して、Marketo のスキーマを更新します。
