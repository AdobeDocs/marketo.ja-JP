---
unique-page-id: 2953461
description: SFDC 同期 - フィールドの同期 - Marketo ドキュメント - 製品ドキュメント
title: SFDC 同期 - フィールドの同期
exl-id: fbd66829-53cb-47fd-a530-149d12baee0e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '413'
ht-degree: 100%

---

# SFDC 同期：フィールドの同期 {#sfdc-sync-field-sync}

Marketo は、Salesforce からフィールド情報を同期します。以下に詳細を示します。

## 同期されるフィールド {#which-fields-are-synced}

SFDC のほとんどの標準フィールドと、同期ユーザーが表示権限を持つカスタムフィールドを同期します。

## Marketo のレコードが Salesforce のリードと連絡先のどちらなのかを判断する方法 {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

Marketo には、「SFDC のタイプ」というフィールドがあります。このフィールドは、リード、連絡先または空の 3 つの値を取ります。空の場合は、この Marketo のリードが SFDC に存在しないことを意味します。

## SFDC でリードや連絡先が削除されたかどうかを判断する方法 {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

Marketo には、「SFDC 削除済み」というフィールドがあります。この値が true の場合、リードは SFDC で削除されています。

## SFDC で追加した新しいフィールドが Marketo にも追加されていることを確認する方法 {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>両方のシステムにフィールドが必要な場合は、最初に SFDC で作成すると、自動的に Marketo に同期されます。

SFDC で新しいフィールドを追加し、同期ユーザーがそれを表示する権限を持っている場合、自動的に Marketo に追加されます。

## SFDC でフィールドラベルを変更する場合の動作 {#what-if-i-change-a-field-label-in-sfdc}

SFDC でフィールドラベルを変更しても、Marketo のフィールドラベルには影響しません。

## SFDC でフィールドタイプを変更する場合の動作 {#what-if-i-change-a-field-type-in-sfdc}

フィールドタイプを変更する場合、Marketo でフィールド内のデータが一致しないと、削除されます（ただし、最初に警告が表示されます）。データを保持するには、フィールドタイプを変更した後、必ずデータをエクスポートおよび再インポートしてください。

## SFDC で API 名を変更する場合の動作 {#what-if-i-change-an-api-name-in-sfdc}

SFDC でフィールドの API 名を変更すると、Marketo に新しいフィールドが作成されます。

## SFDC で新しいピックリスト値を追加する場合の動作 {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

SFDC でフィールドに新しいピックリスト値が追加されると、Marketo から通知が送信されます。

## カスタム SFDC ルックアップフィールドの動作 {#what-about-custom-sfdc-lookup-fields}

SFDC のルックアップフィールドでは、ID は同期されますが、参照される名前は同期されません。

## SFDC 数式フィールドの動作 {#what-about-sfdc-formula-fields}

数式フィールドは同期されますが、数式内の参照に対する更新は、[SystemModStamp](https://help.salesforce.com/apex/HTViewSolution?id=000193203&amp;language=ja_JP) に対する更新があるまで同期されません。

## 以前に Marketo と同期していたフィールドを Salesforce  から削除する場合の動作 {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

SFDC でフィールドを削除しても、Marketo のフィールドは自動的に削除されず、単に同期が停止します。
