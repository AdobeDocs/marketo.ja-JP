---
unique-page-id: 2953461
description: SFDC同期 — フィールド同期 —Marketoドキュメント — 製品ドキュメント
title: SFDC同期 — フィールドの同期
exl-id: fbd66829-53cb-47fd-a530-149d12baee0e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# SFDC同期：フィールドの同期{#sfdc-sync-field-sync}

Marketoは、Salesforceのフィールド情報を同期します。 詳しくは、

## 同期されるフィールドはどれですか。{#which-fields-are-synced}

SFDCのほとんどの標準フィールドと、同期ユーザーが参照する権限を持つカスタムフィールドを同期します。

## MarketoのレコードがSalesforceのリードか連絡先かを判断する方法を教えてください。{#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

MarketoにはSFDC Typeというフィールドがあります。 次の3つの値を指定できます。リード、連絡先、または空です。 空の場合は、このMarketoのリードがSFDCに存在しないことを意味します。

## SFDCでリードまたは連絡先が削除されたかどうかを判断する方法を教えてください。{#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

MarketoにSFDC isDeletedというフィールドがあります。 値がtrueの場合、リードはSFDCで削除されました。

## SFDCに追加する新しいフィールドもMarketoに追加する方法を教えてください。{#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>両方のシステムでフィールドを使用する場合は、まずSFDCでフィールドを作成し、自動的にMarketoに同期します。

SFDCに新しいフィールドを追加し、同期ユーザーがそのフィールドを表示する権限を持っている場合は、そのフィールドが自動的にMarketoに追加されます。

## SFDCでフィールドラベルを変更した場合はどうなりますか。{#what-if-i-change-a-field-label-in-sfdc}

SFDCでフィールドラベルを変更しても、Marketoのフィールドラベルには影響しません。

## SFDCでフィールドの種類を変更した場合はどうなりますか。{#what-if-i-change-a-field-type-in-sfdc}

フィールドの種類を変更すると、Marketoはフィールド内のデータが一致しない場合にそのデータを削除します（ただし、最初に警告が表示されます）。 データを保持するには、フィールドタイプを変更した後に、データを書き出し、再度読み込んでください。

## SFDCでAPI名を変更した場合はどうなりますか。{#what-if-i-change-an-api-name-in-sfdc}

SFDCでフィールドのAPI名を変更すると、Marketoに新しいフィールドが作成されます。

## SFDCに新しいpicklist値を追加するとどうなりますか。{#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

SFDCでフィールドに新しいpicklist値が追加された場合、Marketoから通知が送信されます。

## カスタムSFDCルックアップフィールドについて教えてください。{#what-about-custom-sfdc-lookup-fields}

SFDCのルックアップフィールドでは、IDは同期されますが、参照名は同期されません。

## SFDC Formula Fieldsについて教えてください。{#what-about-sfdc-formula-fields}

数式フィールドは同期されますが、数式内の参照に対する更新は、[システムモードスタンプ](https://help.salesforce.com/apex/HTViewSolution?id=000193203&amp;language=en_US)に対する更新があるまで同期されません。

## 以前にMarketoと同期していたSalesforceのフィールドを削除するとどうなりますか。{#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

SFDCでフィールドを削除しても、Marketoのフィールドは自動的に削除されず、同期が停止します。
