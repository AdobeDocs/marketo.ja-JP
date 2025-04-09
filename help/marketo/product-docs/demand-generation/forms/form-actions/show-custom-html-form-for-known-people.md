---
unique-page-id: 2359644
description: 既知のリードのカスタム HTML フォームの表示 - Marketo ドキュメント - 製品ドキュメント
title: 既知のリードのカスタム HTML フォームの表示
exl-id: 668216ea-7c2b-4204-81a5-56547c3baf1d
feature: Forms
source-git-commit: 55964499f5d49258539492f952513833af5692b5
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 85%

---

# 既知のリードのカスタム HTML フォームの表示 {#show-custom-html-form-for-known-people}

訪問者が過去にフルネームとメールアドレスを指定していて、フォーム全体を取得したくない場合は、カスタム HTML（ダウンロードボタンのみ）を表示する方法を説明します。

1. 「**マーケティングアクティビティ**」に移動します。

   ![](assets/login-marketing-activities-5.png)

1. **マーケティングアクティビティ**&#x200B;で、フォームを選択して「**フォームを編集**」をクリックします。

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. 「**フォームの設定**」で「**設定**」をクリックします。

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. **認識済み訪問者の場合、次を表示：**&#x200B;を&#x200B;**カスタム HTML** に設定します。

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. ![—](assets/image2014-9-25-14-3a1-3a26.png)をクリックして、認識済み訪問者に示される&#x200B;**カスタム HTML** を編集します。

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. デフォルトのコンテンツがいくつかありますが、自由に変更できます。

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   使用可能なトークン：

   | トークン | 説明 |
   |---|---|
   | `{{lead.FirstName}}` | これにより、ユーザーの名が表示されます。 |
   | `{{lead.LastName}}` | これにより、ユーザーの姓が表示されます。 |
   | `{{form.Button:default=Download}}` | これにより、フォームボタンが表示されます。`=` の後ろの領域をクリックして、ボタンのテキストを変更します。 |
   | `{{form.NotYou:default=Not you?}}` | これにより、ユーザーが他のユーザーである場合にもリンクが表示されます。`=` の後ろの領域をクリックして、リンクテキストを変更します。 |

   >[!CAUTION]
   >
   >上記の 4 つのトークンのみを使用できます。他のトークンは、ここでは機能しません。

1. 「**終了**」をクリックします。

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. 「**承認して閉じる**」をクリックします。

   >[!NOTE]
   >
   >ランディングページでフォームを使用するには、承認が必要です。

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >必ず、フォームの変更によって作成された[ランディングページのドラフトを承認](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md)してください。

   簡単でしたね。同じフォームに戻った場合にユーザーに表示される内容を確認します。

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >フォームのフォローアップページをファイルの URL に設定することで、ボタンのクリックをアセットに誘導できます。
