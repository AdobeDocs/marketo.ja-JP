---
unique-page-id: 10100266
description: ビジネス固有のユーザーのアクションを追跡するためのカスタムアクティビティの概要、カスタムオブジェクトとの違い、アクティビティとAPI実装の作成の2段階設定。
title: カスタムアクティビティについて
exl-id: 0bb74d9d-3a9d-4ef7-8c8c-2de36cd6190b
feature: Custom Activities
TQID: https://experienceleague.adobe.com/QwH82DomS1BDHbK3wfoP14N8xDBKZ28gOLyZ-L8fAeY
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 286
ht-degree: 53%

---

# カスタムアクティビティについて {#understanding-custom-activities}

リードが実行したアクションを、ビジネスに特化したカスタムアクティビティとしてトラックできます。

## アクティビティ {#what-are-activities}

ユーザーが組織とやり取りする方法はいくつかあります。 オーディエンスは、自社のweb サイトを訪問したり、展示会に参加したり、電子メールのリンクをクリックしたりします。 こうしたアクションがアクティビティです。どのようなアクションも Marketo で取得されるので、マーケティングチームはタイムリーで適切な内容の情報をどのように送信すればよいか、深く理解することができます。

## カスタムアクティビティ {#custom-activities}

カスタムアクティビティは、Marketoのフォーム、メール、ランディングページに関連しないアクティビティを追跡するのに役立ちます。 顧客が小切手を振り込んだタイミングを追跡するには、カスタムアクティビティを使用します。 ウェビナーへの参加時間を追跡するには、カスタムアクティビティを使用します。

>[!NOTE]
>
>カスタムアクティビティは、カスタムオブジェクトとは異なります。 値が変化する（例えば、「車の色」が青から赤に変化する）場合は、カスタムオブジェクトを使用します。 発生するタイミングをトラックする際に詳細が変わらない場合（例えば、「購入した車」）は、カスタムアクティビティを使用します。

## フィールド {#fields}

アクティビティに関連付ける[追加フィールド &#x200B;](/help/marketo/product-docs/administration/marketo-custom-activities/add-edit-delete-marketo-custom-activity-fields.md)を追加できます。 プライマリフィールドと同じように、スマートリストを絞り込む基準として使用できます。

## はじめに {#getting-started}

カスタムアクティビティは、標準のアクティビティと同じように機能します。 ただし、設定は2段階のプロセスです。

手順 1：[Marketo アカウントでカスタムアクティビティ](/help/marketo/product-docs/administration/marketo-custom-activities/create-a-custom-activity.md)を作成します。

手順2:Marketo APIを使用して作業する組織内の従業員は、その後、実装を開始できます。 詳しくは、[カスタムアクティビティの API](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities/operation/addCustomActivityUsingPOST) を参照してください。
