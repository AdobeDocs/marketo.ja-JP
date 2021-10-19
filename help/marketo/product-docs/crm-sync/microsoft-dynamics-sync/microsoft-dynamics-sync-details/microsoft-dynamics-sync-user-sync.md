---
unique-page-id: 3571840
description: Microsoft Dynamics Sync - ユーザー同期 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics Sync - ユーザー同期
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '154'
ht-degree: 100%

---

# Microsoft Dynamics Sync：ユーザー同期 {#microsoft-dynamics-sync-user-sync}

Marketo がデータベース全体を Dynamics と同期しているのを知っていましたか？同期を実行し、5 分間待ってから再度同期します。一日中、毎日実行します。Marketo での Dynamics アカウントの処理方法の詳細を以下に示します。

統合を行うには、専用の Microsoft Dynamics CRM ユーザーが必要です。このユーザーを、同期ユーザーと呼びます。

## 2 つのシステム間でユーザーの詳細を同期させる方法 {#how-are-user-details-kept-in-sync-between-the-two-systems}

ユーザー同期は、Dynamics から Marketo への一方向です。Dynamics でユーザーに変更を加えると、その変更が Marketo に反映されます。

## Marketo を使用してユーザーを作成できますか？ {#can-i-create-an-user-using-marketo}

いいえ。Marketo は Dynamics でユーザーを作成できません。

## Marketo と同期するのはどのフィールドですか？ {#which-fields-will-sync-to-marketo}

設定時に[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync)できます。ただし、Marketo は、Dynamics 同期ユーザーがアクセスできるフィールドのみを同期します。
