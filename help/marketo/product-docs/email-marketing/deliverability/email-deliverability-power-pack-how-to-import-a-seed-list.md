---
unique-page-id: 10099077
description: シードリストをMarketo Engageインスタンスに読み込む方法を説明します。
title: E メール配信パワーパック — シードリストのインポート方法
exl-id: a4782611-2556-43bf-802b-afeb332eafcd
feature: Deliverability
source-git-commit: 136707304350be59918716233f5d6e2a6438be4e
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 70%

---

# メール到達率パワーパック：シードリストのインポート方法 {#email-deliverability-power-pack-how-to-import-a-seed-list}

シードリストは、Google Apps、Hotmail、Yahoo! など、複数のメールボックスプロバイダーに存在するメールアカウントのリストで、受信ボックスの到達率質とスパムフォルダーの到達率の比率を概算するために使用されます。次に、そのリストをMarketo Engageインスタンスに取り込む手順を示します。

>[!IMPORTANT]
>
>この記事は、現時点でアクティブなエベレストサブスクリプションを持つユーザー向けです。 Bird（旧称 MessageBird）による受信ボックストラッカーを使用する場合は、チュートリアル [ここにあります](/help/marketo/product-docs/email-marketing/deliverability/inbox-tracker/inbox-tracker-tutorials.md){target="_blank"}.

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

1. 書き出し後、リストは.txt ファイルとしてブラウザーの downloads フォルダーに表示されます。 取得し、静的リストとして Marketo インスタンスに[インポート](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)します。

   ![](assets/email-deliverability-power-pack-5.png)

   >[!TIP]
   >
   >リストには見つけやすいような名前を付けてください。

   >[!CAUTION]
   >
   >これらのインボックスへの配置キャンペーンの数は 1 か月あたりで制限されています。数を確認するには、Everest のアカウント設定／サブスクリプションの下の「サブスクリプション」セクションを参照してください。詳細については、Marketo の営業担当にお問い合わせください。

## 新しいシードリストの取得 {#acquiring-new-seedlists}

シードリストは、毎月同じ頻度で変更される場合があります。メール到達率パワーパックに定期的にログインし、シードリストのステータスを確認することが重要です。新しいアドレスが追加されたり、自分側でアップデートが必要な場合は、アプリケーションの左下にある通知アイコンでアラートが表示されます。

Marketoで静的リストを作成したら、そのリストへの送信を開始して、電子メールのインボックスへの配置をテストできます。
