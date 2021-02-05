---
unique-page-id: 11382815
description: IT部門別Marketto Outlookプラグインのインストール — Marketto Docs — 製品ドキュメント
title: IT部門によるMarketo Outlookプラグインのインストール
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---


# IT部門によるMarketo Outlookプラグインのインストール{#marketo-outlook-plugin-installation-by-it}

企業のポリシーによっては、ITチームが従業員のコンピュータにすべてのソフトウェアをインストールする必要がある場合があります。 このような場合、IT部門は、多くの場合、独自の導入ソフトウェアを使用してリモートでこれを実行します。 このドキュメントは、Outlookプラグインをリモートでインストールする展開プロセスで入力として使用するコマンドラインを提供します。

>[!PREREQUISITES]
>
>[エンタープライズキー](http://docs.marketo.com/display/DOCS/Install+the+Marketo+Add-in+for+Outlook+with+an+Enterprise+Key) を設定します。

次のコマンドラインを、「システム」または/iスイッチを指定した管理ユーザーアカウントで実行してインストールします。 `<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**例**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

トラブルシューティングのために、ログを有効にして出力ログファイルを作成できます。 `<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**例**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

ログファイルの場所を指定するには、コマンドラインでファイルパスを指定します。 `<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**例**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>ログファイルのストレージの場所が存在する必要があります。存在しない場合は、インストールが中止されます。

異なるログレベルやユーザーインターフェイスレベルを試す場合は、[Microsoftのスイッチの完全なリスト](https://support.microsoft.com/en-us/kb/227091)を参照してください。

>[!MORELIKETHIS]
>
>[IT部門によるMarketo Outlookプラグインのアンインストール](marketo-outlook-plugin-uninstall-by-it.md)

