---
unique-page-id: 14352464
description: Salesforce のレポートダッシュボード - Marketo ドキュメント - 製品ドキュメント
title: Salesforce のレポートダッシュボード
exl-id: f27ba3e1-210b-46df-81b5-e794826d36c7
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 85%

---

# Salesforce のレポートダッシュボード {#reporting-dashboards-in-salesforce}

以下に、ダッシュボードの設定方法を示します。

## Open and Click レポート {#open-and-click-report}

1. **[!UICONTROL Tasks and Events]** レコードタイプを選択します。
1. 目的の時間枠や階層構造に基づいて、レポートのパラメーターを定義します。
1. [!DNL Salesforce] に記録された内部メールを削除するフィルターを追加します（例：会社/アカウントがMarketoと等しくない）。
1. **[!UICONTROL Summary]** レポート形式を選択します。
1. 「Subject」、「Assigned」および「Marketo Sales Clicked/Marketo Sales Viewed」フィールドをレポートに追加します。
1. Fields ペイン内の「**[!UICONTROL Add Formula]**」をダブルクリックします。
1. 数式に名前を追加し、形式に「**[!UICONTROL Percent]**」を選択して、「**[!UICONTROL Grouping 1]**」を選択します。
1. 「**[!UICONTROL Marketo売上クリック済み/表示されたMarketo売上]**」を選択し、「概要」フィールドで **[!UICONTROL 合計]** を選択します。
1. 数式に除算記号を追加してから、「Summary」フィールドの「**[!UICONTROL Record Count]**」を選択して、_名前を付けて保存_&#x200B;します。

## Template Performance レポート {#template-performance-report}

1. 以下のフィールドを含めるように Open and Click レポートをカスタマイズして、_名前を付けて保存_&#x200B;します。

## Template Volume レポート {#template-volume-report}

1. Template Performance レポートを修正し、「Marketo Sales Template が空に等しくない」というフィルターを含めます。
1. 「Marketo Sales Clicked」フィールドを削除して、_名前を付けて保存_&#x200B;します。

## Trending Accounts レポート {#trending-accounts-report}

1. Accounts レコードタイプのアクティビティを選択します。
1. レポートのパラメーターとフィールドを以下のように設定して、_名前を付けて保存_&#x200B;します。
