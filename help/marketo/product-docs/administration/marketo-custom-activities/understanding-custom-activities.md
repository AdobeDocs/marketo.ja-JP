---
unique-page-id: 10100266
description: ビジネス固有のユーザーのアクションを追跡するためのカスタムアクティビティの概要、カスタムオブジェクトとの違い、アクティビティとAPI実装の作成の2段階設定。
title: カスタムアクティビティについて
exl-id: 0bb74d9d-3a9d-4ef7-8c8c-2de36cd6190b
feature: Custom Activities
TQID: 'https://experienceleague.adobe.com/QwH82DomS1BDHbK3wfoP14N8xDBKZ28gOLyZ-L8fAeY'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
    internal-label: Implementation
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: a8c137b3-8aa5-433e-bdc9-0a216c2a11c1
    internal-label: Custom activities
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 53%
---
# カスタムアクティビティについて {#understanding-custom-activities}

カスタムアクティビティを使用すると、リードがビジネスに特化して実行したアクションをトラッキングできます。

## アクティビティ {#what-are-activities}

ユーザーが組織とやり取りする方法はいくつかあります。 オーディエンスは、自社のweb サイトを訪問したり、展示会に参加したり、電子メールのリンクをクリックしたりします。 こうしたアクションがアクティビティです。どのようなアクションも Marketo によって取得されるので、マーケティングチームは、タイムリーで関連性の高い情報をどのように送信すればよいかをより深く理解できます。

## カスタムアクティビティ {#custom-activities}

カスタムアクティビティは、Marketoのフォーム、メール、ランディングページに関連しないアクティビティを追跡するのに役立ちます。 顧客が小切手を振り込んだタイミングを追跡するには、カスタムアクティビティを使用します。 ウェビナーへの参加時間を追跡するには、カスタムアクティビティを使用します。

>[!NOTE]
>
>カスタムアクティビティは、カスタムオブジェクトとは異なります。 値が変更される場合（例えば、「車の色」が青から赤に変更される場合）は、カスタムオブジェクトを使用します。 発生するタイミングをトラックする際に詳細が変わらない場合（例えば、「購入した車」）は、カスタムアクティビティを使用します。

## フィールド {#fields}

アクティビティに関連付ける[追加フィールド &#x200B;](/help/marketo/product-docs/administration/marketo-custom-activities/add-edit-delete-marketo-custom-activity-fields.md)を追加できます。 プライマリフィールドと同じように、スマートリストのフィルター条件として使用できます。

## はじめに {#getting-started}

カスタムアクティビティは、標準のアクティビティと同じように機能します。 ただし、設定は2段階のプロセスです。

手順 1：[Marketo アカウントでカスタムアクティビティ](/help/marketo/product-docs/administration/marketo-custom-activities/create-a-custom-activity.md)を作成します。

手順2:Marketo APIを使用して作業する組織内の従業員は、その後、実装を開始できます。 詳しくは、[カスタムアクティビティの API](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities/operation/addCustomActivityUsingPOST) を参照してください。
