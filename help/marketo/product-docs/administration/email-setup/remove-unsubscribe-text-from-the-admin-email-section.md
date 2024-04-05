---
unique-page-id: 2360245
description: 「管理者メール」セクションから登録解除テキストの削除 - Marketo ドキュメント - 製品ドキュメント
title: 「管理者メール」セクションから登録解除テキストの削除
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
feature: Email Setup
source-git-commit: d635fbd4807890266429d4a257cf7d6588736bb5
workflow-type: ht
source-wordcount: '165'
ht-degree: 100%

---

# 「管理者／メール」セクションから登録解除テキストの削除 {#remove-unsubscribe-text-from-the-admin-email-section}

**[!UICONTROL 管理者]**／**[!UICONTROL メール]**&#x200B;領域から登録解除コンテンツを完全に削除する必要がある唯一の理由は、メールテンプレート自体に登録解除リンクを作成する場合です。テキストボックスには、コンテンツなしで保存できない検証機能があります。この問題を回避するには、小さな HTML コメントを追加します。HTML コメントは、メールクライアントに表示されません。メールが HTML でレンダリングされ、コメントは省略されるからです。その方法を説明しましょう。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. 「**[!UICONTROL メール]**」をクリックします。

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. すべてのテキストを選択し、「**[!UICONTROL 削除]**」キーを押します。

   >[!CAUTION]
   >
   >削除する前に、バックアップとしてこれをテキストドキュメントにコピー＆ペーストします。

1. `<!--This is a comment -->` と入力します。

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. 「**[!UICONTROL 変更を保存]**」をクリックします。

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>**登録解除テキスト**&#x200B;向けに 1 文字追加する必要があります。ダッシュまたはピリオドを使用します。
