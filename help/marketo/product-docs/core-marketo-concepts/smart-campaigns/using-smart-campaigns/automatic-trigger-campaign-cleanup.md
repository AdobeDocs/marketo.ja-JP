---
unique-page-id: 1147074
description: トリガーキャンペーンの自動クリーンアップについて詳しく見る。 Marketoで古いトリガーキャンペーンをクリーンアップする方法について説明します。
title: 自動トリガーキャンペーンクリーンアップ
exl-id: 08012b55-e241-4524-a387-9644f5a2b17e
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/KygJNZIAwzO7OzNBHiVwXAylH7mRg31v-bPII53SFD8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 258
ht-degree: 70%

---

# 自動トリガーキャンペーンクリーンアップ {#automatic-trigger-campaign-cleanup}

Marketoには、アクティビティを取得しなくなったスマートキャンペーンを無効にする便利なサービスと無料のサービスがあります。 これにより、システム全体のパフォーマンスが向上するとともに、該当するキャンペーンを探して無効化する時間を節約できます。

## どのような処理が行われますか？ {#what-happens}

四半期に1回、Marketoは6か月以上休眠状態にある（ユーザーなし）スマートキャンペーンを見つけて非アクティブ化します。

## 無効化する際に、先に通知してもらえますか？ {#will-you-notify-me-first}

もちろんです。 3 か月に 1 回、無効化する予定のあらゆるキャンペーンを表示する通知を、その 1 週間前に送信します。

1. 「**[!UICONTROL 通知]**」アイコンをクリックします。

   ![](assets/automatic-trigger-campaign-cleanup-1.png)

1. 「**[!UICONTROL 予定されているアイドルトリガーキャンペーンクリーンアップ]**」をクリックします。 次に、「**[!UICONTROL これらのアイドルトリガーキャンペーンが無効化されます]**」リンクをクリックします。

   ![](assets/automatic-trigger-campaign-cleanup-2.png)

   非アクティブ化がスケジュールされているスマートキャンペーンのリストが表示されます。

   ![](assets/automatic-trigger-campaign-cleanup-3.png)

## 無効化されるキャンペーンはどのようなものですか？ {#which-campaigns-will-be-deactivated}

トリガーキャンペーンのうち、6 か月以上アクティブであるが、その期間に対象になったリードが 0 であるものだけが無効化されます。

## 待ってください。 このキャンペーンは無効化したくありません。 {#wait-not-this-campaign}

ご安心ください。スマートキャンペーンの時計は、次の方法でリセットできます。

* キャンペーンの条件を満たすリード。
* キャンペーンを手動で無効化してから、再び有効化する。

どちらの場合も、6 か月のカウンターがリセットされます。

## Marketo が無効化したキャンペーンを確認できますか？ {#will-you-let-me-know-which-campaigns-were-deactivated}

もちろんです。最初の通知から 1 週間後に、（最低 1 人のリードが条件を満たしたもの、または無効化されてから再び有効化されたものを除き）リストされたキャンペーンが無効化されたら、確認の通知が発行されます。

1. 「**[!UICONTROL 予定されているアイドルトリガーキャンペーンクリーンアップ]**」通知を選択します。 「**[!UICONTROL これらのアイドルトリガーキャンペーン]**」リンクをクリックします。

   ![](assets/automatic-trigger-campaign-cleanup-4.png)

1. 無効化されたキャンペーンのリストが表示されます。

   ![](assets/automatic-trigger-campaign-cleanup-5.png)
