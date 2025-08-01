---
unique-page-id: 11382829
description: Marketo [!DNL Outlook]  プラグインのアンインストール（IT 部門） - Marketo ドキュメント – 製品ドキュメント
title: Marketo [!DNL Outlook]  プラグイン IT によるアンインストール
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 65%

---

# Marketo [!DNL Outlook] プラグイン IT によるアンインストール {#marketo-outlook-plugin-uninstall-by-it}

IT 部門がMarketo [!DNL Outlook] プラグインをリモートでアンインストールする方法を次に示します。

次のコマンドを、「System」または管理ユーザアカウントとして実行し、/i スイッチを指定してアンインストールします。

`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

トラブルシューティングのためにはログを有効にして出力ログファイルを作成できます。

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
>プラグインをリモートでアンインストールすると、ユーザーのコンピューター上の [!DNL Outlook] が強制的に閉じられます。

異なるログレベルやユーザインターフェイスレベルを試す場合は、[Microsoft のスイッチの完全なリスト](https://support.microsoft.com/ja-jp/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6)を参照してください。
