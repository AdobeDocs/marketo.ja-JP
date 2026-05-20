---
description: Marketoの購読解除チェックについて説明します。Marketoで購読解除したユーザーにメールを送信できないようにします。
title: Marketo 配信停止チェック
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
feature: Sales Insight Actions
TQID: https://experienceleague.adobe.com/RaIYKEVyjdeUlOa4paltYIS8NPZHi1XWTmO4IeLBy-o
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 149
ht-degree: 90%

---

# [!UICONTROL Marketo 登録解除チェック] {#marketo-unsubscribe-check}

[!UICONTROL Marketo 登録解除チェック]は、チームの Marketo への接続を使用して、Marketo のリード管理システムで登録解除になっているユーザにメールが送信されるのを防ぎます。 セールスユーザが [!DNL Marketo Sales] を使用してメールを送信すると、Marketo に対する API 呼び出しが実行され、そのメール ID が登録解除されているかどうかを確認します。 配信停止の場合、メール送信がブロックされます。

>[!NOTE]
>
>**管理者権限が必要**

## オンにする {#turning-it-on}

1. 歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/marketo-unsubscribe-check-1.png)

1. 「[!UICONTROL 管理者設定]」で、「**[!UICONTROL 登録解除]**」をクリックします。

   ![](assets/marketo-unsubscribe-check-2.png)

1. 「**[!UICONTROL 統合]**」タブをクリックします。 「[!UICONTROL Marketo 登録解除チェック]」セクションで、スライダーをクリックしてチェックを有効にします。

   ![](assets/marketo-unsubscribe-check-3.png)

## 留意事項 {#things-to-know}

Marketo 配信停止チェックの留意事項は次のとおりです。

* API の制限に対してはカウントしません
* Marketo 接続が確立されている必要があります
* グローバル設定です
* Web アプリケーション、メールクライアント、[!DNL Salesforce] から送信されるメールをブロックします
