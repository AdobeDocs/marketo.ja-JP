---
unique-page-id: 10099077
description: E メール配信 Power Pack — シードリストのインポート方法 — Marketoドキュメント — 製品ドキュメント
title: E メール配信パワーパック — シードリストのインポート方法
exl-id: a4782611-2556-43bf-802b-afeb332eafcd
source-git-commit: 6ad418c8f4056b9a2fb31b0ac995692f0c618795
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 5%

---

# メール到達率パワーパック：シードリストのインポート方法 {#email-deliverability-power-pack-how-to-import-a-seedlist}

シードリストは、Google Apps、Hotmail、Yahoo！など、複数のメールボックスプロバイダーに存在する E メールアカウントのリストで、受信ボックスの配信品質とスパムフォルダーの配信品質の比率を概算するために使用されます。 このリストをMarketoインスタンスに取り込む方法を次に示します。

>[!AVAILABILITY]
>
>すべてのお客様がこの機能を購入しているわけではありません。詳細は、営業担当にお問い合わせください。

## シードリストのインポート {#import-a-seedlist}

1. に移動します。 **配信ツール**.

   ![](assets/one-1.png)

1. クリック **インボックス情報**.

   ![](assets/two-1.png)

1. クリック **シードリストの取得**.

   ![](assets/three-1.png)

1. クリック **リストを書き出し**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >選択 **リストを最適化** もし 250ok を [リストの最適化](https://help.returnpath.com/hc/en-us/articles/360046746451-What-is-250ok-s-seedlist-optimizer-and-why-should-I-use-it-) あなたのために。 選択 **リストをカスタマイズ** を選択します。

1. 書き出し後、リストは.txt ファイルとしてブラウザーの downloads フォルダーに表示されます。 取得し、 [インポート](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md) 静的リストとしてMarketoインスタンスに追加します。

   ![](assets/five.png)

   >[!TIP]
   >
   >見つけやすいように、必ずリストに名前を付けてください。

   >[!CAUTION]
   >
   >1 ヶ月あたり、これらの受信ボックス情報キャンペーンの数は制限されています。 250ok を見て、何人手に入ったかを確認してください **アカウント設定**. 詳細については、Marketoの営業担当にお問い合わせください。

## 新しいシードリストの取得 {#acquiring-new-seedlists}

シードリストは、毎月同じ頻度で変更される場合があります。 E メール配信品質 Power Pack に定期的にログインし、シードリストのステータスを確認することが重要です。 新しいアドレスが追加されたり、エンドで更新が必要になったりした場合は、「シードリストの取得」ページのインターフェイスを通じてアラートが表示されます。

Marketoで静的リストを作成したら、そのリストへの送信を開始して、電子メールのインボックスへの配置をテストできます。
