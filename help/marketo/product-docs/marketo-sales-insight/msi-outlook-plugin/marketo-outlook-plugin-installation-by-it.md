---
unique-page-id: 11382815
description: IT によるMarketo [!DNL Outlook]  プラグインのインストール - Marketo ドキュメント – 製品ドキュメント
title: IT によるMarketo [!DNL Outlook]  プラグインのインストール
exl-id: c1ae1fb8-d1ad-4c1b-899b-29629fcb166b
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 85%

---

# IT によるMarketo [!DNL Outlook] プラグインのインストール {#marketo-outlook-plugin-installation-by-it}

企業のポリシーにより、IT チームが従業員のコンピューターにすべてのソフトウェアをインストールすることが要求される場合があります。このような場合、IT 部門はしばしば独自の導入ソフトウェアを使用してリモートでこれを実行します。このドキュメントでは、Outlook プラグインをリモートでインストールするためのデプロイメントプロセスで入力として使用するコマンドラインを提供します。

>[!PREREQUISITES]
>
>エンタープライズキーを[設定](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md)します。

次のコマンドを、「System」または管理ユーザアカウントとして実行し、/i スイッチを指定してインストールします。

`<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**例**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

トラブルシューティングのためには、ログを有効にして出力ログファイルを作成できます。

`<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**例**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

ログファイルの場所を指定するには、コマンドラインでファイルパスを指定します。

`<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**例**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>ログファイルの保存場所が存在する必要があります。存在しない場合、インストールは中止されます。

異なるログレベルやユーザインターフェイスレベルを試す場合は、[Microsoft のスイッチの完全なリスト](https://support.microsoft.com/ja-jp/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6)を参照してください。

>[!MORELIKETHIS]
>
>[IT によるMarketo [!DNL Outlook]  プラグインのアンインストール ](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
