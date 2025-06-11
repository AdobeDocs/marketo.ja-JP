---
unique-page-id: 2949711
description: 登録コードを使用した Outlook 用 Marketo メールアドインのインストール - Marketo ドキュメント - 製品ドキュメント
title: 登録コードを使用した Outlook 用 Marketo メールアドインのインストール
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
feature: Marketo Sales Insights
source-git-commit: ac6c84a82b9bcb535d5f50897d1a068a5a746287
workflow-type: ht
source-wordcount: '551'
ht-degree: 100%

---

# 登録コードを使用した Outlook 用 Marketo メールアドインのインストール {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

ユーザーがノートパソコンの管理者設定にアクセスできる場合は、登録コードを直接送信できます。

招待メールを受け取っていない場合は、Marketo 管理者に招待するよう依頼してください。

>[!PREREQUISITES]
>
>[Marketo メールアドインライセンスが発行されている](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/issue-a-marketo-email-add-in-license.md)必要があります。

>[!IMPORTANT]
>
>Windows ユーザーフォルダーに英語以外の文字が含まれている PC へのインストールはサポートされていません。このフォルダーは、Windows ユーザー名をもとに Windows が`<System Root>\Users\`に自動生成するもので、Windows ユーザー名が英語以外の名前の場合、英語以外の文字が含まれることがあります。インストールに関する問題が発生しているかどうかを IT チームに問い合わせて確認してください。

>[!NOTE]
>
>Sales Insight Actions 機能（セールスメールを送信、セールスキャンペーンに追加、タスクなど）は、Gmail および Outlook 用の Sales Insight メールプラグインでは使用できません。現時点では、ユーザーは、Sales Insight メールプラグインを使用している場合に、Marketo メールテンプレートを使用した／していないトラッキング可能なメールをお使いのメールクライアントから送信する機能のみ使用できます。

## インストーラーのダウンロード {#download-installer}

1. [Microsoft Outlook のバージョン](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c){target="_blank"}を特定します。

1. 以下の表で、リンクをクリックして、お使いの Microsoft Outlook のバージョンに適した .ZIP ファイルをダウンロードします。

1. ファイルを解凍して必要な .MSI ファイルにアクセスし、インストールを続行します。

   >[!NOTE]
   >
   >現時点では、以下のリンクは、Microsoft Edge または Chrome で右クリックした場合にのみ機能します。ご迷惑をおかけして申し訳ありません。

<table><thead>
  <tr>
    <th>Outlook バージョン</th>
    <th>32 ビット Outlook</th>
    <th>64 ビット Outlook</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Outlook 2000</td>
    <td>サポート対象外</td>
    <td>なし</td>
  </tr>
  <tr>
    <td>Outlook 2003</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">ダウンロード</a></td>
    <td>なし</td>
  </tr>
  <tr>
    <td>Outlook 2007</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">ダウンロード</a></td>
    <td>なし</td>
  </tr>
  <tr>
    <td>Outlook 2010</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">ダウンロード</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">ダウンロード</a></td>
  </tr>
  <tr>
    <td>Outlook 2013</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">ダウンロード</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">ダウンロード</a></td>
  </tr>
  <tr>
    <td>Outlook 2016</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">ダウンロード</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">ダウンロード</a></td>
  </tr>
  <tr>
    <td>Outlook 2019</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">ダウンロード</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">ダウンロード</a></td>
  </tr>
  <tr>
    <td>Outlook for Mac</td>
    <td>サポート対象外</td>
    <td>サポート対象外</td>
  </tr>
  <tr>
    <td>Outlook web アプリケーション</td>
    <td>サポート対象外</td>
    <td>サポート対象外</td>
  </tr>
  <tr>
    <td>Office 365*</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">ダウンロード</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">ダウンロード</a></td>
  </tr>
</tbody></table>

*Office 365 バージョン：Windows クライアントのみ（Windows 10、Enterprise または Pro）。

>[!IMPORTANT]
>
>Microsoft は、[Outlook for Windows の新しいバージョン ](https://techcommunity.microsoft.com/t5/outlook-blog/new-outlook-for-windows-now-available/ba-p/3932068){target="_blank"}をリリースしました。この新しいバージョンは、既存の MSI Outlook プラグインをサポートしていません。MSI Outlook プラグインは、Outlook のクラシックバージョンを実行している Windows デスクトップで引き続き機能します。組織向けの新しい Outlook for Windows の詳細については、[こちらをクリック](https://techcommunity.microsoft.com/t5/outlook-blog/the-new-outlook-for-windows-for-organization-admins/ba-p/3929169){target="_blank"}してください。

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
>* [Outlook 用 Marketo メールアドインを使用したメールの送信とトラッキング](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md){target="_blank"}
>* [Marketo テンプレートを使用した Outlook からの送信とトラッキング](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md){target="_blank"}
