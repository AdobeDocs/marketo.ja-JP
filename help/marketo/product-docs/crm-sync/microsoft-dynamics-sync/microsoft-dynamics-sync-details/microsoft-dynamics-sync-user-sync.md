---
unique-page-id: 3571840
description: Microsoft DynamicsからMarketoへのユーザーデータの同期方法について説明します。 同期する所有者フィールドと、スマートリストおよびフローアクションでそれらを使用する方法について説明します。
title: Microsoft  [!DNL Dynamics]  同期 - ユーザ同期
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/8H1bMdkhxcvyTuYtHHk00GUy4uycuQ1unsGbZ19AjCM
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 160
ht-degree: 79%

---

# Microsoft [!DNL Dynamics] 同期：ユーザ同期 {#microsoft-dynamics-sync-user-sync}

Marketoは、データベース全体を[!DNL Dynamics]と同期します。 同期し、5 分待ってから、毎日、再び同期します。 ここでは、Marketo が [!DNL Dynamics] のアカウントをどのように扱っているかを詳しく説明します。

統合を行うには、専用の Microsoft [!DNL Dynamics] CRM ユーザが必要です。 このユーザーを、同期ユーザーと呼びます。

## 2 つのシステム間でユーザーの詳細を同期させる方法 {#how-are-user-details-kept-in-sync-between-the-two-systems}

ユーザ同期は [!DNL Dynamics] から Marketo への一方向で行われます。 [!DNL Dynamics] でユーザに変更を加えると、その変更が Marketo に反映されます。

## Marketo を使用してユーザーを作成できますか？ {#can-i-create-an-user-using-marketo}

いいえ。 Marketo は [!DNL Dynamics] でユーザを作成できません。

## Marketoと同期するフィールドは何ですか。 {#which-fields-will-sync-to-marketo}

[設定時に同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync)できます。 ただし、Marketoは、[!DNL Dynamics] 同期ユーザがアクセスできるフィールドのみを同期します。
