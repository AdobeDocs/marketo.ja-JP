---
unique-page-id: 10099077
description: メール到達率パワーパック：シードリストのインポート方法 - Marketo ドキュメント - 製品ドキュメント
title: メール到達率パワーパック：シードリストのインポート方法
exl-id: a4782611-2556-43bf-802b-afeb332eafcd
source-git-commit: 7edaf40bebec891ac106bcbbaba1fd513d1f642c
workflow-type: ht
source-wordcount: '317'
ht-degree: 100%

---

# メール到達率パワーパック：シードリストのインポート方法 {#email-deliverability-power-pack-how-to-import-a-seed-list}

シードリストは、Google Apps、Hotmail、Yahoo! など、複数のメールボックスプロバイダーに存在するメールアカウントのリストで、受信ボックスの到達率質とスパムフォルダーの到達率の比率を概算するために使用されます。このリストを Marketo インスタンスに取り込む方法を次に示します。

>[!AVAILABILITY]
>
>すべてのお客様がこの機能を購入しているわけではありません。詳細は、セールス担当者にお問い合わせください。

## シードリストのインポート {#import-a-seed-list}

1. My Marketo で、「**配信ツール**」を選択します。

   ![](assets/email-deliverability-power-pack-1.png)

1. Everest アプリケーションが開きます。左側のナビゲーションで、「**フライト中**」をクリックし、「**インボックスへの配置**」を選択します。

   ![](assets/email-deliverability-power-pack-2.png)

1. 「**シードリストを管理**」タブをクリックします。

   ![](assets/email-deliverability-power-pack-3.png)

1. 「アクション」ドロップダウンをクリックし、「**1 行につき 1 件ダウンロード**」を選択します。

   ![](assets/email-deliverability-power-pack-4.png)

   >[!NOTE]
   >
   >Everest でリストを最適化する場合は、（ページ上部にある）シードリストオプティマイザーを使用します。

1. エクスポート後、リストは txt ファイルとしてブラウザーのダウンロードフォルダーに表示されます。取得し、静的リストとして Marketo インスタンスに[インポート](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)します。

   ![](assets/email-deliverability-power-pack-5.png)

   >[!TIP]
   >
   >リストには見つけやすいような名前を付けてください。

   >[!CAUTION]
   >
   >これらのインボックスへの配置キャンペーンの数は 1 か月あたりで制限されています。数を確認するには、Everest のアカウント設定／サブスクリプションの下の「サブスクリプション」セクションを参照してください。詳細については、Marketo の営業担当にお問い合わせください。

## 新しいシードリストの取得 {#acquiring-new-seedlists}

シードリストは、毎月同じ頻度で変更される場合があります。メール到達率パワーパックに定期的にログインし、シードリストのステータスを確認することが重要です。新しいアドレスが追加されたり、自分側でアップデートが必要な場合は、アプリケーションの左下にある通知アイコンでアラートが表示されます。

Marketo で静的リストを作成したら、そのリストへの送信を開始して、メールのインボックスへの配置をテストできます。
