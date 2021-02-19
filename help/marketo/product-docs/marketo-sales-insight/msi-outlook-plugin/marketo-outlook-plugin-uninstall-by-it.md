---
unique-page-id: 11382829
description: Marketo OutlookプラグインのIT部門によるアンインストール — Marketto Docs — 製品ドキュメント
title: IT部門によるMarketo Outlookプラグインのアンインストール
translation-type: tm+mt
source-git-commit: 972cf9769ac751d9abfd5665975703dcd07930f0
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---


# IT部門によるMarketo Outlookプラグインのアンインストール{#marketo-outlook-plugin-uninstall-by-it}

次に、Marketo Outlookプラグインをリモートでアンインストールする方法を示します。

次のコマンドラインを、「System」または/xスイッチを指定した管理ユーザーアカウントで実行してアンインストールします。

`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

トラブルシューティング用に、ログを有効にして出力ログファイルを作成できます。

`<pre>msiexec.exe /x [File Name] /qn /L*v MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v MarketoAddinUninstall.log</pre>`

ログファイルの場所を指定するには、コマンドラインでファイルパスを指定します。

`<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>プラグインをリモートからアンインストールすると、ユーザーのコンピューター上のOutlookが強制的に終了します。

異なるログレベルやユーザーインターフェイスレベルを試す場合は、[Microsoftのスイッチの完全なリスト](https://support.microsoft.com/en-us/kb/227091)を参照してください。
