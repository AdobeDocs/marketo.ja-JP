---
description: Response Library - Marketo ドキュメント – 製品ドキュメント
title: 応答ライブラリ
hide: true
hidefromtoc: true
feature: Dynamic Chat
exl-id: 774346fa-f633-48e8-a489-999404b6070b
source-git-commit: cc16ec5dd5c6671ba9265042e108d0ff76b0e16d
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 4%

---

# 応答ライブラリ {#response-library}

1 か所で、すべての質問、承認ステータス、割り当てられたタスク名/トピックを表示します。

## 質問を手動で追加 {#manually-add-a-question}

1. 「生成 AI」で、 **[!UICONTROL 支援応答]**.

   ![](assets/response-library-1.png)

1. 「」をクリックします **[!UICONTROL 応答ライブラリ]** タブ。

   ![](assets/response-library-2.png)

1. クリック **[!UICONTROL 質問を追加]**.

   ![](assets/response-library-3.png)

1. 質問と回答を入力します。 トピックを割り当て、ユーザーが訪問者と共有できるオプションの URL を追加します。 終了したら「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/response-library-4.png)

1. 「更新」をクリックすると、新しい質問がステータス「」で上部に表示されます[!UICONTROL 処理].」と入力します。

   ![](assets/response-library-5.png)

1. 数分後、もう一度更新すると、ステータスは「承認済み」に変わります。

   ![](assets/response-library-6.png)

## 個々の質問/応答の編集 {#generate-a-new-question}

>[!NOTE]
>
>生成されたすべての質問と回答には、「」が割り当てられます[!UICONTROL レビューが必要]デフォルトでは「ステータス。 Only ``[!UICONTROL 承認済み]」の質問と回答が、訪問者とのチャットに利用できるようになりました。

1. が含まれる **[!UICONTROL 応答ライブラリ]**&#x200B;を選択し、目的の質問をクリックします。

   ![](assets/response-library-7.png)

1. 編集を行い、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/response-library-8.png)

## 質問/回答の一括編集とアップロード {#bulk-edit-and-upload-questions-responses}

ダウンロードした Excel ファイルを一括編集する方法は以下の通りです。 これらは、ファイルの「タスクの詳細」タブでも確認できます。

<table>
<thead>
  <tr>
    <th>アクション</th>
    <th>入力ガイド</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>質問の編集</td>
    <td>「editedQuestion」列（列 H）に新しい質問を入力します。</td>
  </tr>
  <tr>
    <td>応答の編集</td>
    <td>「editedResponse」列（列 I）に新しい応答を入力します</td>
  </tr>
  <tr>
    <td>新しい質問を追加</td>
    <td>「editedQuestion」列（列 H）に新しい質問を入力し、questionResponsed を空白のままにします。 また、適切なトピックを「topics」列（列 C）に、ソース URL を「sourceUr!」列に入力する必要があります。</td>
  </tr>
  <tr>
    <td>質問と回答を追加</td>
    <td>「editedQuestion」列（列 H）に新しい質問を入力し、「editedResponse」列（列 I）に新しい応答を入力して、questionResponse を空白のままにします。 また、列「topics」（列 C）に適切なトピックを入力する必要があります</td>
  </tr>
</tbody>
</table>

1. ファイルの編集が完了したら、に戻ります **[!UICONTROL 応答ライブラリ]** tab キーを押してクリック **[!UICONTROL 応答をアップロード]**.

   ![](assets/response-library-9.png)

1. 該当するタスク名を入力します。 ファイルをドラッグ&amp;ドロップするか、デバイスで参照して選択します。 終了したら「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/response-library-10.png)

1. 確認が表示され、準備が完了しました。

   ![](assets/response-library-11.png)

## 質問をフィルタリング {#filter-your-questions}

デフォルトでは、質問は作成日時の順序でリストされ、最新の質問が最初に表示されます。 特定の質問を検索する場合は、フィルターを適用して検索を絞り込みます。 トピック、タスク名、承認ステータスでフィルタリングします。

![](assets/response-library-12.png)
