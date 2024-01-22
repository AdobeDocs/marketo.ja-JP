---
description: SMS メッセージの作成 — Marketoドキュメント — 製品ドキュメント
title: SMS メッセージの作成
feature: Mobile Marketing
source-git-commit: efaf34e8113fc6364655ff01aa788aa62bdd31af
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 17%

---

# SMS メッセージの作成 {#create-an-sms-message}

SMS メッセージの作成方法を次に示します。

>[!AVAILABILITY]
>
>この機能は、Adobe Marketo Engage アカウントのアドオンとして使用できます。プロビジョニングを適切におこなうには、Adobeで購入する必要があります。 詳しくは、アドビアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

>[!PREREQUISITES]
>
>[Vibes を LaunchPoint サービスとして追加](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md){target="_blank"}

1. 「**[!UICONTROL マーケティングアクティビティ]**」に移動します。

   ![](assets/create-an-sms-message-1.png)

1. 目的のプログラムを右クリックし、「 」を選択します。 **[!UICONTROL 新規ローカルアセット]**.

   ![](assets/create-an-sms-message-2.png)

1. 選択 **SMS メッセージ**.

   ![](assets/create-an-sms-message-3.png)

1. 新しい SMS メッセージの名前と説明（オプション）を入力し、「**作成**」をクリックします。

   ![](assets/create-an-sms-message-4.png)

1. エディターで、青い吹き出しの内側をクリックし、テキストの入力を開始します。

   ![](assets/create-an-sms-message-5.png)

   >[!NOTE]
   >
   >SMS メッセージの文字制限は、標準の ASCII 文字セットを使用した 160 文字です。 160 文字を超える場合、メッセージは合計文字数に基づいて分割されます。

1. メッセージにトークンを追加するには、クイックグリーティングを記入して、 **トークン**.

   ![](assets/create-an-sms-message-6.png)

   >[!NOTE]
   >
   >トークンを追加すると、メッセージの上限を超える場合があります。その後、メッセージが分割され、追加のメッセージが作成されます。

   >[!IMPORTANT]
   >
   >SMS コンプライアンス：すべての送信 SMS メッセージには、ブランド名またはプログラムの説明が含まれている必要があります。 定期的なメッセージプログラムの場合、購読者ごとに少なくとも月に 1 回、ヘルプと停止の手順を提供する必要があります。

1. 目的のを選択します。 **トークン**、オプションの **デフォルト値**&#x200B;をクリックし、 **作成**.

   ![](assets/create-an-sms-message-7.png)

1. リンクを追加するには、メッセージ内で表示する場所を選択し、 **リンク**.

   ![](assets/create-an-sms-message-8.png)

1. リンクタイプを選択します。Marketo ランディングページがデフォルトです。該当するページに移動する場合は、ランディングページドロップダウンをクリックし、目的のページを選択します。 クリック **挿入** 完了したら、

   ![](assets/create-an-sms-message-9.png)

   >[!NOTE]
   >
   >デフォルトでは、2 つのトラッキングリンクが選択されています。 「mkt_tok を含める」だけをオフにしても、リンクの追跡は可能ですが、リダイレクト後は、宛先 URL に mkt_tok クエリー文字列パラメーターは含まれません。 このパラメーターは、Marketoのランディングページと Munchkin で、（オプトアウト時などに）人物のアクティビティを適切に追跡するために使用されます。

1. 代わりに外部 URL を使用する場合は、「 **外部 URL**、URL を入力または貼り付けて、「 **挿入**.

   ![](assets/create-an-sms-message-10.png)

   >[!NOTE]
   >
   >「リンクを追跡」を選択したままにすると、Marketoは追跡のために URL を自動的に変更します。 トラッキングを無効にする場合、URL は変更されずにメッセージに表示されます ( 例： `www.adobe.com`) をクリックします。

   >[!CAUTION]
   >
   >次の操作をお勧めします。 _not_ 通信事業者がメッセージにスパムのフラグを設定する場合があるので、短縮 URL（Bitly など）を使用します。

1. メッセージにリンクが表示されます。

   ![](assets/create-an-sms-message-11.png)

   >[!NOTE]
   >
   >Marketo に、ブランド化されたトラッキングドメインのリンクプレビューが表示されます。mkt_tok リンクチェックボックスをオフにすると、リンクが変更されます。

160 文字を超える文字を挿入した場合、エディターは SMS を複数のセクションに分割します。 メッセージあたり 900 文字の制限が全体として制限されています。 上限を超えると、配信時にメッセージは切り捨てられます。
