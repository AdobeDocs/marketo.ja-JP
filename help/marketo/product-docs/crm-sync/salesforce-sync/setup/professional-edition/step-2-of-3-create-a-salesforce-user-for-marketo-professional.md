---
unique-page-id: 3571797
description: 手順 2／3 - Marketo 用の Salesforce ユーザーの作成（Professional）- Marketo ドキュメント - 製品ドキュメント
title: 手順 2／3 - Marketo 用の Salesforce ユーザーの作成（Professional）
exl-id: 7eb4bf89-b6e4-45e0-adee-e2976cb01dd3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '423'
ht-degree: 100%

---

# 手順 2 / 3：Marketo 用の Salesforce ユーザーの作成（Professional） {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>これらの手順は、Salesforce 管理者が実行する必要があります

>[!PREREQUISITES]
>
>[手順 1／3：Marketo フィールドの Salesforce への追加（Professional）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)

この記事では、Salesforce ページレイアウトを使用してフィールド権限をカスタマイズし、Marketo-Salesforce 同期ユーザーを作成します。

## ページレイアウトの設定 {#set-page-layouts}

Salesforce Professional は、Salesforce Enterprise／Unlimited のプロファイルとは異なり、ページレイアウトでフィールドレベルのアクセシビリティを設定します。これらの手順に従うと、Marketo 同期ユーザーはカスタムフィールドをアップデートできます。

1. ナビゲーション検索バーで「**ページレイアウト**」と入力します。**Enter** を押さず、**リード**&#x200B;の下にある「**ページレイアウト**」をクリックします。

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. ページレイアウトの横にある「**編集**」をクリックします。

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. 新しい&#x200B;**セクション**&#x200B;をページレイアウトに追加します。

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. 「**セクション名**」に「Marketo」と入力し、「**OK**」をクリックします。

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. **獲得日**&#x200B;フィールドをクリックして **Marketo** セクションにドラッグします。

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. 次のフィールドに対して、上記の手順を繰り返します。

   * 新規顧客獲得プログラム
   * 新規顧客獲得プログラム ID
   * メールオプトアウト
   * 推測される都市
   * 推測される企業
   * 推測される国
   * 推測される都市圏
   * 推測される市外局番
   * 推測される郵便番号
   * 推測される都道府県／地域
   * リードのスコア
   * 訪問者の参照元
   * 参照元検索エンジン
   * 参照元検索フレーズ
   * 参照元のソース情報
   * 参照元のソースのタイプ

   >[!NOTE]
   >
   >Marketo が読み取り／書き込みできるように、これらのフィールドをページレイアウト上に配置する必要があります。

   >[!TIP]
   >
   >ページの右側に下にドラッグして、フィールドの列を 2 つ作成します。列の長さのバランスを取るために、フィールドを片側から他方に移動できます。

1. フィールドの追加が完了したら、「**保存**」をクリックします。

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. Salesforce **連絡先ページのレイアウト**&#x200B;に対して上記の手順をすべて繰り返します。

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. **連絡先ページのレイアウト**&#x200B;での作業が終わったら忘れずに「**保存**」をクリックしてください。

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >**終日イベント**&#x200B;フィールドが&#x200B;**イベントページレイアウト**&#x200B;に追加されていることを確認してください。

## 同期ユーザを作成 {#create-sync-user}

Marketo は、Salesforce にアクセスするための資格情報が必要です。これは、次の手順で作成した専用ユーザーでおこなうのが最適です。

>[!NOTE]
>
>組織に追加の Salesforce ライセンスがない場合は、**システム管理者**&#x200B;プロファイルを持つ既存の&#x200B;**マーケティングユーザー**&#x200B;を使用できます。

1. ナビゲーション検索バーに「ユーザー」と入力し、「**ユーザーを管理**」の下の「**ユーザー**」をクリックします。

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. 「**新規ユーザー**」をクリックします。

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. 必須フィールドに入力し、「**ユーザライセンス：Salesforce**」を選択して、「**プロファイル：システム管理者**」を設定します。「**マーケティングユーザー**」のチェックをオンにして、「**保存**」をクリックします。

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >入力した電子メールアドレスが有効であることを確認します。パスワードをリセットするには、同期ユーザーとしてログインする必要があります。

これで完了です。これで、Marketo が Salesforce に接続するために使用できるアカウントが作成されました。やってみましょう。

>[!MORELIKETHIS]
>
>[手順 3 / 3：Marketo と Salesforce の接続（Professional）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md)
