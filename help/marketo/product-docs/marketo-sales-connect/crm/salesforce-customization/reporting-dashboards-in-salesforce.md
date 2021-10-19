---
unique-page-id: 14352464
description: Salesforce のレポートダッシュボード - Marketo ドキュメント - 製品ドキュメント
title: Salesforce のレポートダッシュボード
exl-id: f27ba3e1-210b-46df-81b5-e794826d36c7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '200'
ht-degree: 100%

---

# Salesforce のレポートダッシュボード {#reporting-dashboards-in-salesforce}

以下に、ダッシュボードの設定方法を示します。

## Open and Click レポート {#open-and-click-report}

1. **Tasks and Events** レコードタイプを選択します。
1. 目的の時間枠や階層構造に基づいて、レポートのパラメーターを定義します。
1. Salesforce に記録された内部メールを削除するためのフィルターを追加します（例：企業／アカウントが Marketo と等しくない）。
1. **Summary** レポート形式を選択します。
1. 「Subject」、「Assigned」および「Marketo Sales Clicked/Marketo Sales Viewed」フィールドをレポートに追加します。
1. Fields ペイン内の「**Add Formula**」をダブルクリックします。
1. 数式に名前を追加し、形式に「**Percent**」を選択して、「**Grouping 1**」を選択します。
1. 「**Marketo Sales Clicked/Marketo Sales Viewed**」を選択して、Summary フィールドで「**Sum**」を選択します。
1. 数式に除算記号を追加してから、「Summary」フィールドの「**Record Count**」を選択して、_名前を付けて保存_&#x200B;します。

## Template Performance レポート {#template-performance-report}

1. 以下のフィールドを含めるように Open and Click レポートをカスタマイズして、_名前を付けて保存_&#x200B;します。

## Template Volume レポート {#template-volume-report}

1. Template Performance レポートを修正し、「Marketo Sales Template が空に等しくない」というフィルターを含めます。
1. 「Marketo Sales Clicked」フィールドを削除して、_名前を付けて保存_&#x200B;します。

## Trending Accounts レポート {#trending-accounts-report}

1. Accounts レコードタイプのアクティビティを選択します。
1. レポートのパラメーターとフィールドを以下のように設定して、_名前を付けて保存_&#x200B;します。
