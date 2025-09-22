---
unique-page-id: 7504343
description: 既知のリードデータを使用してセグメントを作成する - Marketo ドキュメント — 製品ドキュメント
title: 既知のリードデータを使用してセグメントを作成する
exl-id: 429d8678-2e62-4b1e-bda1-675ff3a1aae2
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 100%

---

# 既知のリードデータを使用してセグメントを作成する {#create-a-segment-using-known-person-data}

既知のリードデータ値を使用してセグメントを作成する方法は、以下のとおりです。

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

   各フィールドには 1 つの値のみ指定できます。例えば、「役職」フィールドに複数の値を追加する場合は、各値に同じフィールド名を持つ新しい行を作成する必要があります。どの値でも一致するように、必ず OR 値を使用してください。

   ![](assets/seven-1.png)

## 複数のリードデータフィールドを選択する {#selecting-multiple-person-data-fields}

1. リードデータフィールドを追加するには「**+**」をクリックします。

   ![](assets/eight.png)

1. [!UICONTROL AND] または [!UICONTROL OR] 演算子を選択します。追加するフィールドを選択します。複数のリードデータフィールドを選択します。リードデータの値を入力します。

   ![](assets/nine.png)

1. 「**[!UICONTROL 保存]**」をクリックしてセグメントを保存するか、「**[!UICONTROL 保存してキャンペーンを設定]**」をクリックして保存し、[!UICONTROL キャンペーン]ページに移動します。

   ![](assets/image2014-11-19-19-3a48-3a20-1.png)

   これで、認識済み顧客のデータをターゲットにするセグメントが設定されました。
