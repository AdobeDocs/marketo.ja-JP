---
solution: Marketo Engage
product: marketo
title: Litmus を使用したメールレンダリングのテスト
description: Marketo Engage ユーザーは、Litmus アカウントを統合して、様々なメールクライアントでのコンテンツのレンダリングをシームレスにテストできます。
level: Beginner, Intermediate
feature: Email Designer
exl-id: ccef36af-362a-4ac0-9030-492e9d7f10b5
source-git-commit: e5bb92d007db05fc6d0ee1319cb989ad60063e48
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 8%

---

# Litmus を使用したメールレンダリングのテスト {#test-email-rendering-with-litmus}

Marketo Engageの [Litmus](https://www.litmus.com/email-testing) アカウントを活用すると、一般的なメールクライアントでのメールのレンダリング方法を即座に確認できます。

>[!AVAILABILITY]
>
>この機能は、有効な [Litmus Enterprise](https://www.litmus.com/enterprise){target="_blank"} アカウントを持つすべてのMarketo Engage ユーザーが使用できます。

## 使用方法 {#how-to-use}

1. _メールコンテンツを編集_ 画面で、「**コンテンツをシミュレート**」ボタンをクリックします。

   ![](assets/test-email-rendering-with-litmus-1.png)

1. テスト受信者を選択し、「**メールをレンダリング**」ボタンをクリックします。

   ![](assets/test-email-rendering-with-litmus-2.png){width="800" zoomable="yes"}

1. まだ接続していない場合は、**Litmus アカウントに接続** します。 既に行っている場合は、手順 6 に進んでください。

   ![](assets/test-email-rendering-with-litmus-3.png){width="800" zoomable="yes"}

1. Litmus 資格情報を入力し、「**ログイン**」をクリックします。

   >[!IMPORTANT]
   >
   >Litmus アカウントをMarketo Engageに接続する際は、テストメールが Litmus に送信されることに同意する必要があります。 送信後は、これらのテストメールはAdobeで管理されなくなります。 そのため、Litmus のデータ保持メールポリシーは、パーソナライゼーションデータを含む、これらのメールに適用されます。

1. 「**接続**」をクリックして統合を完了します。

   ![](assets/test-email-rendering-with-litmus-4.png)

1. 「**テストを実行**」ボタンをクリックして、メールのプレビューを生成します。

1. 一般的なデスクトップ、モバイル、web ベースのメールクライアントでコンテンツがどのように表示されるかを確認します。 プレビューするサムネールの数だけクリックします。

   ![](assets/test-email-rendering-with-litmus-5.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >[ デフォルトのメールクライアントリストをカスタマイズ ](https://help.litmus.com/article/227-change-your-default-email-clients-list) する方法を説明します。

1. テストが完了したら、左上の後矢印をクリックして _コンテンツをシミュレート_ 画面に戻ります。

   ![](assets/test-email-rendering-with-litmus-6.png)

**オプションの手順**：メールに変更を加える場合は、「**メールをレンダリング**」をクリックして表示した後、必ず「Litmus **メールのプレビュー**」画面の右上にある「_再テスト_」ボタンをクリックします。

![](assets/test-email-rendering-with-litmus-7.png)
