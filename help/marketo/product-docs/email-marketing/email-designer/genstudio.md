---
title: Marketo Engage の GenStudio の統合
description: Marketo EngageのGenStudioを使用して、コンテンツを制作する方法を説明します。 電子メールDesignerワークフロー内でGenStudio機能にアクセスします。
solution: Marketo Engage
product: marketo
level: Beginner, Intermediate
feature: Email Designer
exl-id: bb15b18e-9a17-4dee-87f4-12f216dd3545
TQID: https://experienceleague.adobe.com/opg2aUcpf3QCiu5TazxPMfihsp6DPrRtekX3RicGg-M
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 449
ht-degree: 17%

---

# Marketo Engage の GenStudio の統合 {#genstudio-integration-for-marketo-engage}

Adobe GenStudio for Performance Marketingは、独自の広告やメールを作成し、ブランド基準を満たし、企業のポリシーに準拠した、インパクトのあるパーソナライズされたマーケティング施策を推進できる、生成AIを活用したアプリケーションです。 コンテンツ制作の複雑さを簡素化する多くのツールを提供します。

>[!AVAILABILITY]
>
>この機能を利用するには：
>
>* IMS組織は、Marketo Engageと同じIMS組織でGenStudio for Performance Marketingを使用してプロビジョニングする必要があります（詳しくは、アカウントマネージャーにお問い合わせください）
>* GenStudio for Performance Marketingの使用権限（System Manager、Editor、または共同作業者の製品プロファイル）が必要です

>[!INFO]
>
>[GenStudio for Performance Marketing](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/home){target="_blank"}の詳細をご覧ください。

## Marketo EngageのGenStudio機能を活用する {#leverage-genstudio-capabilities}

この統合により、Marketo Engageを使用してメールキャンペーンを開発および自動化するテクニカルマーケターは、GenStudioを使用してコンテンツを制作するパフォーマンスマーケターと協力することができます。 これにより、GenStudioのブランドに即したコンテンツをMarketo Engageに簡単に統合できます。

## Marketo EngageからGenStudioへのHTML テンプレートの書き出し {#export-an-html-template}

ブランドのガイドラインを含むテンプレートをGenStudio for Performance Marketingに簡単に書き出すことができます。

1. Marketo Engageで、メールの内容にアクセスします。

1. 電子メールDesignerで、「**詳細**」ボタンをクリックし、「**HTMLを書き出し**」を選択します。

   ![HTMLの書き出し](assets/genstudio-integration-1.png)

1. [書き出したHTML](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/content/templates/use-templates#templates-from-ajo-and-marketo){target="_blank"}のテンプレートをGenStudio for Performance Marketingにアップロードします。

1. GenStudioでは、このテンプレートを使用して、AI プロンプトを使用して[いくつかの電子メールのバリエーション ](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/create/create-email-experience){target="_blank"}を作成し、保存します。

## Marketo EngageでのGenStudio体験の活用 {#leverage-genstudio-experiences}

Marketo Engageに読み込んで作成したGenStudio メールのバリエーションを活用するには、次の手順に従います。

1. Marketo Engageで、[電子メールを作成](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#create-an-email)。

1. メールの詳細ページで、**メールコンテンツの編集**&#x200B;をクリックします。

   ![電子メールコンテンツの編集ボタン ](assets/genstudio-integration-2.png)

1. 「**HTMLを読み込み**」を選択します。

   ![HTMLの読み込みボタン ](assets/genstudio-integration-3.png)

1. 「**Adobe GenStudio for Performance Marketing**」ボタンをクリックします。

   ![Adobe GenStudio for Performance Marketing ボタン ](assets/genstudio-integration-4.png)

1. GenStudio エクスペリエンスを参照して、コンテンツの作成を開始します。 商品、ペルソナ、ブランド、さらには色などの基準でエクスペリエンスをフィルタリングすることができます。

1. エクスペリエンスを選択し、「**使用**」をクリックします。

   ![目的のエクスペリエンスを選択](assets/genstudio-integration-5.png){width="800" zoomable="yes"}

1. 選択したコンテンツが E メールデザイナーに表示されます。

   ![E メールデザイナー](assets/genstudio-integration-6.png){width="800" zoomable="yes"}

>[!NOTE]
>
>Marketo Engage テンプレートから作成されたGenStudio エクスペリエンスは、メールDesignerに直接読み込まれます。 Marketo Engage テンプレートなしで作成されたGenStudio エクスペリエンスは、互換モードで読み込まれます。

[ メールコンテンツ編集ツール ](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#add-structure-and-content){target="_blank"}と[ パーソナライゼーションフィールド ](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#personalize-content){target="_blank"}を使用して、必要に応じてメールを編集します。
