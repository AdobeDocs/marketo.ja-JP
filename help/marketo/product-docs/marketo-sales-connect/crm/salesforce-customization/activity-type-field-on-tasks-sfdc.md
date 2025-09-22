---
unique-page-id: 14352476
description: タスクの「アクティビティタイプ」フィールド（SFDC）- Marketo ドキュメント - 製品ドキュメント
title: タスクの「アクティビティタイプ」フィールド（SFDC）
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 100%

---

# タスクの「アクティビティタイプ」フィールド（SFDC） {#activity-type-field-on-tasks-sfdc}

[!DNL Sales Connect] を使用すると、メールと通話を [!DNL Salesforce] のアクティビティとして記録できます。[!DNL Salesforce] で有用なデータを持つ重要な点は、「[!UICONTROL タイプ]」フィールドに正しい値が入力されることです。

>[!NOTE]
>
>BCC によってメールをログに記録する場合、BCC アドレスを通じて [!DNL Salesforce] に配信されるので、「タスクタイプ」選択リストは参照されず、代わりに、タイプフィールドには自動的に「メール」が入力されます。

## 要件 {#requirements}

* [!DNL Salesforce] との接続
* 「タスクタイプ」の選択リストで「デフォルトタイプなし」値が選択されている
* 「通話（Call）」、「返信（Reply）」、「メール（Email）」がすべて「タスクタイプ」の選択リストに存在する（大文字と小文字の区別）
* 「タイプ」フィールドの値に対してアクションを実行するワークフローまたはトリガーがない

## セットアップ {#setup}

まず、適切な選択リスト値が設定されていることを確認します。選択リストに変更を加えるには、[!DNL Salesforce] 管理者の支援が必要です。

1. [Salesforce.com](https://salesforce.com) に移動し、右上隅の「設定」をクリックします。
1. 「**[!UICONTROL カスタマイズ]**」をクリックします。
1. 「**[!UICONTROL アクティビティ]**」をクリックします。
1. 「**[!UICONTROL タスクフィールド]**」をクリックします。
1. 「**[!UICONTROL タイプ]**」をクリックします。
1. 「タスクタイプ選択リスト」が表示されます。「デフォルト」が選択されていないことを確認します。
1. 「[!UICONTROL メール]」、「[!UICONTROL 通話]」、「[!UICONTROL 返信]」に「[!UICONTROL タイプ]」の値が表示されていることを確認します。

これで、「タイプ」フィールドに、ログに記録されたメール、通話、返信の対応する値が表示されます。これらの値は、Sales Connect リマインダータスクには設定され&#x200B;_ません_。

>[!NOTE]
>
>値として「返信」が表示されない場合は、「**[!UICONTROL 新規]**」をクリックして返信を追加します。[!DNL Salesforce] では、「返信」は標準値ではありません。
