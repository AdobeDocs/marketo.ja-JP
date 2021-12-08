---
unique-page-id: 2951640
description: 注目のアクションの使用 - Marketo ドキュメント - 製品ドキュメント
title: 注目のアクションの使用
exl-id: ccf7664b-08e1-490a-a3f9-5fa3bd8fb05f
source-git-commit: 1dd4a4f6bfac0b101f85f3776396aeef1a1f7182
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 79%

---

# 注目のアクションの使用 {#using-interesting-moments}

注目のアクションは、Marketo Sales Insight アプリを通じてセールスチームとコミュニケーションを取るための鍵となります。

>[!AVAILABILITY]
>
>注目のアクションを使用できるのは、Marketo Sales Insight と [Marketo Sales Connect](/help/marketo/product-docs/marketo-sales-connect/marketo/interesting-moments-in-sales-connect.md) を契約されたお客様だけです。

## 注目のアクションとは何でしょうか。 {#what-is-an-interesting-moment}

それは、あなた次第です。どんな情報がセールスチームに関係あるのかを自分で決定します。セールスチームがリードについて知りたいのは、例えば次のようなことです。

* Web サイトの価格設定ページへのアクセス
* 新製品発表メールに記載されたリンクをクリック
* 製品デモをリクエスト

## 注目のアクションを作成する方法  {#how-do-i-create-an-interesting-moment}

1. [スマートキャンペーン](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)を選択します。トリガーされた場合にセールスチームが興味を持つものがいいでしょう。

   ![](assets/using-interesting-moments-1.png)

1. **注目のアクション**&#x200B;フローステップをドラッグします。

   ![](assets/using-interesting-moments-2.png)

1. **タイプ**&#x200B;を選択します（メール、マイルストーン、web）。

   ![](assets/using-interesting-moments-3.png)

1. このアクションが重要である理由として、セールスチームへのメッセージを「**説明**」フィールドに記入します。

   ![](assets/using-interesting-moments-4.png)

   >[!NOTE]
   >
   >注目のアクションが発生した日付と、追加された経緯（リードアクション > フローステップ > SOAP API など）も Marketo によって記録されます。

## 注目のアクションにさらに注目を集めるには  {#how-can-this-get-even-more-interesting}

トークンを使います。より具体的な情報を営業チームに伝えるために、説明フィールドにトークンを追加します。リードが開くメールの件名、または送信者といった情報です。[注目のアクションのトークン](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md)の用語集を参照して使用できるトークンを確認してください。

>[!TIP]
>
>5 つの注目のアクションから始め、セールスチームと協力して、どの情報を確認するのかを判断します。

## 注目のアクションは、Marketo でどのように表示されるか  {#what-does-an-interesting-moment-look-like-in-marketo}

注目のアクションは、[リードのアクティビティログ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)に表示されます。

![](assets/using-interesting-moments-5.png)

## 注目のアクションは、Salesforce でどのように表示されるか  {#what-does-an-interesting-moment-look-like-in-salesforce}

[Marketo Sales Insight アプリをインストール](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)していれば、注目のアクションはリード、連絡先、アカウント、または商談ページに表示されます。また、Sales Insight ダッシュボードで、「リードフィード」、「最有望見込客」、「ウォッチリスト」にも表示されます。

![](assets/using-interesting-moments-6.png)

## 注目のアクションは、Salesforce1 でどのように表示されるか {#what-does-an-interesting-moment-look-like-in-salesforce-1}

Marketo Sales Insight for Salesforce1 をインストールまたは更新すると、リードの関連リンクの下に注目のアクションが表示されます。

![](assets/using-interesting-moments-7.png)

## 注目のアクションを購読 {#subscribe-to-interesting-moments}

「注目のアクション」タブまたはリードフィードで「購読」ボタンをクリックすると、注目のアクションを購読できます。 以下の手順は両方で同じです。

1. 「購読」アイコンをクリックします。 その後、「 E メール配信登録」タブに移動します。

1. 受け取る電子メールアラートの種類を、名前、アカウント、種類、説明のいずれかに基づいて選択できます。

1. アラートを送信する電子メールアドレスを選択します（自分/チームメンバー）

1. クリック **購読**.

![](assets/using-interesting-moments-8.png)
