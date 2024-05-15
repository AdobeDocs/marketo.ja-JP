---
description: 質問の生成 – Marketo ドキュメント – 製品ドキュメント
title: 質問の生成
hide: true
hidefromtoc: true
feature: Dynamic Chat
exl-id: 05e0fd4c-b8e0-47de-8ca8-d4ba07d6a06a
source-git-commit: cc16ec5dd5c6671ba9265042e108d0ff76b0e16d
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# 質問の生成 {#question-generation}

すべてのタスクと、タスクが生成された日時、質問の総数、承認ステータスなどの関連する詳細を表示します。

## 質問の生成 {#generate-questions}

1. 「生成 AI」で、 **[!UICONTROL 支援応答]**.

   ![](assets/question-generation-1.png)

1. クリック **[!UICONTROL 質問の生成]**.

   ![](assets/question-generation-2.png)

1. タスクに名前を付け、すべてのコンテンツが抽出されるソース URL （最大 10）を入力します。 目的のトピック/キーワードを入力し、キーボードの Enter キーを押します。 完了したら、 **[!UICONTROL Generate]**.

   ![](assets/question-generation-3.png)

   >[!IMPORTANT]
   >
   >Marketo Engageが指定された URL からコンテンツを削除できるようにするには、まず複数の IP アドレスを許可リストに加えるする必要があります。 [詳しくは、以下を参照してください](#ip-addresses-to-allowlist).

1. コンテンツに基づいて、質問と応答の生成には、最大 30 分かかる場合があります。 「**[!UICONTROL OK]**」をクリックします。

   ![](assets/question-generation-4.png)

   >[!TIP]
   >
   >「更新」をクリックして、質問生成の最新のステータスを確認します。

   ![](assets/question-generation-5.png)

## 質問と回答のダウンロード {#download-questions-and-responses}

>[!NOTE]
>
>生成された質問と回答は、でも表示できます [応答ライブラリ](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. 目的のタスクを見つけて、名前の横にあるダウンロードアイコンをクリックします。

   ![](assets/question-generation-6.png)

1. ブラウザーでダウンロードフォルダーを見つけて、ファイルを選択します。 使用するブラウザーによって表示が異なる場合があります。

   ![](assets/question-generation-7.png)

1. Excel ファイルで、 **[!DNL Task details]** 質問や回答を追加/編集する方法を含む、タスクに関する様々な詳細を示します。

   ![](assets/question-generation-8.png)

   >[!NOTE]
   >
   >質問や回答を一括で追加/編集する場合、 [再アップロードする方法については、こちらを参照してください。](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. この **[!DNL Q&Rs]** タブには、生成された質問や回答など、追加の詳細が表示されます。

   ![](assets/question-generation-9.png)

## 許可リストへの IP アドレス {#ip-addresses-to-allowlist}

質疑応答の際に URL からコンテンツを抽出できるようにするには、以下のすべての IP アドレスが Web チームによって許可リストに加えるされていることを確認してください。

<table width="150">
  <tr>
    <td>20.167.0.149</td>
  </tr>
  <tr>
    <td>20.248.129.111</td>
  </tr>
  <tr>
    <td>20.167.0.146</td>
  </tr>
</table>
