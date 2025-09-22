---
unique-page-id: 7504051
description: リードデータの管理 - Marketo ドキュメント - 製品ドキュメント
title: リードデータの管理
exl-id: 40f4aac8-c6e5-4cf3-9573-cac2fdf9bcad
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 100%

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

1. 削除アイコン（![—](assets/image2015-3-24-13-3a45-3a56.png)）をクリックして、リストからフィールドを削除します。「**[!UICONTROL はい]**」をクリックして、フィールドの削除を確認します。

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
   <td><p>Department</p></td>
   <td><p>Department</p></td>
  </tr>
  <tr>
   <td><p>title</p></td>
   <td><p>Title</p></td>
   <td><p>Job Title</p></td>
  </tr>
  <tr>
   <td><p>rating</p></td>
   <td><p>Rating</p></td>
   <td><p>Rating</p></td>
  </tr>
  <tr>
   <td><p>leadScore</p></td>
   <td><p>LeadScore</p></td>
   <td><p>Score</p></td>
  </tr>
  <tr>
   <td><p>leadStatus</p></td>
   <td><p>LeadStatus</p></td>
   <td><p>Status</p></td>
  </tr>
  <tr>
   <td><p>priority</p></td>
   <td><p>Priority</p></td>
   <td><p>Priority</p></td>
  </tr>
  <tr>
   <td><p>leadRole</p></td>
   <td><p>LeadRole</p></td>
   <td><p>Role</p></td>
  </tr>
  <tr>
   <td><p>unsubscribed</p></td>
   <td><p>登録解除済み</p></td>
   <td><p>登録解除済み</p></td>
  </tr>
 </tbody>
</table>

新しい [!DNL Web Personalization] アカウント用に、次のリードフィールドが標準で提供されています。

>[!MORELIKETHIS]
>
>[認識済み顧客のデータを使用したセグメントの作成](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-known-person-data.md)
