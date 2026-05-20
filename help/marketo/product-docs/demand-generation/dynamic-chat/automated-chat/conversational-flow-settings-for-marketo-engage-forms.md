---
description: Dynamic Chatの対話型フローを使用して、Marketo フォームを会話型にする方法について説明します。 フォームやリストのデータを使用して、ミーティングの予約やカスタム目標にリードを絞り込むことができます。
title: Marketo Engage フォームの対話型フローの設定
feature: Dynamic Chat
exl-id: 36d00862-4bb9-46fd-a5f8-69df7bf22ecf
TQID: https://experienceleague.adobe.com/1e2YHel2zDZX9Q6VRvak79Kdomb4ch22aRc--tY9jcA
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 299
ht-degree: 85%

---

# Marketo Engage フォームの対話型フローの設定{#conversational-flow-settings-for-marketo-engage-forms}

Marketo Engage フォームを Dynamic Chat 対話型フローと統合して、対話型にします。 フォームデータまたはスマートリストメンバーシップを使用して、会議の予約、ホワイトペーパーのリンクまたはカスタム目標に対して即座にリードを評価します。

>[!AVAILABILITY]
>
>スマートリストのメンバーまたはリストのメンバーの条件には、Dynamic Chat Prime が必要です。 詳しくは、アドビのアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

1. フォームを見つけて選択します（または新しいフォームを作成します）。

   ![](assets/conversational-flow-settings-1.png)

1. **[!UICONTROL ドラフトの編集]**&#x200B;をクリックします。

   ![](assets/conversational-flow-settings-2.png)

1. フォーム編集ページで、「**[!UICONTROL フォーム設定]**」、「**[!UICONTROL 設定]**」の順にクリックします。

   ![](assets/conversational-flow-settings-3.png)

1. 「**[!UICONTROL 対話型フロー設定]**」スライダーをクリックして有効にします。

   ![](assets/conversational-flow-settings-4.png)

1. デフォルトの選択モーダルが表示されます。 環境設定を選択します。 この例では、**[!UICONTROL 対話型フローを使用]**&#x200B;が選択されています。

   ![](assets/conversational-flow-settings-5.png)

1. 目的の&#x200B;**[!UICONTROL 対話型フロー]**&#x200B;と&#x200B;**[!UICONTROL 配信タイプ]**&#x200B;を選択します。

   ![](assets/conversational-flow-settings-6.png)

   >[!NOTE]
   >
   >[詳しくは、対話型フローを参照してください。](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-overview.md){target="_blank"}

   **オプションの手順**：「**[!UICONTROL 選択肢を追加]**」をクリックして、特定の条件を満たすチャット訪問者をターゲットにすることができます。 合計 10 個に対して最大 9 つの選択肢を追加できます。

   ![](assets/conversational-flow-settings-7.png)

   >[!NOTE]
   >
   >静的／スマートリストのメンバーとして資格を得るには、フォーム送信の前に訪問者のブラウザーを既知のユーザとして cookie にする必要があります。

   **オプションの手順**：各手順内の「**+**」記号をクリックして属性を追加すると、オーディエンスを絞り込むことができます（使用可能な属性は、フォームで選択したフィールドです）。 この例では、設定はカリフォルニア州のAdobe テクニカルライターをターゲットにしています。

   ![](assets/conversational-flow-settings-8.png)

   >[!NOTE]
   >
   >条件ロジックが「すべて」に設定されている場合は、資格を得るにはすべての属性が満たされる必要があることを意味します。 条件ロジックが「任意」に設定されている場合は、いずれかの属性で十分であることを意味します。

   **オプションの手順**：2 つ以上の選択肢を追加する場合は、上／下矢印をクリックして並べ替えることができます。

   ![](assets/conversational-flow-settings-9.png)

1. 完了したら、「**[!UICONTROL 終了]**」をクリックします。

   ![](assets/conversational-flow-settings-10.png)
