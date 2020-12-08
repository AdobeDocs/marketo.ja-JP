---
unique-page-id: 3571797
description: 手順2/3 - Marketto(Professional)用のSalesforceユーザーの作成 — Marketto Docs — 製品ドキュメント
title: ステップ2/3 - Marketto(Professional)用のSalesforceユーザーの作成
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---


# 手順2/3:Marketor用のSalesforceユーザーの作成(Professional) {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>これらの手順は、Salesforce管理者が実行する必要があります

>[!NOTE]
>
>**前提条件**
>
>* [手順1/3:Salesforce追加に対するマーケティング担当者のフィールド(Professional)](step-1-of-3-add-marketo-fields-to-salesforce-professional.md)

>



この記事では、Salesforceページレイアウトでフィールド権限をカスタマイズし、Marketor-Salesforce同期ユーザーを作成します。

## ページレイアウトの設定 {#set-page-layouts}

Salesforce Professionalは、Salesforce Enterprise/Unlimitedのプロファイルに対して、ページレイアウトを使用したフィールドレベルのアクセシビリティを設定します。 次の手順に従って、マーケティング担当者がカスタムフィールドを同期できるようにします。

1. ナビゲーション検索バーに **Enterキーを押さずに** ページレイアウトを入力し **、「Leads」の下の「** Page Layout ********」をクリックします。

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. 「Lead Layout」の横にある「 **Edit** 」をクリックします。

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. 新しい **セクションをクリックし、ページレイアウトにドラッグします** 。

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. 「 **セクション名** 」に「Marketo」と入力し、「 **OK**」をクリックします。

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. 「 **獲得日付** 」フィールドをクリックし、「 **マーケティング** 」セクションにドラッグします。

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. 次のフィールドに対して、上記の手順を繰り返します。

   * 獲得プログラム
   * 獲得プログラムID
   * 電子メオプトアウトール
   * 推定都市
   * 推定会社
   * 推定国
   * 推定都市圏
   * 推定電話番号市外局番
   * 推定郵便番号
   * 推定状態領域
   * リードスコア
   * 元の転送者
   * オリジナル検索エンジン
   * オリジナルの検索フレーズ
   * 元のソース情報
   * 元のソースの種類

   >[!NOTE]
   >
   >これらのフィールドは、マーケティング担当者が読み取り/書き込みを行えるように、ページレイアウト上に配置する必要があります。

   >[!TIP]
   >
   >ページの右側に下方向にドラッグして、フィールドに2つの列を作成します。 フィールドを左右に移動して、列の長さのバランスをとることができます。

1. フィールドの追加が完了したら、 **「保存** 」をクリックします。

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. Salesforce **連絡先ページのレイアウトについて、上記の手順をすべて繰り返します**。

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. 「 **連絡先ページのレイアウト」の設定が完了したら、必ず「** 保存 **」をクリックしてください**。

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >**Reminder**
   >
   >
   >「 **終日のイベント** 」フィールドが「 **イベントページのレイアウト**」に追加されていることを確認します。

## 同期ユーザーの作成 {#create-sync-user}

Marketorは、Salesforceにアクセスするために資格情報が必要です。 これは、次の手順で作成した専用のユーザーを使用して行うのが最適です。

>[!NOTE]
>
>組織に追加のSalesforceライセンスがない場合は、シス **テム管理者** プロファイルの既存の **マーケティングユーザー** を使用できます。

1. ナビゲーション検索バーに「users」と入力し、「ユーザーを **管理** 」の下にある「 **Users**」をクリックします。

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. 「 **新規ユーザー**」をクリックします。

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. 必要なフィールドに入力し、「 **ユーザライセンス」を選択します。Salesforce**、 **プロファイルの設定：システム管理者**、「 **マーケティングユーザー** 」を選択し、「 **保存**」をクリックします。

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >入力した電子メールアドレスが有効であることを確認します。 パスワードをリセットするには、同期ユーザーとしてログインする必要があります。

素晴らしい！ これで、MarketoがSalesforceに接続する際に使用できるアカウントが作成されました。 やろう。

>[!NOTE]
>
>**関連記事**
>
>* [手順3/3:MarketoとSalesforce(Professional)の連携](step-3-of-3-connect-marketo-and-salesforce-professional.md)

>



