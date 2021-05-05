---
description: スパムフォームの送信をブロックする方法 —Marketoドキュメント — 製品ドキュメント
title: スパムフォームの送信をブロックする方法
translation-type: tm+mt
source-git-commit: 35ab8d353a2518a1603cb508a6f8c0ea650483e4
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# スパムフォームの送信をブロックする方法{#how-to-block-spam-form-submissions}

多くの場合、チェックサムが無効であるか、チェックサムが見つからないフォーム送信（通常はボットから）は、誤った統計を生成できます。 それを防ぐ方法を次に示します。

>[!CAUTION]
>
>この機能は、プログラム的なPOSTを使用して行われたフォーム送信をleadCapture/save2エンドポイントに拒否します。 ビジネスで、フォームをその方法でMarketoに送信する統合を利用している場合、この機能を有効にすると、それらの送信がブロックされます。 leadCapture/save2をAPIとして使用したり、プログラムによるフォーム送信を直接実行したりすることは、サポートされていません。 次を使用して、ビジネスでフォームのみが送信されるようにしてください。フォームアセット、埋め込みフォームコード、Forms2.js API、または送信フォームREST API。

1. 「**管理者**」をクリックします。

   ![](assets/how-to-block-spam-form-submissions-1.png)

1. **宝箱**&#x200B;をクリックします。

   ![](assets/how-to-block-spam-form-submissions-2.png)

1. 「**人物キャプチャ — 無効なチェックサム値を拒否**」の横にある「**編集**」をクリックします。

   ![](assets/how-to-block-spam-form-submissions-3.png)

1. 「**有効**」チェックボックスを選択し、「**保存**」をクリックします。

   ![](assets/how-to-block-spam-form-submissions-4.png)

>[!NOTE]
>
>この機能を有効にすると、誤った数値が除外されるので、フォームのアクティビティが低下する場合があります。
