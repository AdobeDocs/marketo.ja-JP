---
unique-page-id: 11382829
description: IT部門によるMarketoOutlookプラグインのアンインストール —Marketoドキュメント — 製品ドキュメント
title: IT部門によるMarketoOutlookプラグインのアンインストール
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 2%

---

# IT部門によるMarketoOutlookプラグインのアンインストール{#marketo-outlook-plugin-uninstall-by-it}

次に、IT部門がMarketoOutlookプラグインをリモートでアンインストールする方法を示します。

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
