---
unique-page-id: 42762794
description: ' [!DNL Salesforce]  Classic での一括アクションの使用 - Marketo ドキュメント - 製品ドキュメント'
title: ' [!DNL Salesforce]  Classic での一括アクションの使用'
exl-id: f676ba65-6bc9-41e5-aa70-0f10bceedab7
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 76%

---

# [!DNL Salesforce] Classic での一括アクションの使用 {#using-bulk-actions-in-salesforce-classic}

キャンペーンへのリードの追加、一括メールの送信、[!DNL Salesforce] から [!DNL Sales Connect] へのリードのプッシュなど、一括アクションの実行方法について説明します。

>[!PREREQUISITES]
>
>[!DNL Sales Connect] パッケージの最新バージョンに更新し、リード／取引先責任者表示に一括アクションボタンをインストールします。[手順については、ここをクリックしてください](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf)。

>[!NOTE]
>
>概要を説明する手順に従う前に、Marketo Sales Connect アカウントにログインしていることを確認してください。

## 一括メール {#bulk-email}

1. [!DNL Salesforce] で、「**[!UICONTROL リード]**」タブ、「**[!UICONTROL 移動]**」ボタンをクリックします。

   ![](assets/one-5.png)

1. 目的のリードを選択し、「**[!UICONTROL MSC でのメール（クラシック）]**」ボタンをクリックします。

   ![](assets/two-5.png)

1. MSC メールがポップアップ表示されます。次の機能が含まれます。

   a. 「[!UICONTROL &#x200B; 宛先 &#x200B;]」フィールドに「[!UICONTROL &#x200B; すべての受信者 &#x200B;]」と表示される – これは、リードリスト表示で選択したリードのリストに対応しています
b.このリストは、「[!UICONTROL &#x200B; 一括作成 &#x200B;]」と呼ばれる左側のパネルに表示されます。ここで受信者を追加/削除できます
c. テンプレートを選択するか、独自のメールを作成できます
d. メールに入力される動的フィールドをプレビューできます
e. メールをすぐに送信することも、後で送信するようにスケジュールすることもできます

   ![](assets/three-4.png)

## キャンペーンに追加 {#add-to-campaign}

1. [!DNL Salesforce] で、「**[!UICONTROL リード]**」タブ、「**[!UICONTROL 移動]**」ボタンをクリックします。

   ![](assets/four-3.png)

1. 目的のリードを選択し、「**[!UICONTROL MSC キャンペーンに追加（クラシック）]**」ボタンをクリックします。

   ![](assets/five-3.png)

1. 「[!UICONTROL キャンペーンにリードを追加]」ポップアップが表示されます。「**[!UICONTROL 次へ]**」をクリックし、通常のキャンペーンフローを実行して、MSC キャンペーンをトリガーします。

   ![](assets/six.png)

## Marketo セールスコネクトにプッシュ {#push-to-marketo-sales-connect}

1. [!DNL Salesforce] で、「**[!UICONTROL リード]**」タブ、「**[!UICONTROL 移動]**」ボタンをクリックします。

   ![](assets/seven-1.png)

1. 目的のリードを選択し、「**[!UICONTROL MSC にプッシュ（クラシック）]**」ボタンをクリックします。

   ![](assets/eight-1.png)

1. 「[!UICONTROL Salesforce ブリッジ]」という新しいタブが開きます。「**[!UICONTROL グループに進む→]**」ボタンをクリックします。

   ![](assets/nine-1.png)

1. MSC アカウントに移動し、日時スタンプを使用して作成されたグループが表示されます。同期が完了すると、通知が届き、[!DNL Salesforce] から同期されたリードがグループに含まれます。

   ![](assets/ten.png)

>[!NOTE]
>
>同じ手順に従って、連絡先リスト表示でバルクアクションを使用することもできます。

>[!MORELIKETHIS]
>
>* [グループメールによるメールの送信](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [「選択して送信」による一括メールの作成](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)
