---
unique-page-id: 14352475
description: アクティビティ履歴への Sales Connect イベントフィールドのインストール - Marketo ドキュメント - 製品ドキュメント
title: アクティビティ履歴への Sales Connect イベントフィールドのインストール
exl-id: c1bdb5a6-04f0-4579-84b6-33f4a301128f
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 43%

---

# アクティビティ履歴への Sales Connect イベントフィールドのインストール {#install-sales-connect-event-fields-on-activity-history}

エンタープライズパッケージをにインストールし [!DNL Salesforce] ら、[!UICONTROL Sales Connect] イベントフィールドをアクティビティ履歴セクションにインストールできます。 [!UICONTROL Sales Connect] のイベントフィールドには、ビュー数、クリック数、キャンペーン数などの情報が含まれます。 これにより、[!DNL Salesforce] に直接読み込まれたメールに関する情報を取得できます。

これらの手順を実行する際は、必ず [!DNL Salesforce] 管理者と協力してください。 この例では、**リードページレイアウト**&#x200B;にフィールドをインストールします。また、連絡先、アカウント、商談の各ページのレイアウトにフィールドをインストールすることもできます。メールをアカウントと商談に記録する場合は、連絡先の役割として関連付けられたメールを送信する連絡先が必要になることに注意してください。

1. 「**[!UICONTROL 設定]**」をクリックします。
1. 「**[!UICONTROL カスタマイズ]**」をクリックします。
1. 「**[!UICONTROL リード]**」をクリックします。
1. 「**[!UICONTROL ページレイアウト]**」をクリックします。
1. 変更するページレイアウトの横にある「**[!UICONTROL 編集]**」をクリックします。

   >[!NOTE]
   >
   >[!DNL Sales Connect] はいくつかのページレイアウトをインストールしますが、チームが既にデフォルトで使用している場合は、そこにインストールする必要があります。 使用しない場合は、[!DNL Sales Connect] のページレイアウトを削除できます。

1. 「[!UICONTROL &#x200B; アクティビティ履歴 &#x200B;]」セクションまでスクロールします。
1. レンチをクリックして編集します。
1. [!UICONTROL &#x200B; アクティビティ履歴 &#x200B;] セクションに含める [!UICONTROL Sales Connect] フィールドを選択します。 [!UICONTROL Sales Connect] フィールドが表示されない場合は、間違った [!DNL Salesforce] パッケージがインストールされている可能性があります。
1. 「**[!UICONTROL 追加]**」をクリックして、目的のフィールドを上に移動します。
1. 「**[!UICONTROL OK]**」をクリックします。
1. 「**[!UICONTROL 保存]**」をクリックします。

   ユーザーは、[!DNL Salesforce] でメールに関する貴重な情報や更新を確認できるようになりました。
