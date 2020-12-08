---
unique-page-id: 2953461
description: SFDC同期 — フィールドの同期 — マーケティング担当者向けドキュメント — 製品ドキュメント
title: SFDC同期 — フィールド同期
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---


# SFDC同期：フィールドの同期 {#sfdc-sync-field-sync}

Marketorは、Salesforceのフィールド情報を同期します。 詳しくは、

## 同期されるフィールドはどれですか。 {#which-fields-are-synced}

SFDCのほとんどの標準フィールドと、同期ユーザーが参照する権限を持つカスタムフィールドを同期します。

## MarketoのレコードがSalesforceのリードか連絡先かを判断する方法を教えてください。 {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

MarketoにはSFDC Typeというフィールドがあります。 次の3つの値を指定できます。リード、連絡先、または空です。 空の場合は、このマーケティング担当者がSFDCに存在しないことを意味します。

## SFDCでリードまたは連絡先が削除されたかどうかを判断する方法を教えてください。 {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

MarketoにはSFDC isDeletedというフィールドがあります。 値がtrueの場合、リードはSFDCで削除されました。

## SFDCに追加する新しいフィールドもMarketoに追加するようにするには、どうすればよいですか。 {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>両方のシステムでフィールドが必要な場合は、まずSFDCでフィールドを作成しておくと、自動的にMarketoと同期します。

SFDCに新しいフィールドを追加し、同期ユーザーがそのフィールドを表示する権限を持っている場合は、そのフィールドが自動的にMarketoに追加されます。

## SFDCでフィールドラベルを変更した場合はどうなりますか。 {#what-if-i-change-a-field-label-in-sfdc}

SFDCでフィールドラベルを変更しても、Marketoのフィールドラベルには影響しません。

## SFDCでフィールドの種類を変更した場合はどうなりますか。 {#what-if-i-change-a-field-type-in-sfdc}

フィールドの種類を変更すると、一致しない場合はフィールド内のデータが削除されます（ただし、最初に警告が表示されます）。 データを保持するには、フィールドタイプを変更した後に、データを書き出し、再度読み込んでください。

## SFDCでAPI名を変更した場合はどうなりますか。 {#what-if-i-change-an-api-name-in-sfdc}

SFDCでフィールドのAPI名を変更すると、Marketoに新しいフィールドが作成されます。

## SFDCに新しいpicklist値を追加するとどうなりますか。 {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

SFDCでフィールドに新しいpicklist値が追加された場合、Marketoから通知が送信されます。

## カスタムSFDCルックアップフィールドについて教えてください。 {#what-about-custom-sfdc-lookup-fields}

SFDCのルックアップフィールドでは、IDは同期されますが、参照名は同期されません。

## SFDC Formula Fieldsについて教えてください。 {#what-about-sfdc-formula-fields}

数式フィールドは同期されますが、数式内の参照に対する更新は、 [システムモードスタンプに対する更新があるまで同期されません](https://help.salesforce.com/apex/HTViewSolution?id=000193203&amp;language=en_US)。

## 以前にMarketoと同期していたSalesforceからフィールドを削除するとどうなりますか。 {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

SFDCでフィールドを削除しても、Marketoのフィールドは自動的には削除されませんが、同期が停止するだけです。
