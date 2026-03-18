---
unique-page-id: 1147340
description: リード所有者のアドレスからメールを送信する方法を説明します。 「リード所有者から送信」オプションを使用すると、メールに正しい送信者が表示されます。
title: リード所有者からのメール送信
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
feature: Email Editor
source-git-commit: 7eb2f49718ea02be4a394a142c3a0ff05eeff796
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 88%

---

# リード所有者からのメール送信 {#send-emails-from-the-lead-owner}

リード所有者の代わりにリードにメールを送信する場合はどうすればよいですか？手順は次のとおりです。

1. 目的のメールを選択して、「**[!UICONTROL ドラフトを編集]**」をクリックします。

   ![](assets/one.png)

1. 「**[!UICONTROL 送信者]**」フィールドをクリックして（既存の名前を削除）、「**トークンを挿入**」ボタンをクリックします。

   ![](assets/two.png)

1. 「`{{lead.Lead Owner`」を入力し始めて **`{{lead.Lead Owner First Name}}`** トークンを選択します。

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. リードにまだリード所有者がいない場合のデフォルト値を入力し、「**[!UICONTROL 挿入]**」をクリックします。

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. 最初のトークンの後をクリックし、スペースを追加して、「**トークンを挿入**」ボタンをクリックします。

   ![](assets/five.png)

1. 「`{{lead.Lead Owner`」を入力し始めて **`{{lead.Lead Owner Last Name}}`** トークンを選択します。

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. リードにまだリード所有者がいない場合のデフォルト値を入力し、「**[!UICONTROL 挿入]**」をクリックします。

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >姓と名のトークンの間にスペースを追加していることを確認してください。

1. 「**[!UICONTROL 差出人アドレス]**」フィールドをクリックして（既存のメールアドレスを削除）、「**トークンを挿入**」ボタンをクリックします。

   ![](assets/eight.png)

1. 「`{{lead.Lead Owner`」を入力し始めて **`{{lead.Lead Owner Email Address}}`** トークンを選択します。

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. リードにまだリード所有者がいない場合のデフォルト値を入力し、「**[!UICONTROL 挿入]**」をクリックします。

   ![](assets/ten.png)

1. 「**[!UICONTROL 返信先]**」および「**[!UICONTROL 件名]**」フィールドに値が入力されます。これで完了です。

   ![](assets/eleven.png)
