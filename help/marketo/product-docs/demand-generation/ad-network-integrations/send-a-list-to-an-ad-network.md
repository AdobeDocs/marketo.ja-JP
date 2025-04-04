---
description: 広告ネットワークへのリストの送信 - Marketo ドキュメント - 製品ドキュメント
title: 広告ネットワークへのリストの送信
exl-id: d5c55df7-53c8-491a-9d79-ecf7c25cee08
feature: Integrations
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 74%

---

# 広告ネットワークへのリストの送信 {#send-a-list-to-an-ad-network}

静的リストをLinkedIn、FacebookまたはGoogleに送信する方法について説明します。

## リストの送信方法 {#how-to-send-a-list}

1. Marketo Engageでリストを選択し、「**[!UICONTROL リストのアクション]**」ドロップダウンをクリックして、「**[!UICONTROL Ad Network に送信]**」を選択します。

   ![](assets/send-a-list-to-an-ad-network-1.png)

1. LinkedIn、Facebook、Google のいずれかを選択します（現時点では、その他のオプションは使用できません）。この例では、**[!UICONTROL LinkedIn]** を選択します。「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/send-a-list-to-an-ad-network-2.png)

1. **[!UICONTROL オーディエンス]** ドロップダウンをクリックし、目的のオーディエンスを選択します。

   ![](assets/send-a-list-to-an-ad-network-3.png)

   >[!TIP]
   >
   >確認する必要がある場合は、「ステータス」タブで、リストが同期されている宛先オーディエンスを確認できます。

1. 目的のプッシュタイプを選択し、「**[!UICONTROL アップデート]**」をクリックします。

   ![](assets/send-a-list-to-an-ad-network-4.png)

   >[!NOTE]
   >
   >「継続的なオーディエンスの同期を有効にする」を選択した場合、Marketo インスタンスでリストが変更されるため、Marketo は選択された広告ネットワークでリストを最新の状態に保ちます。静的リストに追加されたユーザーや静的リストから削除されたユーザーは、両方ともオーディエンスから追加 _および_ 削除します。

1. これで完了です。「**[!UICONTROL OK]**」をクリックして終了します。

   ![](assets/send-a-list-to-an-ad-network-5.png)

## よくある質問 {#faq}

**単一の静的リストを複数の広告オーディエンスと同期できますか？**

いいえ。リストは 1 つの宛先オーディエンスにのみ同期できます。

**既存の広告オーディエンスへの継続的な同期を有効にした場合、既存のオーディエンスは置き換えられますか。**

いいえ、既存のオーディエンスに追加されますが、置き換えられません。
