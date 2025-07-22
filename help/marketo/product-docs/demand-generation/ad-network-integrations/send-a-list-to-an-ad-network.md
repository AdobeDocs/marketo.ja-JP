---
description: 広告ネットワークへのリストの送信 - Marketo ドキュメント - 製品ドキュメント
title: 広告ネットワークへのリストの送信
exl-id: d5c55df7-53c8-491a-9d79-ecf7c25cee08
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 67%

---

# 広告ネットワークへのリストの送信 {#send-a-list-to-an-ad-network}

静的リストを [!DNL LinkedIn]、[!DNL Facebook] またはGoogleに送信する方法を説明します。

## リストの送信方法 {#how-to-send-a-list}

1. Marketo で、リストを選択して、**[!UICONTROL リストアクション]**&#x200B;ドロップダウンをクリックして、「**[!UICONTROL 広告ネットワークに送信]**」を選択します。

   ![](assets/send-a-list-to-an-ad-network-1.png)

1. [!DNL LinkedIn]、[!DNL Facebook]、Googleのいずれかを選択します（現時点では、他のオプションは使用できません）。 この例では、「**[!DNL LinkedIn]**」を選択します。 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/send-a-list-to-an-ad-network-2.png)

1. **[!UICONTROL オーディエンス]** ドロップダウンをクリックし、目的のオーディエンスを選択します。

   ![](assets/send-a-list-to-an-ad-network-3.png)

   >[!TIP]
   >
   >確認する必要がある場合は、「ステータス」タブで、リストが同期されている宛先オーディエンスを確認できます。

1. 目的の [!UICONTROL &#x200B; プッシュタイプ &#x200B;] を選択し、「**[!UICONTROL 更新]**」をクリックします。

   ![](assets/send-a-list-to-an-ad-network-4.png)

   >[!NOTE]
   >
   >「[!UICONTROL &#x200B; 継続的なオーディエンス同期を有効にする &#x200B;] を選択した場合、Marketo インスタンスのリストが変更されるので、Marketoは選択した Ad Network のリストを最新の状態に保ちます。 静的リストに追加された人物、または静的リストから削除された人物の&#x200B;**両方**&#x200B;がオーディエンスに追加されます。

1. これで完了です。「**[!UICONTROL OK]**」をクリックして終了します。

   ![](assets/send-a-list-to-an-ad-network-5.png)

## よくある質問 {#faq}

**単一の静的リストを複数の広告オーディエンスと同期できますか？**

いいえ。リストは 1 つの宛先オーディエンスにのみ同期できます。

**既存の広告オーディエンスへの継続的な同期を有効にした場合、既存のオーディエンスは置き換えられますか。**

いいえ、既存のオーディエンスに追加されますが、置き換えられません。
