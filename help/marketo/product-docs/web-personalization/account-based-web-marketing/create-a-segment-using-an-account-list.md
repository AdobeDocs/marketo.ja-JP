---
unique-page-id: 4720236
description: Marketo Engageでアカウントリストを使用してセグメントを作成する方法を説明します。 このガイドを使用して、次のステップを完了してください。
title: アカウントリストを使用したセグメントの作成​
exl-id: 73179ed9-2f9b-46df-abfa-6e8ebb645cc5
feature: Web Personalization
TQID: 'https://experienceleague.adobe.com/zhhNc7H7KwSbYiNJXSZcqqMylcwm5VeYe-gPaZdGqd0'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
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
source-wordcount: '215'
ht-degree: 68%
---
# アカウントリストを使用したセグメントの作成&#x200B; {#create-a-segment-using-an-account-list}

アカウントリストを使用してセグメントを作成する方法です。

>[!PREREQUISITES]
>
>[新規アカウントリストの作成](/help/marketo/product-docs/target-account-management/target/account-lists.md)

>[!NOTE]
>
>Web Personalization内でアカウントリストを表示するには、「Web ABM」という追加のモジュールが必要です。 アカウントリストが表示されない場合は、Adobe アカウントチーム（アカウントマネージャー）にお問い合わせください。

1. 「**[!UICONTROL セグメント]**」に移動します。

   ![](assets/new-dropdown-segments-hand-no-account-list.jpg)

1. 「**[!UICONTROL 新規作成]**」をクリックします。

   ![](assets/image2014-11-19-19-3a33-3a47.png)

1. セグメントの名前を入力します。 **[!UICONTROL ファーモグラフィック]**&#x200B;セクションから&#x200B;**[!UICONTROL 顧客リスト]**&#x200B;をドラッグ＆ドロップします。

   ![](assets/set-segment-hands.jpg)

1. アップロードした重点アカウントのリストからアカウントリストを選択します。 アカウントリスト名の横にある角括弧内の数字は、API 参照用のリスト ID です。

   ![](assets/select-list-for-segment-hands.jpg)

   >[!NOTE]
   >
   >アカウントリストは、セグメント化で使用できるように ABM から web パーソナライゼーションに同期されます。 ドロップダウンから選択してください。 同期には最大で 5 分かかります。 アカウントリストに 1 つ以上の重点アカウントが存在する場合にのみ同期されます。

1. 「**[!UICONTROL 保存]**」をクリックするか「**[!UICONTROL 保存してキャンペーンを設定]**」をクリックして、キャンペーンページに移動します。

   ![](assets/image2014-11-19-19-3a48-3a20.png)

これで完了です。 アカウントリストをターゲティングするセグメントを設定しました。
