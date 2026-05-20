---
unique-page-id: 11382829
description: IT部門がMarketo Outlook プラグインをアンインストールする方法について説明します。 必要に応じて、ユーザーマシンからアドインを削除します。
title: IT による Marketo  [!DNL Outlook]  プラグインのアンインストール
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/p2CjKHycrJRHLpphyn2qsUEKP-dWh2OlTezwrOn9Ljw
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 139
ht-degree: 87%

---

# IT による Marketo [!DNL Outlook] プラグインのアンインストール {#marketo-outlook-plugin-uninstall-by-it}

IT 部門が Marketo [!DNL Outlook] プラグインをリモートでアンインストールする方法を次に示します。

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
>プラグインをリモートでアンインストールすると、ユーザのマシン上の [!DNL Outlook] が強制的に閉じます。

異なるログレベルやユーザインターフェイスレベルを試す場合は、[Microsoft のスイッチの完全なリスト](https://support.microsoft.com/ja-jp/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6)を参照してください。
