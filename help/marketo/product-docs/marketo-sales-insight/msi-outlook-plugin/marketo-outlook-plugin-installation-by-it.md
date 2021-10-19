---
unique-page-id: 11382815
description: IT による Marketo Outlook プラグインのインストール - Marketo ドキュメント - 製品ドキュメント
title: IT による Marketo Outlook プラグインのインストール
exl-id: c1ae1fb8-d1ad-4c1b-899b-29629fcb166b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '175'
ht-degree: 100%

---

# IT による Marketo Outlook プラグインのインストール {#marketo-outlook-plugin-installation-by-it}

企業のポリシーにより、IT チームが従業員のコンピューターにすべてのソフトウェアをインストールすることが要求される場合があります。このような場合、IT 部門はしばしば独自の導入ソフトウェアを使用してリモートでこれを実行します。このドキュメントでは、Outlook プラグインをリモートでインストールするためのデプロイメントプロセスで入力として使用するコマンドラインを提供します。

>[!PREREQUISITES]
>
>エンタープライズキーを[設定](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md)します。

次のコマンドを、「System」または管理ユーザーアカウントとして実行し、/i スイッチを指定してインストールします。

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

異なるログレベルやユーザーインターフェイスレベルを試す場合は、[Microsoft のスイッチの完全なリスト](https://support.microsoft.com/en-us/kb/227091)を参照してください。

>[!MORELIKETHIS]
>
>[IT による Marketo Outlook プラグインのアンインストール](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
