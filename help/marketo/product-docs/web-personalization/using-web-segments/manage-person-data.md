---
unique-page-id: 7504051
description: 人物データの管理や人物データの管理など、Marketo Engageでの人物データの管理について説明します。 このガイドを使用して、次のステップを完了してください。
title: リードデータの管理
exl-id: 40f4aac8-c6e5-4cf3-9573-cac2fdf9bcad
feature: Web Personalization
TQID: https://experienceleague.adobe.com/rIiC-JXLkaMByk7GizVOcCEcUHN8AL-8Hy66-U2GZhs
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 213
ht-degree: 89%

---

# リードデータの管理 {#manage-person-data}

セグメントで使用する人物のフィールドを選択して、[!DNL Web Personalization] で人物のデータを活用します。

1. 「**[!UICONTROL アカウント設定]**」に移動します。

   ![](assets/image2015-5-7-15-3a17-3a23.png)

1. **[!UICONTROL データベース]**&#x200B;に移動します。

   ![](assets/account-settings-dropdown-database.jpg)

## 新しいリードフィールドの追加 {#adding-a-new-person-field}

1. **追加するフィールド**&#x200B;をドロップダウンから選択して、リードデータフィールドをリストに追加します。

   ![](assets/add-a-person-field-hand.jpg)

   >[!NOTE]
   >
   >新しいフィールドが保留状態で追加されます。アクティブ化には最大 24 時間かかる場合があります。

## リードフィールドの削除 {#deleting-a-person-field}

1. 削除アイコン（![—](assets/image2015-3-24-13-3a45-3a56.png)）をクリックして、リストからフィールドを削除します。 「**[!UICONTROL はい]**」をクリックして、フィールドの削除を確認します。

   ![](assets/web-engagement-settings-delete.jpg)

   >[!NOTE]
   >
   >**リードデータフィールドの管理**
   >
   >* リードデータフィールドのみを含めることができます
   >* リードデータフィールドは最大 30 個まで追加できます
   >* 新規フィールドを追加した場合、アクティベーションには最大で 24 時間かかります
   >* 文字列タイプの上限は 255 文字です
   >* 非表示のフィールドは自動的に削除されます

<table>
 <tbody>
  <tr>
   <th><p>REST API 名</p></th>
   <th><p>SOAP API 名</p></th>
   <th><p>フレンドリ名</p></th>
  </tr>
  <tr>
   <td><p>department</p></td>
   <td><p>部門</p></td>
   <td><p>部門</p></td>
  </tr>
  <tr>
   <td><p>title</p></td>
   <td><p>役職</p></td>
   <td><p>役職</p></td>
  </tr>
  <tr>
   <td><p>rating</p></td>
   <td><p>評価</p></td>
   <td><p>評価</p></td>
  </tr>
  <tr>
   <td><p>leadScore</p></td>
   <td><p>LeadScore</p></td>
   <td><p>スコア</p></td>
  </tr>
  <tr>
   <td><p>leadStatus</p></td>
   <td><p>LeadStatus</p></td>
   <td><p>ステータス</p></td>
  </tr>
  <tr>
   <td><p>優先度</p></td>
   <td><p>優先度</p></td>
   <td><p>優先度</p></td>
  </tr>
  <tr>
   <td><p>leadRole</p></td>
   <td><p>LeadRole</p></td>
   <td><p>役割</p></td>
  </tr>
  <tr>
   <td><p>unsubscribed</p></td>
   <td><p>配信停止完了</p></td>
   <td><p>配信停止完了</p></td>
  </tr>
 </tbody>
</table>

新しい [!DNL Web Personalization] アカウント用に、次のリードフィールドが標準で提供されています。

>[!MORELIKETHIS]
>
>[認識済み顧客のデータを使用したセグメントの作成](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-known-person-data.md)
