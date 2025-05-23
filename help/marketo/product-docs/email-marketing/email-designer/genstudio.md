---
title: Marketo EngageのGenStudio統合
description: Marketo EngageでGenStudioを使用する方法を説明します。
hide: true
hidefromtoc: true
source-git-commit: f236f2cf73637ee1a0ee6062c1ecbf82f0e02130
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 16%

---

# Marketo EngageのGenStudio統合 {#work-with-experience-manager-assets}

Adobe GenStudio for Performance Marketingは、独自の広告やメールを作成し、ブランド標準に準拠し、企業ポリシーに準拠した、インパクトのあるパーソナライズされたマーケティングキャンペーンを推進できる、ジェネレーティブ AI ファーストのアプリケーションです。 コンテンツ作成の複雑さを簡素化する多くのツールを提供します。

>[!INFO]
>
>[GenStudio for Performance Marketing](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/home){target="_blank"} の詳細情報。

## Marketo EngageでのGenStudio機能の活用 {#leverage-genstudio-capabilities}

この統合により、Marketo Engageを使用してメールキャンペーンの開発と自動化を行うテクニカルマーケターは、GenStudioを使用してコンテンツを作成するパフォーマンスマーケターと共同作業ができるようになります。 これにより、GenStudioのオンブランドコンテンツをMarketo Engageに簡単に統合できます。

## Marketo EngageからGenStudioへのHTML テンプレートの書き出し {#export-an-html-template}

ブランドのガイドラインを含んだテンプレートをGenStudio for Performance Marketingに簡単に書き出すことができます。

1. Marketo Engageで、メールのコンテンツにアクセスします。

1. E メールDesignerで「**詳細**」ボタンをクリックし、「**HTMLを書き出し**」を選択します。

   スクリーンショット

1. 書き出したテンプレートをGenStudio for Performance Marketingに [HTMLをアップロード ](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/content/templates/use-templates#templates-from-ajo-and-marketo){target="_blank"} します。

1. GenStudio では、このテンプレートを使用して、AI プロンプトを含む複数のメールのバリエーションを作成し、保存します。

>[!NOTE]
>
>メールエクスペリエンスを作成する方法については、[GenStudio専用セクション ](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/create/create-email-experience){target="_blank"} を参照してください。

## Marketo EngageでのGenStudio Experience の活用 {#leverage-genstudio-experiences}

Marketo Engageに読み込むことで作成したGenStudio メールのバリエーションを活用するには、次の手順に従います。

1. Marketo Engageで、メールを作成します。

1. メールの詳細ページで、「**メール本文を編集**」をクリックして、メールDesignerを開きます。

1. **HTMLを読み込み** を選択し、「**Adobe GenStudio for Performance Marketing**」ボタンをクリックします。

   スクリーンショット

1. GenStudio エクスペリエンスを参照して、コンテンツの作成を開始します。エクスペリエンスは、条件（製品、ペルソナ、ブランド、さらにカラーなど）に基づいてフィルタリングできます。

1. エクスペリエンスを選択し、「**使用**」をクリックします。

スクリーンショット

1. GenStudio エクスペリエンスをインポートするフォルダーを選択します。

スクリーンショット

選択したコンテンツが E メールデザイナーに表示されます。

スクリーンショット

>[!NOTE]
>
>Marketo Engage テンプレートから作成されたGenStudio エクスペリエンスは、電子メールDesignerに直接読み込まれます。 GenStudio テンプレートを使用せずに作成されたMarketo Engage エクスペリエンスは、互換モードで読み込まれます。

[ メールコンテンツ編集ツール ](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#add-structure-and-content){target="_blank"} および [ パーソナライゼーションフィールド ](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#personalize-content){target="_blank"} を使用して、必要に応じてメールを編集します。
