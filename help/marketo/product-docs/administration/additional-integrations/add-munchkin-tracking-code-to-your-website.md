---
unique-page-id: 2360354
description: "Web サイトへの  [!DNL Munchkin]  トラッキングコードの追加 - Marketo ドキュメント - 製品ドキュメント"
title: "Web サイトへの  [!DNL Munchkin]  トラッキングコードの追加"
exl-id: a03a7f11-8d5e-4325-b975-8fc350711da0
feature: Administration, Munchkin Tracking Code
source-git-commit: bb9593ab500d57127f22b14757688d7521661e38
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 93%

---

# Web サイトへの [!DNL Munchkin] トラッキングコードの追加 {#add-munchkin-tracking-code-to-your-website}

Marketo のカスタム JavaScript トラッキングコード（[!DNL Munchkin] コードと呼ばれる）は、自社の web サイトを訪問したすべての個人をトラッキングして、自動化されたマーケティングキャンペーンで訪問に応答できるようにします。匿名の訪問者でも、IP アドレスなどの情報と共にトラッキングします。**このトラッキングコードがなければ、web サイトへの訪問やその他のアクティビティをトラッキングできません**。

>[!PREREQUISITES]
>
>経験豊富な JavaScript 開発者の協力を得るようにしてください。Marketo テクニカルサポートでは、カスタム JavaScript のトラブルシューティングについては対応できません。

## Web サイトへのトラッキングコードの追加 {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Adobe Experience Cloudユーザーは、 [AdobeLaunch でのMarketo統合](https://exchange.adobe.com/apps/ec/100223/adobe-launch-core-extension){target="_blank"} 含める [!DNL Munchkin] スクリプトを Web ページに配置できます。 AdobeLaunch を使用する場合、 _の [!DNL Munchkin] スクリプトが自動的に追加されました_&#x200B;を追加する必要はありません。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/add-munchkin-tracking-code-to-your-website-1.png)

1. 「**[!UICONTROL Munchkin]**」をクリックします。

   ![](assets/add-munchkin-tracking-code-to-your-website-2.png)

1. **[!UICONTROL トラッキングコードタイプ]**&#x200B;は「**[!UICONTROL 非同期]**」を選択します。

   ![](assets/add-munchkin-tracking-code-to-your-website-3.png)

   >[!NOTE]
   >
   >ほとんどの場合、非同期コードを使用する必要があります。[詳細情報](#types-of-munchkin-tracking-codes)

1. JavaScript のトラッキングコードをクリックしてコピーし、web サイトに貼り付けます。

   ![](assets/add-munchkin-tracking-code-to-your-website-4.png)

   >[!CAUTION]
   >
   >このスクリーンショットのコードは使用しないでください。ご自身のアカウントに表示される固有のコードを使用する必要があります。

   >[!TIP]
   >
   >トラッキングする web ページにトラッキングコードを貼り付けます。規模が小さいサイトの場合は、ページごとに貼り付けることも可能です。または動的に生成される web ページ、ユーザーフォーラムなどが多数あるサイトの場合は、主なページに貼り付けるだけでかまいません。

   最適な結果を得るには、非同期 [!DNL Munchkin] コードを使用して、ページの `<head>` 要素内に配置します。簡易コード（推奨しません）を使用する場合は、`</body>` タグの直前に貼りつけます。

   ![](assets/add-munchkin-tracking-code-to-your-website-5.png)

   >[!TIP]
   >
   >トラフィック量が非常に大きくなる（例：1 か月の訪問数が 10 万以上）サイトの場合、匿名の人物をトラッキングすることはお勧めしません。[詳細情報](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/){target="_blank"}.

## 複数のワークスペースを使用する場合のトラッキングコードの追加 {#add-tracking-code-when-using-multiple-workspaces}

Marketo アカウントで Workspaces を使用している場合、ワークスペースに対応した個々の web プレゼンスを使用していることも考えられます。その場合は、[!DNL Munchkin] トラッキングコードの JavaScript を使用して、適切なワークスペースおよびパーティションに匿名の人物を割り当てることができます。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/add-munchkin-tracking-code-to-your-website-6.png)

1. 「**[!UICONTROL Munchkin]**」をクリックします。

   ![](assets/add-munchkin-tracking-code-to-your-website-7.png)

1. トラッキングする web ページに適したワークスペースを選択します。

   ![](assets/add-munchkin-tracking-code-to-your-website-8.png)

   >[!NOTE]
   >
   >ワークスペースごとの [!DNL Munchkin] コードを使用しない場合、人物はアカウントの設定時に作成されたデフォルトのパーティションに割り当てられます。このパーティションの名前は、初期状態では「[!UICONTROL デフォルト]」ですが、Marketo アカウントで変更することもできます。

1. **[!UICONTROL トラッキングコードタイプ]**&#x200B;は「**[!UICONTROL 非同期]**」を選択します。

   ![](assets/add-munchkin-tracking-code-to-your-website-9.png)

1. JavaScript のトラッキングコードをクリックしてコピーし、web サイトに貼り付けます。

   ![](assets/add-munchkin-tracking-code-to-your-website-10.png)

   >[!CAUTION]
   >
   >このスクリーンショットのコードは使用しないでください。ご自身のアカウントに表示される固有のコードを使用する必要があります。

1. Web ページでトラッキングコードを貼り付ける場所は、`<head>` 要素内です。このページにアクセスした新しいリードは、このリードパーティションに割り当てられます。

   ![](assets/add-munchkin-tracking-code-to-your-website-11.png)

   >[!CAUTION]
   >
   >[!DNL Munchkin] のトラッキングスクリプトは、1 つのページの単一のパーティションおよびワークスペースに対して 1 つだけ使用できます。Web サイトの複数のパーティション／ワークスペースに、トラッキングスクリプトを追加しないようにします。

   >[!NOTE]
   >
   >Marketo で作成したランディングページには、自動的にトラッキングコードが追加されるので、このコードを貼り付ける必要はありません。

## [!DNL Munchkin] トラッキングコードのタイプ {#types-of-munchkin-tracking-codes}

[!DNL Munchkin] トラッキングコードは、以下の 3 つのタイプから選択できます。それぞれ、web ページの読み込み時間に対する影響が異なります。

1. **[!UICONTROL 簡易]**：コードの行数は最小限ですが、web ページの読み込み時間に関しては最適化されません。このコードは、web ページを読み込むたびに jQuery ライブラリーを読み込みます。
1. **[!UICONTROL 非同期]**：web ページの読み込み時間が短くなります。
1. **[!UICONTROL 非同期 jQuery]**：web ページの読み込み時間が短くなり、システムのパフォーマンスも向上します。既に jQuery があると想定し、チェックも読み込みも行いません。

## [!DNL Munchkin] コードのテスト {#test-if-your-munchkin-code-is-working}

[!DNL Munchkin] コードを追加後に、コードが機能していることを確認するには、以下の手順に従います。

1. Web ページにアクセスします。

1. [!DNL My Marketo] で、「**[!UICONTROL 分析]**」タイルをクリックします。

   ![](assets/add-munchkin-tracking-code-to-your-website-12.png)

1. 「**[!UICONTROL Web ページアクティビティ]**」をクリックします。

   ![](assets/add-munchkin-tracking-code-to-your-website-13.png)

1. 「**[!UICONTROL セットアップ]**」タブをクリックし、「**[!UICONTROL アクティビティソース]**」をダブルクリックします。

   ![](assets/add-munchkin-tracking-code-to-your-website-14.png)

1. [!UICONTROL アクティビティソース]を「**[!UICONTROL 匿名の訪問者（ISP を含む）]**」に変更し、「**[!UICONTROL 適用]**」をクリックします。

   ![](assets/add-munchkin-tracking-code-to-your-website-15.png)

1. 「**[!UICONTROL レポート]**」タブをクリックします。

   ![](assets/add-munchkin-tracking-code-to-your-website-16.png)

   >[!NOTE]
   >
   >データが表示されない場合は、数分待ってから、下部にある更新アイコンをクリックします。
