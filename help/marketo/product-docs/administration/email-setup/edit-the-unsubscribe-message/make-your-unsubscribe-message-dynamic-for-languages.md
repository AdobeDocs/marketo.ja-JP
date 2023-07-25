---
unique-page-id: 6848782
description: 登録解除メッセージを言語に対して動的に設定 - Marketo ドキュメント - 製品ドキュメント
title: 登録解除メッセージを言語に対して動的に設定
exl-id: 953a7fd8-b1f2-4f3f-b889-87d1f0471e0d
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 80%

---

# 登録解除メッセージを言語に対して動的に設定 {#make-your-unsubscribe-message-dynamic-for-languages}

デフォルトの登録解除メッセージとリンクは英語です。動的コンテンツを使用して、様々な言語で表示できます。

>[!NOTE]
>
>この記事はベストプラクティスですが、他の方法でも実行できます。

## データを準備する {#prepare-your-data}

1. 「優先言語」という名前の[カスタムフィールドを作成](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)します。（このフィールドを同期する場合は、CRM で設定します）

   >[!TIP]
   >
   >今後、言語の環境設定を取得するために[フォームを作成](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md)するときに、このフィールドを使用します。

## セグメントを作成する {#create-segmentation}

1. **[!UICONTROL データベース]**&#x200B;に移動します。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-1.png)

1. 「**[!UICONTROL 新規]**」ドロップダウンで、「**[!UICONTROL 新規セグメント化]**」をクリックします。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-2.png)

1. セグメントに「**[!UICONTROL 優先言語]**」という名前を付けます。「**[!UICONTROL セグメントを追加]**」をクリックします。言語を入力します。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-3.png)

   >[!NOTE]
   >
   >デフォルトのセグメントは英語になります。

1. すべての言語が表示されるまで、セグメントの追加を続けます。「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-4.png)

1. セグメントを選択します。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-5.png)

1. 「**[!UICONTROL スマートリスト]**」タブに移動します。検索フィールドに&#x200B;**[!UICONTROL 優先言語]**&#x200B;を入力します。フィルターをキャンバスにドラッグ＆ドロップします。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-6.png)

1. 適切な対応言語を設定します。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-7.png)

1. すべての言語で繰り返します。次に、「**[!UICONTROL セグメント化アクション]**」ドロップダウンを選択して、「**[!UICONTROL 承認]**」をクリックします。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-8.png)

## スニペットの作成 {#create-a-snippet}

1. **[!UICONTROL Design Studio]** に移動します。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-9.png)

1. 「**[!UICONTROL 新規]**」ドロップダウンで、「**[!UICONTROL 新規スニペット]**」をクリックします。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-10.png)

1. スニペットに「**登録解除メッセージ**」という名前を付けます。「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-11.png)

1. デフォルトの登録解除メッセージを入力し、ハイライト表示して、ハイパーリンクアイコンをクリックします。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-12.png)

1. 次のトークンをコピー&amp;ペーストします。 `{{system.unsubscribeLink}}` に **[!UICONTROL URL]** フィールドに入力します。 次に「**[!UICONTROL 挿入]**」をクリックします。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-13.png)

1. セグメント化セクションの「**[!UICONTROL セグメント別]**」を選択します。****

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-14.png)

1. 次の **[!UICONTROL セグメント化]** ドロップダウン、次に入力 **[!UICONTROL 優先]** を選択し、 **[!UICONTROL 優先言語]**. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-15.png)

1. ツリーからセグメントを選択します。購読解除をクリックし、リンクアイコンをクリックします。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-16.png)

1. 確認 `{{system.unsubscribeLink}}` が **[!UICONTROL URL]** フィールドに入力します。 を編集します。 **[!UICONTROL テキストを表示]** 選択した言語に一致するように設定します。 「**[!UICONTROL 適用]**」をクリックします。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-17.png)

1. すべてのセグメントに対してこの手順を繰り返します。次に、 **[!UICONTROL デザインスタジオ]**、 **[!UICONTROL スニペットアクション]** ドロップダウンで、 **[!UICONTROL 承認]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-18.png)

これで完了です。もう少しです。

## メールでスニペットを使用する {#use-snippet-in-an-email}

1. メールエディターで、編集可能な要素をクリックします。次に、歯車アイコンをクリックし、「**[!UICONTROL スニペットに置換]**」を選択します。編集可能なスニペット要素を選択する場合は、歯車アイコンをクリックして、「**[!UICONTROL 編集]**」を選択します。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-19.png)

1. ドロップダウンからスニペットを探して選択し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-20.png)

1. テストするには、「**[!UICONTROL 戻る]**」をクリックし...

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-21.png)

1. ...次に「**[!UICONTROL 動的]**」タブをクリックします。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-22.png)

1. 異なる言語をクリックして、スニペットの変更を確認します。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-23.png)

   >[!TIP]
   >
   >もちろん、残りのメールも動的言語用に編集できます。それと同時に、登録解除ページで同じ方法を行います。

## 動的コンテンツを含む登録解除ページのカスタマイズ {#customizing-your-unsubscribe-page-with-dynamic-content}

登録解除ページが優先言語で表示されるようにする場合は、ランディングページと確認ページで動的コンテンツを使用できます。

1. 次に移動： **[!UICONTROL デザインスタジオ]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-24.png)

1. 入力 _配信停止_ を選択し、目的の購読解除ページを選択します。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-25.png)

1. **[!UICONTROL ドラフトの編集]**&#x200B;をクリックします。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-26.png)

1. 「**[!UICONTROL セグメント別]**」を選択します。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-27.png)

1. 次を検索： **[!UICONTROL 優先言語]** セグメント。 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-28.png)

   各ランディングページのコンテンツを編集し、承認し、これで準備完了です。

   >[!NOTE]
   >
   >[動的コンテンツ](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md)と、その他の役立つ情報を参照してください。
