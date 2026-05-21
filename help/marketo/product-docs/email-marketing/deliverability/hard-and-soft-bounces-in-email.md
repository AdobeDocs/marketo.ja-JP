---
unique-page-id: 1147328
description: ハードバウンスとソフトバウンス、およびMarketoがそれらのバウンスを分類する方法について説明します。 「電子メールの一時停止」フィールドと「電子メールの無効」フィールドを使用して、問題のある配信を管理します。
title: メールのハードバウンスとソフトバウンス
exl-id: 53298562-76b6-473a-bf9f-2bec682f4d35
feature: Deliverability
TQID: https://experienceleague.adobe.com/qr4rAdOWWg5dazZVztnoTUv6WJQE8Xpm2WKttjQaOOg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 310
ht-degree: 67%

---

# メールのハードバウンスとソフトバウンス {#hard-and-soft-bounces-in-email}

ハードバウンスは、リードのメールアドレスが無効な場合に発生し、リードのメールを配信できないという通知がメールサーバーから届きます。 ソフトバウンスとは、電子メールを受信する際に何らかの問題が発生したことを意味します。この問題は自動的に解決され、数日かかることもあります。 ハードバウンスとソフトバウンスの両方が[複数のカテゴリ](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838)で構成されます。

## バウンスの分類 {#bounce-classification}

Marketoには、問題のあるメール配信に関連する5つの人物フィールドがあります。

1. **メールの中断** - 特定のタイプのハードバウンスが発生したときに True に設定されます。
1. **メールの中断原因** - 考えられる原因は様々ですが、 このフィールドでは原因の特定を試みます。
1. **メールの中断時刻** - 原因となるバウンスが発生すると、Marketo はこのタイムスタンプから 24 時間にわたって当該リードへのメール送信を中断します。
1. **メール無効** - ハードバウンスが発生したときに True に設定されます。
1. **メール無効の理由** - ハードバウンスの理由です。

>[!NOTE]
>
>リードが「**メールの中断**」ステータスに達した後は、「メールの中断」チェックボックスをオフにする方法はありません。 しかし、最初の中断から 24 時間経過すると、引き続き送信可能になります。
>
>ユーザーが&#x200B;**電子メールが無効**&#x200B;とマークされている場合、レコードの「ユーザー情報」タブの「電子メールが無効」ボックスのチェックを外して、手動でのみリセットできます（電子メールアドレスが有効であることを確認した場合にのみ推奨されます）。

>[!PREREQUISITES]
>
>[次の手順](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md)に従って、メールパフォーマンスレポートを作成し、バウンスデータを生成します。

メールパフォーマンスレポートを作成した後、画面は次のようになります。

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>スパムフィルターによってハードバウンスが発生することがあります。 このような「偽陽性」は、リードのメールアドレスが本当に有効かどうかを示しているわけではありません。
