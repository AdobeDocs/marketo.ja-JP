---
unique-page-id: 9438139
description: リードをブロックリストに追加 - Marketo ドキュメント - 製品ドキュメント
title: リードをブロックリストに追加
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 44%

---

# リードをブロックリストに追加 {#add-person-to-blocklist}

リードをブロックリストに追加すると、コンテンツを気に入ってくれた有望な人だけにコンテンツを読んでもらえるようになります。

1. 新しい [&#x200B; デフォルトプログラム &#x200B;](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md){target="_blank"} を作成し、「ブロックリストに追加」という名前を付けます。

1. 「**[!UICONTROL 新規作成]**」をクリックして、「**[!UICONTROL 新規ローカルアセット]**」を選択します。

   ![](assets/add-person-to-blocklist-1.png)

1. 「**[!UICONTROL スマートリスト]**」を選択します。

   ![](assets/add-person-to-blocklist-2.png)

1. リストに名前を付け、「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/add-person-to-blocklist-3.png)

1. ブロックリストに追加する全員をスマート リストに追加します。

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >ブロックリストに加えられたリードには、オペレーショナルメールが送信されません。

1. プログラムに戻ります。

   ![](assets/add-person-to-blocklist-5.png)

1. 「**[!UICONTROL 新規作成]**」をクリックして、「**[!UICONTROL 新規スマートキャンペーン]**」を選択します。

   ![](assets/add-person-to-blocklist-6.png)

1. 新しいスマートキャンペーンに名前を付けます。 「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/add-person-to-blocklist-7.png)

1. 「**[!UICONTROL スマートリストのメンバー]**」をドラッグ＆ドロップします。

   ![](assets/add-person-to-blocklist-8.png)

1. 作成したスマート・リストを選択します。

   ![](assets/add-person-to-blocklist-9.png)

1. 「**[!UICONTROL フロー]**」タブをクリックします。 **[!UICONTROL データ値を変更]** フローアクションをドラッグ&amp;ドロップします。

   ![](assets/add-person-to-blocklist-10.png)

1. **[!UICONTROL 属性]** ドロップダウンで **[!UICONTROL Block Listed]** を選択し、**[!UICONTROL New Value]** を **[!UICONTROL true]** に設定します。

   ![](assets/add-person-to-blocklist-11.png)

1. 「**[!UICONTROL スケジュール]**」タブをクリックし、「**[!UICONTROL 1 回実行]**」を選択します。

   ![](assets/add-person-to-blocklist-12.png)

1. 「**[!UICONTROL 今すぐ実行]**」を選択し、「**[!UICONTROL 実行]**」をクリックします。

   ![](assets/add-person-to-blocklist-13.png)

1. もう一度 **[!UICONTROL 実行]** をクリックします。

   ![](assets/add-person-to-blocklist-14.png)

これらのユーザーにはメールが送信されません。

>[!TIP]
>
>[トリガーブロックリストに加える可能な属性を持つ今後のすべてのユーザーについて、{Block Listed が true](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"} の **Change Data Value** を使用して **0} パーソナライゼーションキャンペーンを作成します。**
