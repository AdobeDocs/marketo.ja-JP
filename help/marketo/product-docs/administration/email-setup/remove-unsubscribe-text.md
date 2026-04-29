---
unique-page-id: 2360245
description: テンプレートにリンクを作成する際に、HTML コメントを使用して、管理者メールからデフォルトの購読解除コンテンツを削除します。
title: 登録解除テキストの削除
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
feature: Email Setup
source-git-commit: 9c4f0d0a43d3ef06132d827b605b9e42de712e22
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 68%

---

# 登録解除テキストの削除 {#remove-unsubscribe-text}

購読解除コンテンツを&#x200B;**[!UICONTROL 管理者]** > **[!UICONTROL 電子メール]**&#x200B;領域から完全に削除する必要がある唯一の理由は、購読解除リンクを電子メールテンプレート自体に構築することを選択している場合です。 テキストボックスには、コンテンツなしで保存できない検証機能があります。 この問題を回避するには、小さな HTML コメントを追加します。 HTML コメントは、メールクライアントに表示されません。メールが HTML でレンダリングされ、コメントは省略されるからです。

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
>**登録解除テキスト**&#x200B;向けに 1 文字追加する必要があります。 ダッシュまたはピリオドを使用します。
