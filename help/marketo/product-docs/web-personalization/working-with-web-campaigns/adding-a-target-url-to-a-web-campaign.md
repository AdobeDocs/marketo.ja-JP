---
unique-page-id: 6094879
description: Web キャンペーンへのターゲット URL の追加 - Marketo ドキュメント - 製品ドキュメント
title: Web キャンペーンへのターゲット URL の追加
exl-id: 5fbb3f12-1474-46c3-8315-8d081422e154
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 90%

---

# Web キャンペーンへのターゲット URL の追加 {#adding-a-target-url-to-a-web-campaign}

ターゲット URL はキャンペーンを設定ページの下に配置され、web キャンペーンを表示する特定の URL を 1 つ以上定義します。

## ダイアログまたはウィジェット web キャンペーン用のターゲット URL の追加 {#adding-a-target-url-for-dialog-or-widget-web-campaigns}

1. 「**[!UICONTROL Web キャンペーン]**」に移動します。

   ![](assets/web-campaigns-hand-5.jpg)

1. 「**[!UICONTROL Web キャンペーンの新規作成]**」を選択します。

   ![](assets/create-new-web-campaign-hand.jpg)

1. **[!UICONTROL キャンペーン名]**&#x200B;を追加します。**[!UICONTROL ターゲットセグメント]**&#x200B;を選択します。**[!UICONTROL ターゲット URL]** を追加します。

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
   <td colspan="1" rowspan="1"><strong>[!UICONTROL 任意のページ &#x200B;]</strong></td> 
   <td colspan="1" rowspan="1"><p>任意のページにキャンペーンを表示できるようにします。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>[!UICONTROL 一致時に URL パラメーターを含める &#x200B;]</strong></p></td> 
   <td colspan="1" rowspan="1">URL パラメーターを追加して、一致させ、このパラメーターを含む URL でキャンペーンを表示します。例：campaign=cpc</td> 
  </tr> 
 </tbody> 
</table>

## ターゲット URL への複数の URL の追加 {#adding-multiple-urls-to-target-url}

プラスアイコン（![—](assets/image2015-2-18-8-3a40-3a59.png)）をクリックすると、[!UICONTROL &#x200B; 複数値エントリ &#x200B;] ダイアログが開き、複数の URL を追加できます。 1 行に 1 つの URL を追加します。

![](assets/image2015-2-23-18-3a15-3a57.png)

>[!NOTE]
>
>* ダイアログおよびウィジェット web キャンペーンでは任意のページとワイルドカード（&#42;）オプションを使用できます。
>* 高度な使用例では、ゾーン内 web キャンペーンで URL パスの終わりにワイルドカードを使用できます。例：[www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)
>* URL では大文字と小文字が区別されます

## ゾーン内 web キャンペーン用のターゲット URL の追加 {#adding-a-target-url-for-in-zone-web-campaigns}

1. 「**[!UICONTROL Web キャンペーン]**」に移動します。

   ![](assets/web-campaigns-hand-5.jpg)

1. 「**[!UICONTROL Web キャンペーンの新規作成]**」を選択します。

   ![](assets/create-new-web-campaign-hand.jpg)

1. **[!UICONTROL キャンペーン名]**&#x200B;を追加します。**[!UICONTROL ターゲットセグメント]**&#x200B;を選択します。**[!UICONTROL ターゲット URL]** を追加します。

   >[!NOTE]
   >
   >ゾーン内のターゲット URL は、特定の URL を 1 つ以上定義する必要があります。高度な使用例では、ゾーン内 web キャンペーンで URL パスの終わりにワイルドカードを使用できます。例：[www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)

   ![](assets/set-web-campaign-multiple-hands.jpg)

>[!MORELIKETHIS]
>
>* [ダイアログキャンペーンを作成する](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
>* [RTP ゾーン内キャンペーンを作成する](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
>* [RTP ウィジェットキャンペーンを作成する](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
