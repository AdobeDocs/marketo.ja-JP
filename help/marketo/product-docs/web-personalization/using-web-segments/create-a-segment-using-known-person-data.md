---
unique-page-id: 7504343
description: Marketo Engageの既知の人物データを使用して、既知の人物を使用してセグメントを作成する方法を説明します。 このガイドを使用して、次のステップを完了してください。
title: 認識済み顧客データを使用したセグメントの作成
exl-id: 429d8678-2e62-4b1e-bda1-675ff3a1aae2
feature: Web Personalization
TQID: 'https://experienceleague.adobe.com/I1rOpg5OueqFqd-ge7kYQsZiSmBuwYaXsNq-0xmS4fs'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
    internal-label: Personalization
  - id: 664d862c-1673-5ed4-a3d6-386ac83225e4
    internal-label: Web Personalization
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
    internal-label: Segmentation
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 86%
---
# 認識済み顧客データを使用したセグメントの作成 {#create-a-segment-using-known-person-data}

認識済み顧客データの値を使用してセグメントを作成する方法は、次のとおりです。

>[!PREREQUISITES]
>
>[リードデータの管理](/help/marketo/product-docs/web-personalization/using-web-segments/manage-person-data.md)

1. 「**[!UICONTROL セグメント]**」に移動します。

   ![](assets/new-dropdown-segments-hand-2.jpg)

1. 「**[!UICONTROL 新規作成]**」をクリックします。

   ![](assets/image2015-8-28-13-3a19-3a59.png)

1. セグメントの「名前」を入力します。

   ![](assets/image2015-8-28-13-3a2-3a59.png)

1. 「プロファイルのセグメント化」で、「**[!UICONTROL データベース]**」をキャンバスまでドラッグします。

   ![](assets/four-1.png)

1. ドロップダウンからリードデータフィールドを選択します。

   ![](assets/five-1.png)

1. リードデータの値を入力します。

   ![](assets/six.png)

   各フィールドには 1 つの値のみ指定できます。 例えば、「役職」フィールドに複数の値を追加する場合は、各値に同じフィールド名を持つ新しい行を作成する必要があります。 どの値でも一致するように、必ず OR 値を使用してください。

   ![](assets/seven-1.png)

## 複数の人物データフィールドを選択する {#selecting-multiple-person-data-fields}

1. リードデータフィールドを追加するには「**+**」をクリックします。

   ![](assets/eight.png)

1. [!UICONTROL AND] または [!UICONTROL OR] 演算子を選択します。 追加するフィールドを選択します。 人物データフィールドを選択します。 人物データの値を入力します。

   ![](assets/nine.png)

1. 「**[!UICONTROL 保存]**」をクリックしてセグメントを保存するか、「**[!UICONTROL 保存してキャンペーンを設定]**」をクリックして保存し、[!UICONTROL キャンペーン]ページに移動します。

   ![](assets/image2014-11-19-19-3a48-3a20-1.png)

   これで、認識済み顧客のデータをターゲティングするセグメントが設定されました。
