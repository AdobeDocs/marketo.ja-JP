---
description: オーディエンス条件 — Marketoドキュメント — 製品ドキュメント
title: オーディエンス条件
source-git-commit: 38e65efc50f7f5e7a2a3dbe91035327007475721
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 95%

---

# オーディエンス条件 {#audience-criteria}

Marketo スマートリストと同様に、オーディエンス条件属性を使用すると、ターゲットオーディエンスを定義できます。推測される人、人、会社の属性（またはその組み合わせ）を使用して、既知の人または不明な人をターゲットに設定できます。

**認識済み担当者**

_多数の_&#x200B;属性の組み合わせから選択できます。この例では、50 人以上の従業員を持つ会社で働くカリフォルニア州のすべての&#x200B;**認識済みユーザー**&#x200B;をターゲットにしています。

1. **Person State** 属性を選択し、右にドラッグします。

   ![](assets/audience-criteria-1.png)

1. _Is_ はデフォルトで設定されています。「値を選択」フィールドに「CA」と入力します（ドロップダウンをクリックして、リストから選択することもできます）。

   ![](assets/audience-criteria-2.png)

1. **Company Size** 属性を選択し、_ここに属性をドラッグ＆ドロップ_&#x200B;と書かれた場所にドラッグします。

   ![](assets/audience-criteria-3.png)

   >[!NOTE]
   >
   >属性の **+** アイコンをクリックして選択することもできます。

1. 演算子のドロップダウンをクリックし、「**Greater Than**」を選択します。 

   ![](assets/audience-criteria-4.png)

1. 「50」と入力し、画面の別の場所をクリックして保存します。

   ![](assets/audience-criteria-5.png)

これで完了です。

**匿名担当者**

まだデータベース内にいない人を特定してターゲット設定するのは簡単です。この例では、ニューヨーク地区にいるすべての&#x200B;**匿名ユーザー**&#x200B;をターゲットに設定しています。

1. **Person Email** 属性を選択し、右にドラッグします。

   ![](assets/audience-criteria-6.png)

1. 演算子のドロップダウンをクリックし、「**Is Empty**」を選択します。

   ![](assets/audience-criteria-7.png)

1. **Inferred State** 属性を選択し、_ここに属性をドラッグ＆ドロップ_&#x200B;と書かれた場所にドラッグします。 

   ![](assets/audience-criteria-8.png)

   >[!NOTE]
   >
   >ユーザーが Web サイトが訪問すると、[Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) cookie が作成されてシステムに格納されます。IP は特別なデータベースで調べられ、あらゆる情報が推測されます。

1. _Is_ はデフォルトで設定されています。「値を選択」フィールドに「NY」と入力します（ドロップダウンをクリックして、リストから選択することもできます）。

   ![](assets/audience-criteria-9.png)

## グループを追加 {#add-groups}

すべての特定の属性を別の属性の「すべてまたは任意」と共に持つ場合に備えて、属性をグループ化することもできます。複数のグループを追加できます。

![](assets/audience-criteria-10.png)

![](assets/audience-criteria-11.png)

## ターゲット {#target}

特定のダイアログを表示する URL を入力する場所です。

使用可能な形式：

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>アスタリスクを使用すると包括的なワイルドカードとして機能します。`https://*.website.com` はサブドメイン（例：`support.website.com`）を含み、ダイアログをサイトのすべてのページに配置します。また、`https://website.com/folder/*` は後続のフォルダー内のすべての HTML ページにダイアログを配置します（例：フォルダーが「sports」の場合、website.com/sports/baseball.html、website.com/sports/football.html などになります）。

>[!MORELIKETHIS]
>
>* [ダイアログの作成](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}
>* [ストリームデザイナー](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/stream-designer.md){target=&quot;_blank&quot;}
>* [レポート](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target=&quot;_blank&quot;}

