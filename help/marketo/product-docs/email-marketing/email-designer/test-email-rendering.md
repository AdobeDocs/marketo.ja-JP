---
solution: Marketo Engage
product: marketo
title: Litmus を使用したメールのレンダリングのテスト
description: Litmusを使用して、クライアント間でメールのレンダリングをテストする方法を説明します。 Litmus アカウントを統合して、様々なメールクライアントでコンテンツをプレビューします。
level: Beginner, Intermediate
feature: Email Designer
exl-id: ccef36af-362a-4ac0-9030-492e9d7f10b5
TQID: https://experienceleague.adobe.com/HDelTp-9vepH8-TeDRN6FyAe-Nik-hfegvHrakdYDT4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 394
ht-degree: 5%

---

# Litmus を使用したメールのレンダリングのテスト {#test-email-rendering-with-litmus}

Marketo Engageの[Litmus](https://www.litmus.com/email-testing) アカウントを活用して、人気のあるメールクライアントでのメールのレンダリングを即座に確認します。

>[!AVAILABILITY]
>
>この機能は、アクティブなLitmus アカウントを持つすべてのMarketo Engage ユーザーが利用できます。

## Litmus Enterprise ユーザー {#litmus-enterprise}

次の手順は、[Litmus エンタープライズ プラン ](https://www.litmus.com/pricing/enterprise){target="_blank"}のユーザー向けです。

1. _メールコンテンツを編集_&#x200B;画面で、「**コンテンツをシミュレート**」ボタンをクリックします。

   ![](assets/test-email-rendering-with-litmus-1.png)

1. テスト受信者を選択し、「**メールをレンダリング**」ボタンをクリックします。

   ![](assets/test-email-rendering-with-litmus-2.png){width="800" zoomable="yes"}

1. まだ使用していない場合は、**Litmus アカウントを接続します**。 既に実行している場合は、手順6に進んでください。

   ![](assets/test-email-rendering-with-litmus-3.png){width="800" zoomable="yes"}

1. Litmusの資格情報を入力し、**ログイン**&#x200B;をクリックします。

   >[!IMPORTANT]
   >
   >Litmus アカウントをMarketo Engageに接続すると、テストメールがLitmusに送信されることに同意したことになります。 送信後、これらのテストメールはAdobeで管理されなくなります。 そのため、Litmusのデータ保持メールポリシーは、それらのメールに含まれる可能性のあるパーソナライゼーションデータを含め、それらのメールに適用されます。

1. **Connect**&#x200B;をクリックして統合を完了します。

   ![](assets/test-email-rendering-with-litmus-4.png)

1. 「**テストを実行**」ボタンをクリックして、メールのプレビューを生成します。

1. デスクトップ、モバイル、web ベースの一般的なメールクライアントで、コンテンツがどのように表示されるかをご確認ください。 プレビューするサムネールをクリックします。

   ![](assets/test-email-rendering-with-litmus-5.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >デフォルトのメールクライアントリストを[ カスタマイズする方法について説明します](https://help.litmus.com/article/227-change-your-default-email-clients-list)。

1. テストが完了したら、左上の後方矢印をクリックして、_コンテンツをシミュレート_&#x200B;画面に戻ります。

   ![](assets/test-email-rendering-with-litmus-6.png)

**オプション手順**：電子メールを変更する場合、**電子メールをレンダリング**&#x200B;をクリックして表示した後、Litmus _電子メールプレビュー_&#x200B;画面の右上にある&#x200B;**再テスト** ボタンもクリックすることを忘れないでください。

![](assets/test-email-rendering-with-litmus-7.png)

## Litmus コアユーザー {#litmus-core}

次の手順は、[Litmus コアプラン ](https://www.litmus.com/pricing/){target="_blank"}のユーザー向けです。

1. Litmus アカウントで、_テスト_&#x200B;画面の「**テストアドレスをコピー**」ボタンをクリックして、テストメールアドレスを取得します。

   ![](assets/test-email-rendering-with-litmus-8.png){width="800" zoomable="yes"}

1. Marketo Engageで、目的の電子メールの&#x200B;_電子メールコンテンツを編集_&#x200B;画面に移動し、「**コンテンツをシミュレート**」ボタンをクリックします。

   ![](assets/test-email-rendering-with-litmus-9.png){width="600" zoomable="yes"}

1. テスト受信者を選択し、**プルーフを送信** ボタンをクリックします。

   ![](assets/test-email-rendering-with-litmus-10.png){width="800" zoomable="yes"}

1. 手順1でコピーしたLitmus電子メールアドレスを入力し、**プルーフを送信**&#x200B;をもう一度クリックします。

   ![](assets/test-email-rendering-with-litmus-11.png)

1. Litmus アカウント内（Litmusからコピーしたメールアドレスに対応するフォルダー内）のメールを確認します。

   ![](assets/test-email-rendering-with-litmus-12.png){width="800" zoomable="yes"}
