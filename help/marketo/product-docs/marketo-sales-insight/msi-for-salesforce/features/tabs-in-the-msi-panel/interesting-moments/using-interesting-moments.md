---
unique-page-id: 2951640
description: 注目のアクションの使用 - Marketo ドキュメント - 製品ドキュメント
title: 注目のアクションの使用
exl-id: ccf7664b-08e1-490a-a3f9-5fa3bd8fb05f
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 69%

---

# 注目のアクションの使用 {#using-interesting-moments}

興味深い瞬間は、[!DNL Marketo Sales Insight] アプリを通じてセールスチームとコミュニケーションを取るための鍵です。

>[!AVAILABILITY]
>
>これらは、[!DNL Marketo Sales Insight] および [[!DNL Marketo Sales Connect]](/help/marketo/product-docs/marketo-sales-connect/marketo/interesting-moments-in-sales-connect.md) のお客様のみが利用できます。

## 注目のアクションとは何でしょうか。 {#what-is-an-interesting-moment}

それは、あなた次第です。どんな情報がセールスチームに関係あるのかを自分で決定します。セールスチームがリードについて知りたいのは、例えば次のようなことです。

* Web サイトの価格設定ページへのアクセス
* 新製品発表メールに記載されたリンクをクリック
* 製品デモをリクエスト

## 注目のアクションを作成する方法  {#how-do-i-create-an-interesting-moment}

1. [スマートキャンペーン](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)を選択します。トリガーされた場合にセールスチームが興味を持つものがいいでしょう。

   ![](assets/using-interesting-moments-1.png)

1. **[!UICONTROL 注目のアクション]**&#x200B;フローステップをドラッグします。

   ![](assets/using-interesting-moments-2.png)

1. **タイプ** （[!UICONTROL  メール ]、[!UICONTROL  マイルストーン ] または [!UICONTROL Web]）を選択します。

   ![](assets/using-interesting-moments-3.png)

1. このアクションが重要である理由として、セールスチームへのメッセージを「**[!UICONTROL 説明]**」フィールドに記入します。

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

## [!DNL Salesforce] で興味深い瞬間は何に見えますか？  {#what-does-an-interesting-moment-look-like-in-salesforce}

アプリを [ インストール  [!DNL Marketo Sales Insight]  すると、リード ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) 連絡先、アカウント、商談のページに注目すべき瞬間が表示されます。 また、これらの指標は、リードフィード、リー [!DNL Sales Insight] ー、監視リストの [!DNL Best Bets] ダッシュボードにも表示されます。

![](assets/using-interesting-moments-6.png)

## [!DNL Salesforce1] で興味深い瞬間は何に見えますか？ {#what-does-an-interesting-moment-look-like-in-salesforce-1}

[!DNL Marketo Sales Insight] 用に [!DNL Salesforce1] をインストールまたは更新すると、リードの関連リンクの下に興味深い瞬間が表示されます。

![](assets/using-interesting-moments-7.png)

## 注目のアクションを購読 {#subscribe-to-interesting-moments}

興味深いモーメントを購読するには、「興味深いモーメント」タブまたはリードフィードで「[!UICONTROL  購読 ]」ボタンをクリックします。 以下の手順は両方で同じです。

1. 購読アイコンをクリックします。その後、「メール購読」タブに移動します。

1. [!UICONTROL  名前 ]、[!UICONTROL  アカウント ]、[!UICONTROL  タイプ ]、または [!UICONTROL  説明 ] に基づいて、受信するメールアラートのタイプを選択できます。

1. アラートを送信するメールアドレスを選択します（自分／チームメンバー）

1. 「**[!UICONTROL 購読]**」をクリックします。

>[!NOTE]
>
>注目のアクションのタイプまたは説明を購読する場合、ユーザは、そのタイプまたは説明に一致する注目のアクションをトリガーする際に、所有する人（リード／取引先責任者）に関するメール通知を受け取ります。

![](assets/using-interesting-moments-8.png)
