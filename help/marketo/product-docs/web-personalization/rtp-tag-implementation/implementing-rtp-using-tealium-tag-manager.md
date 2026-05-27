---
unique-page-id: 9437340
description: dnlを使用したrtpの実装など、Marketo Engageのtealium tag managerを使用したrtpの実装について説明します。 このガイドを使用して、次のステップを完了してください。
title: Tealium タグマネージャーを使用した RTP の実装
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
TQID: https://experienceleague.adobe.com/zMs2Dii5RERdH8tKb86a6EhxXUx2IpbZkDOCklUvvY4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ea90ebee-5c84-42d9-8b21-006bdabc95a3id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 233
ht-degree: 89%

---

# [!DNL Tealium] タグマネージャーを使用した RTP の実装 {#implementing-rtp-using-tealium-tag-manager}

RTP タグを実装するには、次のインストール手順に従います。

1. [!DNL Tealium] タグマネージャーアカウントにログインします。

1. 「[!UICONTROL タグ]」タブに移動し、タグマーケットプレイスの「[!UICONTROL その他]」タブにある「[!UICONTROL Tealium カスタムコンテナタグ]」を追加します。

1. 「[!UICONTROL タイトル]」フィールドに、「**Marketo RTP**」と入力して「**[!UICONTROL 完了]**」をクリックします。

1. 変更を保存します。

   >[!NOTE]
   >
   >まだ新しいコンテナを公開する必要はありません。

1. プロファイルを保存したら、Tealium iQ コンソールの右上隅にある名前／メールアドレスをクリックします。

1. [!UICONTROL 管理者]メニューの「[!UICONTROL アカウント管理者]」で「**[!UICONTROL テンプレートを管理]**」をクリックします。

1. ドロップダウンリストから「**[!UICONTROL Tealium カスタムコンテナ]：Marketo RTP**」を選択して、タグテンプレートを開きます。

1. RTP アカウントにログインします。

1. 「[!UICONTROL アカウント設定]」に移動します。

   >[!NOTE]
   >
   >サポートから既に JavaScript タグを受け取っている場合は、手順 11 に進みます。

1. ドメインで、該当するドメインを選択し、「**[!UICONTROL タグの生成]**」をクリックします。

1. RTP JavaScript タグをコピーし、Tealium プロファイルテンプレートの「[!UICONTROL Start Tag Library Code]」と「[!UICONTROL End Tag Library Code]」の間に貼り付けます。

   >[!NOTE]
   >
   >**重要な手順**
   >
   >このファイルに配置するコードから `<!-- RTP tag -->` タグと `<!-- End of RTP tag -->` タグを削除します。
   >
   >このファイルに配置するコードから `<script type='text/javascript'>` タグと `</script>` タグを削除します。

1. 「**[!UICONTROL プロファイルテンプレートを保存]**」をクリックすると、新しいプロファイルが公開されます。
