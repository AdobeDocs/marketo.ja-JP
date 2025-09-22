---
unique-page-id: 14352475
description: アクティビティ履歴への Sales Connect イベントフィールドのインストール - Marketo ドキュメント - 製品ドキュメント
title: アクティビティ履歴への Sales Connect イベントフィールドのインストール
exl-id: c1bdb5a6-04f0-4579-84b6-33f4a301128f
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 100%

---

# アクティビティ履歴への Sales Connect イベントフィールドのインストール {#install-sales-connect-event-fields-on-activity-history}

[!DNL Salesforce] に Enterprise パッケージをインストールしたら、[!UICONTROL Sales Connect] イベントフィールドをアクティビティ履歴セクションにインストールできます。[!UICONTROL Sales Connect] イベントフィールドには、表示回数、クリック数、キャンペーンなどの情報が含まれます。これにより、メールに関する情報を [!DNL Salesforce] に直接読み込むことができます。

これらの手順を実行する際は、[!DNL Salesforce] 管理者と連携して行ってください。この例では、**リードページレイアウト**&#x200B;にフィールドをインストールします。また、連絡先、アカウント、商談の各ページのレイアウトにフィールドをインストールすることもできます。メールをアカウントと商談に記録する場合は、連絡先の役割として関連付けられたメールを送信する連絡先が必要になることに注意してください。

1. 「**[!UICONTROL 設定]**」をクリックします。
1. 「**[!UICONTROL カスタマイズ]**」をクリックします。
1. 「**[!UICONTROL リード]**」をクリックします。
1. 「**[!UICONTROL ページレイアウト]**」をクリックします。
1. 変更するページレイアウトの横にある「**[!UICONTROL 編集]**」をクリックします。

   >[!NOTE]
   >
   >[!DNL Sales Connect] は、いくつかのページレイアウトをインストールしますが、既に使用しているデフォルトのレイアウトがある場合は、そこにインストールします。使用しない場合は、[!DNL Sales Connect] ページのレイアウトを削除できます。

1. 下にスクロールして、「[!UICONTROL アクティビティの履歴]」セクションを表示します。
1. レンチをクリックして編集します。
1. 「[!UICONTROL アクティビティの履歴]」セクションに含める [!UICONTROL Sales Connect] フィールドを選択します。ここに [!UICONTROL Sales Connect] フィールドが表示されない場合は、誤った [!DNL Salesforce] パッケージがインストールされている可能性があります。
1. 「**[!UICONTROL 追加]**」をクリックして、目的のフィールドを上に移動します。
1. 「**[!UICONTROL OK]**」をクリックします。
1. 「**[!UICONTROL 保存]**」をクリックします。

   [!DNL Salesforce] でメールに関する貴重な情報や更新を確認できるようになりました。
