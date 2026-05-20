---
unique-page-id: 11382815
description: IT部門が組織用のMarketo Outlook プラグインをインストールする方法について説明します。 Outlook ユーザー向けにアドインを大規模に展開します。
title: IT による Marketo  [!DNL Outlook]  プラグインのインストール
exl-id: c1ae1fb8-d1ad-4c1b-899b-29629fcb166b
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/7Gq4FJlVf9jvqL2Bz34oQVL8HtBNYCjEHl32g-0RXYk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 196
ht-degree: 89%

---

# IT による Marketo [!DNL Outlook] プラグインのインストール {#marketo-outlook-plugin-installation-by-it}

企業のポリシーにより、IT チームが従業員のコンピューターにすべてのソフトウェアをインストールすることが要求される場合があります。 このような場合、IT 部門はしばしば独自の導入ソフトウェアを使用してリモートでこれを実行します。 このドキュメントでは、Outlook プラグインをリモートでインストールするためのデプロイメントプロセスで入力として使用するコマンドラインを提供します。

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
>[IT による Marketo  [!DNL Outlook]  プラグインのアンインストール](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
