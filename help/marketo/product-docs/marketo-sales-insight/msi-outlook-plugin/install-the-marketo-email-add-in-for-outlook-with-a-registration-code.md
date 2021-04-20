---
unique-page-id: 2949711
description: Outlook用Marketo電子メールイ追加ンを登録コード —Marketoドキュメント — 製品ドキュメントと共にインストールする
title: 登録コードを使用したOutlook用Marketo電子メールイン追加のインストール
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 6%

---

# 登録コード{#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}を使用してOutlook用Marketo電子メールイ追加ンをインストールする

ユーザーがラップトップの管理設定にアクセスできる場合は、ユーザーに登録コードを直接送信できます。

招待メールを受け取っていない場合は、Marketoの管理者に招待を依頼してください。

>[!PREREQUISITES]
>
>[Marketo電子メールインライセンス](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/issue-a-marketo-email-add-in-license.md)を発行する必要があり追加ます。

>[!NOTE]
>
>2010年10月1日現在、Outlookプラグインの最新バージョンでは、オフラインモードがサポートされなくなりました。 これは、10/1以降にインストール/アップグレードした後に有効になります。

## インストーラーのダウンロード{#download-installer}

1. [Microsoft Outlookのバージョン](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c)を特定する

1. リンクをクリックして、お使いのバージョンのMicrosoft Outlookに適したインストーラをダウンロードします。

   >[!NOTE]
   >
   >現時点では、以下のリンクはMicrosoft Edgeでのみ機能します。または、Chromeで右クリックしても機能します。 ご不便をおかけして申し訳ございません。

   | Outlookバージョン | 32ビットOutlook | 64ビットOutlook |
   |---|---|---|
   | Outlook 2000 | 非対応 | 該当なし |
   | Outlook 2003 | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | 該当なし |
   | Outlook 2007 | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | 該当なし |
   | Outlook 2010 | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2013 | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2016 | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2019 | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook for Mac | 非対応 | 非対応 |
   | Outlook Web App | 非対応 | 非対応 |
   | Office 365* | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [ダウンロード](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |

   *Office 365バージョン：Windowsクライアントのみ（Windows 10、EnterpriseまたはProの場合）。

## 登録コードをコピー{#copy-your-registration-code}

1. 受け取った招待用電子メールから登録コードをコピーします。

   ![](assets/image2016-7-22-10-3a45-3a10.png)

1. Microsoft Outlookを閉じます。

   ![](assets/ent-key-close-outlook-hand.png)

## インストール {#install}

1. インストーラーを実行します。

   ![](assets/image2016-7-25-10-3a23-3a33.png)

   >[!NOTE]
   >
   >警告が出たら心配するな！ [****&#x200B;を実行]をクリックします。

1. 「**次へ**」をクリックします。

   ![](assets/welcome-to-the-setup-wizard-hand.png)

1. **姓**、**姓**、**電子メールアドレス**&#x200B;を入力し、電子メールから&#x200B;**登録コード**&#x200B;をコピーしてフォームに貼り付け、**次へ**&#x200B;をクリックします。

   ![](assets/enter-your-information-hands.png)

   >[!TIP]
   >
   >インストールに失敗した場合は、IT部門に問い合わせて、HTTPSトラフィックがブロックされていないことを確認してください。 インストーラーでHTTPSトラフィックが開いている必要があります。

1. 「**次へ**」をクリックして、デフォルトの場所にインストールします。

   ![](assets/select-installation-folder-hand.png)

1. 「**次へ**」をクリックします。

   ![](assets/confirm-installation-hand.png)

   >[!NOTE]
   >
   >不明なパブリッシャに関するセキュリティプロンプトが表示された場合は、[**はい**]をクリックします。

1. インストールが完了したら、「**閉じる**」をクリックします。

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. Microsoft Outlookを開き、[Marketo]ボタンを確認します。

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   素晴らしい！ Marketoのボタンの方がいい場所です。

「Marketoメッセージ」および「Marketoとログ」アクションの使用についての詳細。

>[!MORELIKETHIS]
>
>* [Outlook用のMarketo電子メールインを使用した電子メールの送信追加と追跡](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md)
>* [Marketoテンプレートを使用したOutlookからの送信と追跡](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md)

