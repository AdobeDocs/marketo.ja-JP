---
unique-page-id: 2949711
description: 登録コードを使用した Outlook 用 Marketo メールアドインのインストール - Marketo ドキュメント - 製品ドキュメント
title: 登録コードを使用した Outlook 用 Marketo メールアドインのインストール
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
source-git-commit: 268a7f1ca441661e1d943a8d6abce7bdcf308a98
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 85%

---

# 登録コードを使用した Outlook 用 Marketo メールアドインのインストール {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

ユーザーがノートパソコンの管理者設定にアクセスできる場合は、登録コードを直接送信できます。

招待メールを受け取っていない場合は、Marketo 管理者に招待するよう依頼してください。

>[!PREREQUISITES]
>
>[Marketo メールアドインライセンスが発行されている](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/issue-a-marketo-email-add-in-license.md)必要があります。

>[!IMPORTANT]
>
>Windows ユーザーフォルダに英語以外の文字が含まれている PC では、インストールはサポートされていません。 このフォルダは、Windows によって `<System Root>\Users\` Windows ユーザー名に基づきます。Windows ユーザー名が英語以外の名前の場合は、英語以外の文字を含めることができます。 インストールに関する問題が発生しているかどうかを IT チームに問い合わせて確認してください。

>[!NOTE]
>
>10/1/20で、Outlook プラグインの最新バージョンがオフラインモードのサポートを停止しました。

## インストーラーのダウンロード {#download-installer}

1. [Microsoft Outlook のバージョン](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c)を特定する

1. リンクをクリックして、お使いのバージョンの Microsoft Outlook に適したインストーラーをダウンロードします。

   >[!NOTE]
   >
   >現時点では、以下のリンクは、Microsoft Edge または Chrome で右クリックした場合にのみ機能します。ご迷惑をおかけして申し訳ありません。

   | Outlook バージョン | 32 ビットOutlook | 64 ビット Outlook |
   |---|---|---|
   | Outlook 2000 | サポート対象外 | なし |
   | Outlook 2003 | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | なし |
   | Outlook 2007 | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | なし |
   | Outlook 2010 | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2013 | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2016 | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2019 | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook for Mac | サポート対象外 | サポート対象外 |
   | Outlook web アプリケーション | サポート対象外 | サポート対象外 |
   | Office 365* | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |

   *Office 365 バージョン：Windows クライアントのみ（Windows 10、Enterprise または Pro）。

## 登録コードをコピーする {#copy-your-registration-code}

1. 受け取った招待メールから登録コードをコピーします。

   ![](assets/image2016-7-22-10-3a45-3a10.png)

1. Microsoft Outlook を閉じます。

   ![](assets/ent-key-close-outlook-hand.png)

## インストール {#install}

1. インストーラーを実行します。

   ![](assets/image2016-7-25-10-3a23-3a33.png)

   >[!NOTE]
   >
   >セキュリティ警告が表示されても、問題はありません。「**実行**」をクリックしてください。

1. 「**次へ**」をクリックします。

   ![](assets/welcome-to-the-setup-wizard-hand.png)

1. **名**、**姓**、**メールアドレス**&#x200B;を入力し、**登録コード**&#x200B;をメールからフォームにコピー＆ペーストして、「**次へ**」をクリックします。

   ![](assets/enter-your-information-hands.png)

   >[!TIP]
   >
   >インストールに失敗した場合は、IT 担当者と相談し、HTTPS トラフィックがブロックされていないことを確認してください。インストーラーを実行するには HTTPS トラフィックが必要です。

1. 「**次へ**」をクリックして、デフォルトの場所にインストールします。

   ![](assets/select-installation-folder-hand.png)

1. 「**次へ**」をクリックします。

   ![](assets/confirm-installation-hand.png)

   >[!NOTE]
   >
   >不明な発行元に関するセキュリティプロンプトが表示された場合は、「**はい**」をクリックします。

1. インストールが完了したら、「**閉じる**」をクリックします。

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. Microsoft Outlook を開くと、「Marketo」ボタンが表示されます。

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   これで完了です。これで、Marketo のボタンの位置が改善されました。

Marketo アクションでのメッセージとログの使用について詳しくは、こちらを参照してください。

>[!MORELIKETHIS]
>
>* [Outlook 用 Marketo メールアドインを使用したメールの送信とトラック](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md)
>* [Marketo テンプレートを使用した Outlook からの送信とトラック](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md)

