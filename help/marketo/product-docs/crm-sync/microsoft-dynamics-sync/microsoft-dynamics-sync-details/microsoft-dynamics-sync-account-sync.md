---
unique-page-id: 3571836
description: アカウント情報をMicrosoft DynamicsからMarketoに同期する方法について説明します。 一方向の同期と連絡先とアカウントの関係について説明します。
title: Microsoft Dynamics Sync — アカウントの同期
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
feature: Microsoft Dynamics
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 91%

---

# [!DNL Microsoft Dynamics] 同期：アカウントの同期 {#microsoft-dynamics-sync-account-sync}

Marketo がデータベース全体を [!DNL Dynamics] と同期しているのを知っていましたか？同期し、5 分待ってから、毎日、再び同期します。ここでは、Marketo が [!DNL Dynamics] のアカウントをどのように扱っているかを詳しく説明します。

## 情報の同期方向 {#which-way-does-the-information-sync}

同期は [!DNL Dynamics] から Marketo への一方向です。

## 更新の仕組み {#how-do-the-updates-work}

Marketo で取引先責任者の「アカウント」フィールドを更新すると、Marketo でそのアカウントに属するすべての取引先責任者の値が変更されます。[!DNL Dynamics] とは同期しません。ただし、次回 [!DNL Dynamics] でアカウントが更新されたときは、Marketo のすべてのアカウント情報が変更によって上書きされます。

## Marketoを使用してアカウントを作成できますか？ {#can-i-create-an-account-using-marketo}

いいえ.Marketo は [!DNL Dynamics] でアカウントを作成できません。

## Marketoと同期するフィールドは何ですか。 {#which-fields-will-sync-to-marketo}

[設定時に同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync)できます。ただし、Marketoは、[!DNL Dynamics] 同期ユーザがアクセスできるフィールドのみを同期します。

## [!DNL Dynamics] の「アカウント」フィールドに変更を加えると、各取引先責任者のデータ値を変更アクティビティログが表示されますか？  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

ほとんどの場合は、表示されます。ただし、アカウントに 5,000 人を超える取引先責任者が存在し、そのアカウントのフィールドが [!DNL Dynamics] で変更された場合は、変更を同期しますが、5,000 人を超える取引先責任者のアクティビティはログに記録されません。
