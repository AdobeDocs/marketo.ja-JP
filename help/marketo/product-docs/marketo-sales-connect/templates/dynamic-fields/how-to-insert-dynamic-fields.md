---
unique-page-id: 14352592
description: 動的フィールドの挿入方法 — Marketo ドキュメント — 製品ドキュメント
title: 動的フィールドの挿入方法
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 100%

---

# 動的フィールドの挿入方法 {#how-to-insert-dynamic-fields}

メールテンプレートを、`{{first_name}}` や `{{company}}` のような事前定義済みの属性を使用してパーソナライズできます。動的フィールドを使用すると、複数の取引先責任者にメールを送信したり、フィールドを取引先責任者ごとに入力せずに自動入力したりできます。

>[!TIP]
>
>「first_name」フィールドと「company」フィールドは、[!DNL Sales Connect] と [!DNL Salesforce] の両方に表示される唯一のフィールドです。つまり、取引先責任者が [web アプリケーション](https://toutapp.com/login)に存在しない場合、[!DNL Salesforce] を調べて、一致するメールアドレスを持つ取引先責任者／リードレコードが見つかるかどうかを確認します。その後、そのレコードの情報を使用してフィールドにデータを入力します。

## テンプレートへの動的フィールドの挿入 {#insert-a-dynamic-field-into-a-template}

1. **[!UICONTROL テンプレートとキャンペーン]**&#x200B;で、編集するテンプレートを見つけて、「**[!UICONTROL テンプレートを編集]**」をクリックします。

1. 「**[!UICONTROL Tout の動的フィールド]**」をクリックします。

   >[!NOTE]
   >
   >[!DNL Sales Connect] に存在する取引先責任者にメールを送信する場合は、基本的な動的フィールドを使用できます。それらのフィールドは、取引先責任者から直接取り込まれます。

[!DNL Salesforce] に存在する取引先責任者にメールを送信する場合は、[!DNL Salesforce] の動的フィールドを利用できます。フィールドはすべて「sfdc」で始まります。[!DNL Salesforce] と連携している限り、動的フィールドは [!DNL Salesforce] 内のリード／取引先責任者を直接呼び出し、テンプレートに情報を入力します。

## 件名行に動的フィールドを挿入 {#insert-dynamic-fields-in-a-subject-line}

メールの件名フィールドに手動でコピーペーストするだけで、適切な形式になっていることを確認できます。
