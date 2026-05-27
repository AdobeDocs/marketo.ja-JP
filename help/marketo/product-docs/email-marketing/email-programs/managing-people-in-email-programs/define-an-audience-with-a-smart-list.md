---
unique-page-id: 1900595
description: スマートリストを使用してメールプログラムオーディエンスを定義する方法を説明します。 フィルターを使用して、メールプログラムの受信者をターゲティングします。
title: スマートリストを使用してオーディエンスを定義する
exl-id: 72a1e717-271b-46b5-b097-d29658b8f6ff
feature: Email Programs
TQID: https://experienceleague.adobe.com/sGFMl-NIr1URbKsPhRb-ze6h2c1k72W-E28f-8p--sE
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 276
ht-degree: 85%

---

# スマートリストを使用してオーディエンスを定義する {#define-an-audience-with-a-smart-list}

[メールプログラムを作成](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)したら、メールを送信する相手を指定します。 これは、[リードのリストをインポート](/help/marketo/product-docs/email-marketing/email-programs/managing-people-in-email-programs/define-an-audience-by-importing-a-list.md)するか、スマートリストを使用することで実行できます。 スマートリストを使用する方法を次に示します。

>[!PREREQUISITES]
>
>[メールプログラムの作成](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

>[!NOTE]
>
>オーディエンスの定義は、メールプログラムが承認されていない場合にのみ機能します。

1. **[!UICONTROL マーケティングアクティビティ]**&#x200B;に移動します。

   ![](assets/login-marketing-activities.png)

1. メールプログラムを選択し、 「**[!UICONTROL オーディエンス]**」タイルの下にある「**[!UICONTROL スマートリストの編集]**」をクリックします。

   ![](assets/2017-05-22-09-46-37.png)

   >[!TIP]
   >
   >この項目が表示されない場合は、「表示」が「**[!UICONTROL コントロールパネル]**」に設定されていることを確認してください。

1. 使用するフィルターを検索し、キャンバスまでドラッグします。

   ![](assets/dragstate.png)

1. フィルターを定義します。

   ![](assets/image2014-9-12-11-3a1-3a14.png)

1. フィルターの追加と定義が完了したら、メインのプログラムタブに戻ります。 ここで、条件を満たすリードの数を確認します。

   ![](assets/myemailprogram.jpg)

   できましたね。 次に、[既存の電子メールを選択](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)するか、[電子メールを作成](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)して、これらのユーザーに送信します。

>[!NOTE]
>
>**定義**
>
>ブロック番号に気づきましたか。 この数は、条件を満たすリードのうち、以下の理由によりそのメールを送信できないサブセットを表します。
>
>* 配信停止完了
>* マーケティングを中断したリード
>* ブロックリスト掲載
>* メール無効
>* メールが空欄
>
>数字をクリックすると、このメール配信からブロックされているリードの詳細なリストが表示されます。 **注意**：オペレーショナルなメールは、登録解除済みのリードとマーケティングを中断したリードに引き続き送信されます。
>
>このメールを受け取る人物の数を確認するには、「**[!UICONTROL オーディエンス]**」タイルの「![--](assets/image2014-10-23-16-3a32-3a36.png)」ボタンを使用します。

>[!MORELIKETHIS]
>
>* [既存のメールの選択](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [メールプログラム向け新規メールの作成](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)
