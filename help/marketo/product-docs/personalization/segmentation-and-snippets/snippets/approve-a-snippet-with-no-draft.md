---
unique-page-id: 10095644
description: 「ドラフトなし」オプションを使用してスニペットを承認する方法を説明します。 「承認時にすべてのアセットを更新」または「承認時にドラフトを作成」を選択し、スニペットを使用してアセットを更新する方法を制御します。
title: ドラフトなしのスニペットを承認する
exl-id: a06aa77a-68f1-41a4-b2bd-bf1882b81578
feature: Snippets
TQID: https://experienceleague.adobe.com/3vwVKLZIr-z7I22-WaEc4I75rb6luv2n8s1xP6v-q8A
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: d65b4a73-87a3-4d56-b638-74e74d9939ceid: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2: id: a1d50dda-6d94-4e16-8c30-5eb7181c4650id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: e0eb8757-182f-49f3-94a4-1587d16f5094id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 259
ht-degree: 87%

---

# ドラフトなしのスニペットを承認する {#approve-a-snippet-with-no-draft}

## スニペットを承認する {#approve-the-snippet}

スニペットが承認されるたびにドラフトなしがトリガーされます。 これには、他のワークスペースでアセットによって共有、または参照されるスニペットも含まれます。

1. **[!UICONTROL Design Studio]** に移動します。

   ![](assets/approve-the-snippet-1.png)

1. 目的のスニペットを見つけて選択します。

   ![](assets/approve-the-snippet-2.png)

1. **[!UICONTROL スニペットアクション]**&#x200B;ドロップダウンで、「**[!UICONTROL ドラフトを承認]**」を選択します。

   ![](assets/approve-the-snippet-3.png)

1. スニペットを承認ダイアログボックスでオプションを選択し、「**[!UICONTROL 承認]**」をクリックします。

   * **[!UICONTROL すべて更新]**：スニペットを使用して承認したアセットのドラフトを作成しません。 すべてのアセットが更新され、以前のステータスが維持されます。 画面の右上に進行状況を示すモジュールが表示され、これはいつでも閉じることができます。 再度開くには、スニペット名を右クリックして「承認ステータスの表示」を選択してください。
   * **[!UICONTROL ドラフトの作成]**：スニペットを使用して承認したアセットのドラフトを作成します。 スニペットの変更を先にレビューする必要がある場合は、このオプションを選択してください。 ドラフトはすべて、手動で承認する必要があります。

   ![](assets/approve-the-snippet-4.png)

   >[!NOTE]
   >
   >まだ使用されていない新しいスニペットの場合、このドラフトの承認画面は表示されません。 これは、スニペットが 1 つ以上のアセットで使用されると表示されます。

>[!CAUTION]
>
>この機能は、スニペット承認のワークフローで時間を節約するために用意されています。 制限事項があるので、注意してください。 詳しくは、[この記事](https://nation.marketo.com/t5/knowledgebase/no-draft-snippet-limitations-and-troubleshooting/ta-p/300799){target="_blank"}を参照してください。

>[!MORELIKETHIS]
>
>[スニペットでドラフトなしを有効にする](/help/marketo/product-docs/administration/users-and-roles/enable-no-draft-for-snippets.md){target="_blank"}
