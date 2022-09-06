---
unique-page-id: 10099077
description: メール到達率パワーパック：シードリストのインポート方法 — Marketo ドキュメント — 製品ドキュメント
title: メール到達率パワーパック：シードリストのインポート方法
exl-id: a4782611-2556-43bf-802b-afeb332eafcd
source-git-commit: 4448d6e082c0c4fad35fc2980446175bffe47e4b
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 95%

---

# メール到達率パワーパック：シードリストのインポート方法 {#email-deliverability-power-pack-how-to-import-a-seedlist}

シードリストは、Google Apps、Hotmail、Yahoo!など、複数のメールボックスプロバイダーに存在するメールアカウントのリストで、受信ボックスの到達率質とスパムフォルダーの到達率の比率を概算するために使用されます。このリストを Marketo インスタンスに取り込む方法を次に示します。

>[!AVAILABILITY]
>
>すべてのお客様がこの機能を購入しているわけではありません。詳細は、セールス担当者にお問い合わせください。

## シードリストのインポート {#import-a-seedlist}

1. マイMarketoで、 **配信ツール**.

   ![](assets/email-deliverability-power-pack-1.png)

1. 「**インボックス情報**」をクリックします。

   ![](assets/two-1.png)

1. 「**シードリストを取得**」をクリックします。

   ![](assets/three-1.png)

1. 「**リストをエクスポート**」をクリックします。

   ![](assets/four.png)

   >[!NOTE]
   >
   >250ok で[リストを最適化](https://help.returnpath.com/hc/en-us/articles/360046746451-What-is-250ok-s-seedlist-optimizer-and-why-should-I-use-it-)する場合は、「**リストを最適化**」を選択します。含めるシードリスト領域を選択する場合、「**リストをカスタマイズ**」を選択します。

1. エクスポート後、リストは txt ファイルとしてブラウザーのダウンロードフォルダーに表示されます。取得し、静的リストとして Marketo インスタンスに[インポート](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)します。

   ![](assets/five.png)

   >[!TIP]
   >
   >リストには見つけやすいような名前を付けてください。

   >[!CAUTION]
   >
   >これらのインボックス情報キャンペーンの数は 1 か月あたりで制限されています。250ok の&#x200B;**アカウント設定**&#x200B;を見て、その数を確認してください。詳細については、Marketo の営業担当にお問い合わせください。

## 新しいシードリストの取得 {#acquiring-new-seedlists}

シードリストは、毎月同じ頻度で変更される場合があります。メール到達率パワーパックに定期的にログインし、シードリストのステータスを確認することが重要です。新しいアドレスが追加されたり、自分側でアップデートが必要になったりした場合は、シードリストを取得ページのインターフェイスを通じてアラートが表示されます。

Marketo で静的リストを作成したら、そのリストへの送信を開始して、メールのインボックスへの配置をテストできます。
