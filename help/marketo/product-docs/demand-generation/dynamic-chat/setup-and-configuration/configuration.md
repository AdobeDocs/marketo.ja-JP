---
description: Dynamic Chat ダイアログウィンドウのルックアンドフィールをカスタマイズする方法について説明します。 色、フォント、配置、アバター、通知のサウンドを設定します。
title: 設定
feature: Dynamic Chat
exl-id: 01ca6a38-4918-46b0-b0f6-1baffbb0bbaf
TQID: https://experienceleague.adobe.com/RYL35cMTXpq9dpJp0S-1YhUL29J2sPALRP1Rz3V60vU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 414
ht-degree: 78%

---

# 設定 {#configuration}

チャットボットダイアログウィンドウのルックアンドフィールをカスタマイズする方法を説明します。

開始するには、「**設定**」の下の「**チャットボット**」をクリックします。

![](assets/configuration-1.png)

カスタマイズオプションは複数あります。

![](assets/configuration-2.png)

## 「スタイル」タブ {#style-tab}

### スタイル {#style}

ここでは、ボットウィジェットの色、フォント、配置、チャットボットの名前とアバターなど、ダイアログが表示されるチャットボットのルックアンドフィールを定義します。

各カテゴリのカラーは、[16 進数のカラー値](https://color.adobe.com/create/color-wheel){target="_blank"}（例：白 = #ffffff、赤 = #bf1932 など）で特定されます。

![](assets/configuration-3.png)

「アンカー」を使用すると、サイト訪問者はチャットボックスを開いたり閉じたりできます。 アイコンを右下に表示するか左下に表示するかを選択できます。 パディング（アイコンと web ページの下部の間のスペースの量）を増減させることもできます。

![](assets/configuration-4.png)

### ボット設定 {#agent-settings}

ボット設定で、チャットボックスの上部に表示されるラベルを追加できます（例：「Adobe Assistant」）。 また、応答遅延（秒）を決定し、チャットアバターを変更することもできます。 独自のアバター画像をアップロードするには、「**+**」ボタンをクリックします。

![](assets/configuration-5.png)

>[!NOTE]
>
>カスタムアバターは、256 kb 未満の正方形の画像で、200x200 px 未満である必要があります。 サポートされているファイルタイプは、.jpg、.png、.gif、.webp、.svg などです。

**新着メッセージ通知音**

ドロップダウンをクリックして、セッションでチャットボットがトリガーされるたびに訪問者に通知するサウンドを選択します。 選択できるサウンドは複数あります。

**モバイルでポークメッセージを有効にする**

訪問者がモバイルデバイスからチャットインする場合、訪問者がチャットアイコンの横に開いている質問をクリックせずに表示する「ポーク」を有効にするには、スライダーを選択します。

![](assets/configuration-6.png)

>[!NOTE]
>
>ポークは会話の最初の[カード](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-cards){target="_blank"}でのみ利用できます。

変更が完了したら、**保存**&#x200B;をクリックすることを忘れないでください。

![](assets/configuration-7.png)

## 「プライバシー」タブ {#privacy-tab}

「**プライバシー**」タブをクリックし、サイトのプライバシーポリシーの URL を追加または編集します（オプション）。

![](assets/configuration-8.png)

## 「インストール」タブ {#installation-tab}

Web サイトにチャットボットを表示するには、まず Dynamic Chat JavaScript スニペットをインストールする必要があります。 必要なコードを検索またはコピーするには、このタブをクリックしてください。 この操作に詳しくない場合は、web チームまたはIT部門にお問い合わせください。

![](assets/configuration-9.png)

>[!TIP]
>
>サイトでコンテンツセキュリティポリシー（CSP）を使用している場合に追加すべきコードを以下に示します。

>[!NOTE]
>
>Marketo サポートは、HTML のトラブルシューティングについては対応できません。 HTMLのサポートについては、web デベロッパーにお問い合わせください。
