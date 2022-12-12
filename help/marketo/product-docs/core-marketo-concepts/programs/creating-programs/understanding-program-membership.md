---
unique-page-id: 1147091
description: プログラムメンバーシップについて - Marketo ドキュメント - 製品ドキュメント
title: プログラムメンバーシップについて
exl-id: 02480a93-b499-4e0f-8a1c-a22f7d3b7178
source-git-commit: 59768a413038472e38d28e5fb8bcadc4419b360d
workflow-type: ht
source-wordcount: '309'
ht-degree: 100%

---

# プログラムメンバーシップについて {#understanding-program-membership}

>[!NOTE]
>
>Marketo は、すべてのサブスクリプションにわたって言語を標準化することになりました。そのため、サブスクリプションでは「リード」、ドキュメントでは「人物」と表記される場合があります。これらの用語は同じことを意味します。記事の説明には影響しません。他にもいくつかの変更があります。[詳細情報](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)

>[!NOTE]
>
>**定義：**&#x200B;メンバーとは、プログラム内のステータスを持つ人物のことです。

## 人物がプログラムのメンバーになる方法 {#how-people-become-members-of-a-program}

1. 人物が[ランディングページ上のフォーム](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)に入力。

   1. 人物は、自動的に進行の最初のステータスになります。

1. CSV ファイルから[プログラムにメンバーをインポート](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-members-from-a-spreadsheet-into-a-program.md)。

   1. 人物は、自動的に進行の最初のステータスになります。

1. [プログラムステータスの変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md)フローステップを使用。
1. 人物が[イベントプログラムと同期されたウェビナー](/help/marketo/product-docs/demand-generation/events/understanding-events/event-partners.md)に登録するまたは参加。
1. 人物が [Marketo iPad チェックインアプリケーションを使用して作成される](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/check-people-into-your-event-from-your-tablet.md)。
1. 人物が SFDC キャンペーン（[プログラムに同期済み](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md)）に追加される。

>[!NOTE]
>
>メールプログラムの場合、メールの送信時にのみ人物がメンバーシップに追加される。

## プログラムのステータス {#program-statuses}

プログラムのステータスとは、プログラムでユーザが通過する手順を指します（招待済み、返信依頼済み、出席済み、欠席など）。これらの手順は、[チャネル](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)で定義されます。

![](assets/image2015-2-5-15-3a14-3a48.png)

>[!NOTE]
>
>人物は、以前のプログラムステータスに戻ることはできません。ステータスの進行は一方向のみです。

## 成功のステータス {#success-statuses}

プログラムの目的は、人物または見込み客との有意義なインタラクションを作成することです。成功は、人物がその目標に達成するステータスに達したときにマークされます。

>[!NOTE]
>
>ウェビナーの場合、登録は、実際にウェビナーを見ない限り、意味のあるインタラクションではありません。この場合、出席が成功です。

## 新規顧客獲得プログラム  {#acquisition-program}

新しい名前がプログラムメンバーとしてシステムに入力されると、Marketo は自動的にそのプログラムを「獲得」として設定します。これにより、[ファーストタッチ属性](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md)にクレジットが設定されます。

>[!MORELIKETHIS]
>
>* [プログラムでのタグの使用](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags/use-tags-in-a-program.md)
>* [プログラム効果レポートの作成](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report.md)

