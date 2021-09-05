---
unique-page-id: 2949718
description: Sales Insight への電子メールの公開 - Marketo ドキュメント - 製品ドキュメント
title: Sales Insight への電子メールの公開
exl-id: 59b6821f-cbed-427f-942f-0a67cbd4e2df
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '213'
ht-degree: 100%

---

# Sales Insight への電子メールの公開 {#publish-an-email-to-sales-insight}

Sales Insight に公開する設定を有効にして、セールスチームが Sales Insight だけでなく、Outlook および Gmail アドインでも電子メールを利用できるようにします。また、有効期限を指定することもできます。

1. 目的のメールを選択して、「**ドラフトを編集**」をクリックします。

   ![](assets/one.png)

1. エディターが開いたら、「**メール設定**」をクリックします。

   ![](assets/two.png)

1. 「**Marketo Sales Insight に公開**」をオンにします。

   ![](assets/three.png)

1. 有効期限を設定するには（オプション）、「**有効期限を設定**」をオンにして日付を選択します。

   ![](assets/four.png)

   >[!NOTE]
   >
   >（設定した場合）有効期限日の午後 11:59（CST）に、使用可能にしたメールが Sales Insight およびアドインから削除されます。もちろん、Marketo では引き続きアクセス可能です。

1. 「**保存**」をクリックします。

   ![](assets/five.png)

これで完了です。セールスチームが CRM 側で送信するメールを使用できるようにし、必要に応じて利用可能な期間を制限する方法が理解できました。

>[!NOTE]
>
>Microsoft Dynamics または Salesforce の Sales Insight からメールを送信しても、[マイトークン](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)は解決されません。標準のトークン（リード、会社など）のみが入力されます。ただし、トークンのデフォルト値は機能します。

>[!TIP]
>
>変更を有効にするために、忘れずにこのメールを承認してください。[電子メールの承認](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md)方法を参照してください。
