---
description: ON24 とMarketoの統合の設定 — Marketoドキュメント — 製品ドキュメント
title: Marketoとの ON24 統合の設定
exl-id: 395ffa37-b87d-4eb4-bf9f-72aa96dc819c
source-git-commit: e0d656352c83360d5453b91592c50efe4396a4cc
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 11%

---

# Marketoとの ON24 統合の設定{#set-up-the-on24-integration-with-marketo}

ON24 イベント統合の設定方法を以下に示します。

## API 専用のロールの作成 {#Create an API Only Role}

1. My Marketo で、「**管理者**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-1.png)

1. 「セキュリティ」で「**ユーザーと役割**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-2.png)

1. 「**役割**」タブをクリックしてから、「**新規の役割**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-3.png)

1. ロール名を入力します。 を開きます。 **API にアクセス** メニューを開き、「読み取り/書き込みカスタムオブジェクト」と「読み取り/書き込み担当者」を選択します。 「**作成**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-4.png)

## ユーザーを新規作成する {#create-a-new-user}

1. 引き続き「ユーザーとロール」で、 **ユーザー** タブをクリックし、 **新しいユーザーの招待**.

   ![](assets/set-up-the-on24-integration-with-marketo-5.png)

1. 新しいユーザーの情報を入力し、 **次へ**.

   ![](assets/set-up-the-on24-integration-with-marketo-6.png)

1. 先ほど作成した ON24 API のみのロールを選択します。 を選択します。 **API のみ** チェックボックス。 「**次へ**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-7.png)

1. 「**送信**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-8.png)

>[!NOTE]
>
>API のみのユーザーには招待状は必要ありません。

## ON24 接続のセットアップ {#set-up-on24-connection}

1. 引き続き「管理者」セクションで、「 **LaunchPoint**.

   ![](assets/set-up-the-on24-integration-with-marketo-9.png)

1. クリック **新規** その後 **新しいサービス**.

   ![](assets/set-up-the-on24-integration-with-marketo-10.png)

1. 表示名を選択します。 次をクリック： **サービス** ドロップダウンして「 」を選択します。 **カスタム**. 説明を入力します。 「 API のみのユーザー」ドロップダウンをクリックし、作成したユーザーを選択します [上記の手順で](#create-a-new-user). 「**作成**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-11.png)

1. 作成したカスタム LaunchPoint サービスを見つけ、「詳細を表示」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-12.png)

1. クライアント ID をハイライトし、右クリックしてコピーし、保存します（後で必要になります）。 クライアントの秘密鍵に対してこの手順を繰り返します。

   ![](assets/set-up-the-on24-integration-with-marketo-13.png)

1. 左側のツリーで、「Web サービス」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-14.png)

1. 「REST API」で、ハイライト表示し、右クリックし、コピーして、ID の最初の部分を保存します（.com の「m」まで）。

   ![](assets/set-up-the-on24-integration-with-marketo-15.png)

1. 保存したクライアント ID、クライアントの秘密鍵、ID を使用して、ON24 アカウントに移動します。 残りの手順は、ここで実行され、以下が実行されます。 [概要](https://on24support.force.com/Support/s/article/Connect-Marketo-ON24-Connect-Data-Integration#Step6){target=&quot;_blank&quot;}。
