---
description: セールスメールのメールトラッキングについて詳しく見る。 ビュー、クリック、返信がどのように追跡され、ログに記録されるかを把握します。
title: メールトラッキングの概要
exl-id: 89437d22-d739-45ea-8a2e-046a7de80379
feature: Sales Insight Actions
TQID: 'https://experienceleague.adobe.com/y1dxCUs89NkZe9B7UHrWUUchy8BXlCtvg6OxRmqaKD8'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: 412786a7-b8da-5b9d-8c3f-2539a3faad9f
    internal-label: Sales Insight Actions
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 89%
---
# メールトラッキングの概要 {#email-tracking-overview}

## 返信トラッキングの仕組み&#x200B; {#how-reply-tracking-works}

返信トラッキングは、送信するすべてのメールに含まれるメッセージ ID を調べることでおこなわれます。 すべてのメールには、最適な返信トラッキングに利用できる一意のメッセージ ID が含まれています。

>[!PREREQUISITES]
>
>メールサーバーとの接続：新しい返信が届いた日時を知るには、[!DNL Sales Connect] をインボックスに接続する必要があります。 [!DNL Sales Connect] アカウントを Gmail に接続する必要があります。 Outlook を使用している場合は、Exchange サーバーと統合する必要があります。

[!DNL Sales Connect] が送信メールに対する見込み客の返信をトラックできない場合、返信検出に基づくキャンペーンを停止したり、その返信を Salesforce に記録したりすることはできません。 どのメールアドレスでも返信できるとはどういう意味でしょうか？

つまり、<flynn@flynnsarcade.com>に電子メールを送信し、<kevinf@flynnsarcade.com>で返信した場合、返信を追跡できます。 さらに、<flynn@flynnsarcade.com>とCC <alan@encom.com>に電子メールを送信し、Alanが返信を書き込んだ場合、返信も検出され、キャンペーンが終了します。

## メールの添付ファイルのトラッキング方法 {#how-to-track-your-email-attachments}

[!DNL Sales Connect] では添付ファイル（.doc、.ppt、.pdf）のトラッキングが提供されるので、開封／ダウンロードした日時や、受信者がどのページを閲覧しているかを確認できます。 [Web アプリケーション](https://toutapp.com/login)と Gmail（または Google Apps）の両方で、トラッキング可能な添付ファイル機能を使用できます。

>[!NOTE]
>
>添付ファイルのトラッキングは、チームプラン（g3startup プラン以上）でのみ使用できます。&#x200B;

**初めてのトラッキング可能な添付ファイルの送信方法**

1. メールを作成するかテンプレートを編集し、「**[!UICONTROL コンテンツ]**」ボタンをクリックします。

1. 添付ファイルをアップロードして送信します。 PDF、[!DNL Word] ドキュメント、[!DNL Powerpoint] プレゼンテーションをサポートしています。

1. 「**[!UICONTROL メールに追加]**」を選択します。

1. 「**[!UICONTROL 送信]**」をクリックして、ライブフィードを起動します。 受信者が添付ファイルを開き、ページを閲覧していることが確認できます。

>[!TIP]
>
>添付ファイルをトラッキングしない場合は、「ファイルを添付」をクリックするだけで、その添付ファイルはトラッキングされません。

## 表示トラッキングの仕組み&#x200B; {#how-view-tracking-works}

送信するメールの中に見えない画像を配置することで、メールの開封をトラッキングします。&#x200B;

受信者が送信メールに応答しても、[!DNL Sales Connect] では未開封と表示されている場合、受信者がメールクライアント内の画像を有効にしていない可能性があります（例：メール内の「画像をダウンロードするには、ここをクリック」をクリック）。

メールのトラッキング統計を向上させるためのヒント：&#x200B;

* メールに画像（ロゴなど）を含めると、受信者は、画像を有効化してメッセージを表示するように促されます。
* メール内に、コールトゥアクションとしてリンクを含めてください。

## テストメールが表示済みとされていない {#test-email-not-showed-as-viewed}

別のメールアドレスにメッセージを送信した場合でも、自分に送信したメールがライブフィードに記録されることはありません。 アドビのトラッキングはデバイスベースです。[!DNL Sales Connect] にログインしたコンピュータを使用している限り、そのアクティビティは除外されます。

その理由は、 [!DNL Sales Connect] はスマートであり、アクティブユーザは送信したメールを見るたびに、ライブフィードアクティビティに自分自身の情報を表示されたくはないからです。
