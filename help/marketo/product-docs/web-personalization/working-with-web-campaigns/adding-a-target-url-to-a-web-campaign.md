---
unique-page-id: 6094879
description: webにターゲット URLを追加するなど、Marketo Engageでweb キャンペーンにターゲット URLを追加する方法について説明します。 このガイドを使用して、次のステップを完了してください。
title: Web キャンペーンへのターゲット URL の追加
exl-id: 5fbb3f12-1474-46c3-8315-8d081422e154
feature: Web Personalization
TQID: 'https://experienceleague.adobe.com/IrYPeEwQnyczC1KUGtKvKfmQ-gKTOqCIEVtZr9usCgk'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
    internal-label: Personalization
  - id: 664d862c-1673-5ed4-a3d6-386ac83225e4
    internal-label: Web Personalization
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 89%
---
# Web キャンペーンへのターゲット URL の追加 {#adding-a-target-url-to-a-web-campaign}

ターゲット URL は、キャンペーン設定ページ内にあり、web キャンペーンを表示する特定の URL（複数可）を定義します。

## ダイアログまたはウィジェット web キャンペーン用のターゲット URL の追加 {#adding-a-target-url-for-dialog-or-widget-web-campaigns}

1. 「**[!UICONTROL Web キャンペーン]**」に移動します。

   ![](assets/web-campaigns-hand-5.jpg)

1. 「**[!UICONTROL Web キャンペーンの新規作成]**」を選択します。

   ![](assets/create-new-web-campaign-hand.jpg)

1. **[!UICONTROL キャンペーン名]**&#x200B;を追加します。 **[!UICONTROL ターゲットセグメント]**&#x200B;を選択します。 **[!UICONTROL ターゲット URL]** を追加します。

   ![](assets/set-web-campaign-hands.jpg)

<table>
 <thead>
  <tr>
   <th colspan="1" rowspan="1">名前</th>
   <th colspan="1" rowspan="1">説明</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td colspan="1" rowspan="1"><strong>[!UICONTROL 任意のページ]</strong></td>
   <td colspan="1" rowspan="1"><p>任意のページにキャンペーンを表示できるようにします。</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>[!UICONTROL 一致時に URL パラメーターを含める]</strong></p></td>
   <td colspan="1" rowspan="1">URL パラメーターを追加して、一致させ、このパラメーターを含む URL でキャンペーンを表示します。 例： campaign=cpc</td>
  </tr>
 </tbody>
</table>

## ターゲット URL への複数の URL の追加 {#adding-multiple-urls-to-target-url}

プラスアイコン（![--](assets/image2015-2-18-8-3a40-3a59.png)）をクリックすると、[!UICONTROL 複数の値を入力]ダイアログが開き、複数の URL を追加できます。 1 行に 1 つの URL を追加します。

![](assets/image2015-2-23-18-3a15-3a57.png)

>[!NOTE]
>
>* ダイアログおよびウィジェット web キャンペーンでは任意のページとワイルドカード（&#42;）オプションを使用できます。
>* 高度なユースケースでは、In Zone web キャンペーンで URL パスの末尾にワイルドカードを使用できます。 例：[www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)
>* URL では大文字と小文字が区別されます

## In Zone web キャンペーン用のターゲット URL の追加 {#adding-a-target-url-for-in-zone-web-campaigns}

1. 「**[!UICONTROL Web キャンペーン]**」に移動します。

   ![](assets/web-campaigns-hand-5.jpg)

1. 「**[!UICONTROL Web キャンペーンの新規作成]**」を選択します。

   ![](assets/create-new-web-campaign-hand.jpg)

1. **[!UICONTROL キャンペーン名]**&#x200B;を追加します。 **[!UICONTROL ターゲットセグメント]**&#x200B;を選択します。 **[!UICONTROL ターゲット URL]** を追加します。

   >[!NOTE]
   >
   >ゾーン内のターゲット URL は、特定の URL を 1 つ以上定義する必要があります。 高度なユースケースでは、In Zone web キャンペーンで URL パスの末尾にワイルドカードを使用できます。 例：[www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)

   ![](assets/set-web-campaign-multiple-hands.jpg)

>[!MORELIKETHIS]
>
>* [ダイアログキャンペーンを作成する](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
>* [RTP ゾーン内キャンペーンを作成する](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
>* [RTP ウィジェットキャンペーンを作成する](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
