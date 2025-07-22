---
unique-page-id: 14352476
description: タスクの「アクティビティタイプ」フィールド（SFDC）- Marketo ドキュメント - 製品ドキュメント
title: タスクの「アクティビティタイプ」フィールド（SFDC）
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 58%

---

# タスクの「アクティビティタイプ」フィールド（SFDC） {#activity-type-field-on-tasks-sfdc}

[!DNL Sales Connect] を使用すると、メールと通話を [!DNL Salesforce] のアクティビティとしてログに記録できます。 [!DNL Salesforce] に貴重なデータを含めるには、[!UICONTROL  タイプ ] フィールドに正しい値を入力することが重要です。

>[!NOTE]
>
>BCC を介したメールのログは、タスクタイプの選択リストを参照せず、代わりに、BCC アドレスを通じて [!DNL Salesforce] に配信されるので、タイプ フィールドに「メール」と自動的に入力します。

## 要件 {#requirements}

* [!DNL Salesforce] との接続
* 「タスクタイプ」の選択リストで「デフォルトタイプなし」値が選択されている
* 「通話（Call）」、「返信（Reply）」、「メール（Email）」がすべて「タスクタイプ」の選択リストに存在する（大文字と小文字の区別）
* 「タイプ」フィールドの値に対してアクションを実行するワークフローまたはトリガーがない

## セットアップ {#setup}

まず、適切な選択リスト値が設定されていることを確認します。選択リストに変更を加えるには、[!DNL Salesforce] 管理者の支援が必要です。

1. [Salesforce.com](https://salesforce.com) に移動し、右上隅の「設定」をクリックします。
1. 「**[!UICONTROL カスタマイズ]**」をクリックします。
1. **[!UICONTROL アクティビティ]** をクリックします。
1. 「**[!UICONTROL タスクフィールド]**」をクリックします。
1. 「**[!UICONTROL タイプ]**」をクリックします。
1. 「タスクタイプ選択リスト」が表示されます。「デフォルト」が選択されていないことを確認します。
1. [!UICONTROL Email]、[!UICONTROL Call]、および [!UICONTROL Reply] に [!UICONTROL Type] 値がリストされていることを確認します。

これで、「タイプ」フィールドに、ログに記録されたメール、通話、返信の対応する値が表示されます。これらの値は、Sales Connect リマインダータスクには設定され&#x200B;_ません_。

>[!NOTE]
>
>値として「返信」が表示されない場合は、「**[!UICONTROL 新規]**」をクリックして返信を追加します。「返信」は、[!DNL Salesforce] の標準値ではありません。
