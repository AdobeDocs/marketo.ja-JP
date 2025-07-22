---
unique-page-id: 11382535
description: マイトークンでの URL の使用 - Marketo ドキュメント - 製品ドキュメント
title: マイトークンでの URL の使用
exl-id: 6830c621-4d94-4f31-a608-2f7b2aced88c
feature: Tokens
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 88%

---

# マイトークンでの URL の使用 {#using-urls-in-my-tokens}

以下の手順に従って、[!UICONTROL  マイトークン ] を使用して、メールに URL を挿入します。

1. プログラムを選択し、「**[!UICONTROL マイトークン]**」をクリックします。

   ![](assets/one-4.png)

1. 「**[!UICONTROL テキスト]**&#x200B;マイトークンを」選択して、キャンバスにドラッグ＆ドロップします。

   ![](assets/two-4.png)

1. トークンに一意の名前を付け、URL（https:// を除く）を入力して、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/three-4.png)

   >[!CAUTION]
   >
   >**http／https… の使用**
   >
   >* メール内でクリック数が確実に追跡されるようにするには、トークンの値&#x200B;_内_&#x200B;に https:// と入力&#x200B;**しない**&#x200B;でください。 手順 7 に示すように、トークン外で使用します。
   >
   >* http／https を除外しないことを強くお勧めします。 これにより、メールの [web バージョン](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"}が正しくレンダリングされない可能性があります。

1. プログラム内のメールを選択します。

   ![](assets/four-3.png)

1. 「**[!UICONTROL ドラフトを編集]**」をクリックします。

   ![](assets/five-3.png)

1. 編集するテキスト領域をダブルクリックします。

   ![](assets/six-1.png)

1. メールの任意の場所で、`https://` と入力し（後ろにスペースを残さず）、トークンを挿入アイコンをクリックします。

   ![](assets/seven.png)

   >[!NOTE]
   >
   >もちろん、サイトで「https」を使用しない場合は、`http://` を入力することもできます。

1. マイトークンを探し、選択して、「**[!UICONTROL 挿入]**」をクリックします。

   ![](assets/eight.png)

1. https:// とトークンをハイライト表示し、Ctrl+X（Windows）またはCmd+X（Mac）を押してテキストを切り取ります。

   ![](assets/nine.png)

1. リンクを表示するテキストをハイライト表示し、「[!UICONTROL  リンクを挿入/編集 ]」アイコンをクリックします。

   ![](assets/ten.png)

1. Ctrl/Cmd+V を押して、内容を「**[!UICONTROL URL]**」ボックスにペーストして「**[!UICONTROL 挿入]**」をクリックします。

   ![](assets/eleven.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/twelve.png)

   これで完了です。 送信後に URL が自動入力されます。https://をトークンの前に置くことで、トラッキング可能なリンクが生成されます。
