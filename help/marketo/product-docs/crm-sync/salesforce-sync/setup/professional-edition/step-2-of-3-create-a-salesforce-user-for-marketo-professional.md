---
unique-page-id: 3571797
description: 手順2/3 -Marketo（プロフェッショナル）向けSalesforceユーザーの作成 —Marketoドキュメント — 製品ドキュメント
title: ステップ2/3 -Marketo（プロフェッショナル）向けのSalesforceユーザーの作成
exl-id: 7eb4bf89-b6e4-45e0-adee-e2976cb01dd3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 9%

---

# 手順2/3:Marketo版Salesforceユーザーの作成（専門） {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>これらの手順は、Salesforce管理者が実行する必要があります

>[!PREREQUISITES]
>
>[手順1/3:Salesforce追加 (Professional)に対するMarketoフィールド](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)

この記事では、Salesforceページレイアウトでフィールド権限をカスタマイズし、MarketoとSalesforceの同期ユーザを作成します。

## ページレイアウトの設定{#set-page-layouts}

Salesforce Professionalは、Salesforce Enterprise/Unlimitedのプロファイルに対して、ページレイアウトを使用したフィールドレベルのアクセシビリティを設定します。 次の手順に従って、Marketo同期ユーザがカスタムフィールドを更新できるようにします。

1. ナビゲーション検索バーに&#x200B;**ページレイアウト**&#x200B;と入力し、**Enter**&#x200B;キーを押さずに入力し、**リード**&#x200B;の下の&#x200B;**ページレイアウト**&#x200B;をクリックします。

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. 「Lead Layout」の横の「**Edit**」をクリックします。

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. 新しい&#x200B;**セクション**&#x200B;をクリックし、ページレイアウトにドラッグします。

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. **セクション名**&#x200B;に&quot;Marketo&quot;と入力し、**OK**&#x200B;をクリックします。

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. フィールド&#x200B;**獲得日**&#x200B;をクリックし、**Marketo**&#x200B;セクションにドラッグします。

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. 次のフィールドに対して、上記の手順を繰り返します。

   * 新規顧客獲得プログラム
   * 獲得プログラムID
   * メールオプトアウト
   * 推測される都市
   * 推測される企業
   * 推測される国
   * 推測される都市圏
   * 推測される市外局番
   * 推測される郵便番号
   * 推測される都道府県/地域
   * リードスコア
   * 訪問者の参照元
   * 参照元検索エンジン
   * 参照元検索フレーズ
   * 参照元のソース情報
   * 参照元のソースのタイプ

   >[!NOTE]
   >
   >これらのフィールドは、Marketoが読み取り/書き込みを行えるように、ページレイアウト上に配置する必要があります。

   >[!TIP]
   >
   >ページの右側に下方向にドラッグして、フィールドに2つの列を作成します。 フィールドを左右に移動して、列の長さのバランスをとることができます。

1. フィールドの追加が終了したら、「**保存**」をクリックします。

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. Salesforce **連絡先ページのレイアウト**&#x200B;に対して、上記の手順をすべて繰り返します。

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. **連絡先ページのレイアウト**&#x200B;を終了したら、「**保存**」をクリックします。

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >**終日のイベント**&#x200B;フィールドが&#x200B;**イベントページレイアウト**&#x200B;に追加されていることを確認します。

## 同期ユーザーの作成{#create-sync-user}

Marketoは、Salesforceにアクセスするために資格情報が必要です。 これは、次の手順で作成した専用のユーザーを使用して行うのが最適です。

>[!NOTE]
>
>組織に追加のSalesforceライセンスがない場合は、既存の&#x200B;**マーケティングユーザー**&#x200B;と&#x200B;**システム管理者**&#x200B;プロファイルを使用できます。

1. ナビゲーション検索バーに「users」と入力し、「**ユーザーを管理**」の下の「**ユーザー**」をクリックします。

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. 「**新しいユーザー**」をクリックします。

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. 必須フィールドに入力し、**ユーザーライセンスを選択します。Salesforce**、**プロファイルを設定します。システム管理者**、「**マーケティングユーザー**」をオンにし、「**保存**」をクリックします。

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >入力した電子メールアドレスが有効であることを確認します。 パスワードをリセットするには、同期ユーザーとしてログインする必要があります。

素晴らしい！ これで、MarketoがSalesforceに接続する際に使用できるアカウントが作成されました。 やろう。

>[!MORELIKETHIS]
>
>[手順3/3:MarketoとSalesforce(Professional)の接続](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md)
