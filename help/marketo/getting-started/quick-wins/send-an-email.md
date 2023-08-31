---
unique-page-id: 2359410
description: メールの送信 - Marketo ドキュメント - 製品ドキュメント
title: メールの送信
exl-id: 1f80fc08-3587-41f0-9c51-2feea10dff0d
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 100%

---

# メールの送信 {#send-an-email}

みんなが最初にやりたがる事です。Marketo からメールを送信しましょう。

>[!PREREQUISITES]
>
>[セットアップと人物の追加](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}

## メールプログラムの作成 {#create-an-email-program}

1. **[!UICONTROL マーケティングアクティビティ]**&#x200B;領域に移動します。

   ![](assets/send-an-email-1.png)

1. **[!UICONTROL 学習]**&#x200B;フォルダーを選択します。**[!UICONTROL 新規]**&#x200B;ドロップダウンをクリックして、**[!UICONTROL 新規プログラム]**&#x200B;を選択します。

   ![](assets/send-an-email-2.png)

1. **[!UICONTROL 名前]**&#x200B;を入力し、「**[!UICONTROL プログラムタイプ]**」で「**[!UICONTROL メール]**」を選択します。

   >[!TIP]
   >
   >プログラム名の最後にイニシャルを追加して、一意にします。

   ![](assets/send-an-email-3.png)

1. 「**[!UICONTROL チャネル]**」で「**[!UICONTROL メール送信]**」を選択し、「**[!UICONTROL 作成]**」をクリックします

   ![](assets/send-an-email-4.png)

## オーディエンスの定義 {#define-your-audience}

1. 「[!UICONTROL オーディエンス]」タイルの下にある「**[!UICONTROL スマートリストを編集]**」をクリックします。

   ![](assets/send-an-email-5.png)

1. 「[!UICONTROL メールアドレス]」フィルターを見つけて、キャンバスにドラッグします。

   ![](assets/send-an-email-6.png)

   >[!TIP]
   >
   >**[!UICONTROL 検索]**&#x200B;機能を使用して、より簡単にフィルターを見つけます。

1. 自分のメールアドレスを探して選択します。

   ![](assets/send-an-email-7.png)

   >[!NOTE]
   >
   >メールが自動入力されない場合は、[リードの設定と追加](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}を行っていないことが考えられます。

   >[!NOTE]
   >
   >この例では、自分に対してのみメールを送信するようにしていますが、オーディエンスは必要に応じてカスタマイズできます。

1. メインのプログラムタブに戻り、「**[!UICONTROL 人物]**」の更新アイコンをクリックします。

   ![](assets/send-an-email-8.png)

   人物が 1 と表示されます。あなたのことです。

## メールの作成 {#create-an-email}

1. 「メール」タイルで、「**[!UICONTROL 新規メール]**」をクリックします。

   ![](assets/send-an-email-9.png)

1. 「**[!UICONTROL 名前]**」を入力し、**テンプレート**&#x200B;を選択して「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/send-an-email-10.png)

1. メールエディターウィンドウが開きます。50 文字以下の件名を入力します（推奨）。

   ![](assets/send-an-email-11.png)

   >[!NOTE]
   >
   >ポップアップブロッカーがある場合は、「**[!UICONTROL 下書きの編集]**」をクリックして、メールエディターに入ります。

1. 編集する領域を選択し、右側の歯車アイコンをクリックして、「**[!UICONTROL 編集]**」を選択します（編集可能セクションをダブルクリックして編集することもできます）。

   ![](assets/send-an-email-12.png)

1. 目的のコンテンツを入力し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/send-an-email-13.png)

1. **[!UICONTROL メールアクション]**&#x200B;ドロップダウンをクリックし、**[!UICONTROL 承認して閉じる]**&#x200B;を選択します。

   ![](assets/send-an-email-14.png)

   >[!TIP]
   >
   >ローンチ前にサンプルを自分に送信して、メールがどのように表示されるかを確認するには、上のメニューで「**[!UICONTROL サンプルを送信]**」を選択するか、「**[!UICONTROL メールアクション]**」をクリックして、「[**[!UICONTROL サンプルを送信]**](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md){target="_blank"}」をクリックします。

1. 左側のツリーで「メールプログラム」を選択します。

   ![](assets/send-an-email-15.png)

1. 「[!UICONTROL スケジュール]」タイルで、メールのローンチ日を「**[!UICONTROL 今日]**」に設定します。

   ![](assets/send-an-email-16.png)

   >[!NOTE]
   >
   >詳しくは、[受信者のタイムゾーン](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md){target="_blank"} and [Head Start](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md){target="_blank"}を参照してください。

1. 15 分以上後の時間を選択してください。

   ![](assets/send-an-email-17.png)

   >[!TIP]
   >
   >デフォルトのタイムゾーンが異なりますか？[ここで更新](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md){target="_blank"}方法をご確認ください。

1. 「[!UICONTROL 承認]」タイルで「**[!UICONTROL プログラムを承認]**」をクリックすれば完了です。

   ![](assets/send-an-email-18.png)

スケジュールされた日時のすぐ後にメールが届きます。

## ミッション完了です。 {#mission-complete}

<br>

[◄ セットアップと人物の追加](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)

[ミッション 2：フォームを含むランディングページ ►](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)
