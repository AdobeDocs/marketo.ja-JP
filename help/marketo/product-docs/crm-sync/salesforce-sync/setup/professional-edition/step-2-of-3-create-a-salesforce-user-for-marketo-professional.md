---
unique-page-id: 3571797
description: 手順 2／3 - Marketo 用の Salesforce ユーザーの作成（Professional）- Marketo ドキュメント - 製品ドキュメント
title: 手順 2／3 - Marketo 用の Salesforce ユーザーの作成（Professional）
exl-id: 7eb4bf89-b6e4-45e0-adee-e2976cb01dd3
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 100%

---

# 手順 2／3：Marketo 用の [!DNL Salesforce] ユーザの作成（Professional） {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>これらの手順は、Salesforce 管理者が実行する必要があります。

>[!PREREQUISITES]
>
>[手順 1／3：Marketo フィールドの Salesforce への追加（Professional）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md){target="_blank"}

この記事では、[!DNL Salesforce] ページレイアウトを使用してフィールド権限をカスタマイズし、Marketo-[!DNL Salesforce] 間の同期ユーザを作成します。

## ページレイアウトの設定 {#set-page-layouts}

[!DNL Salesforce] Professional は、[!DNL Salesforce] Enterprise／Unlimited のプロファイルとは異なり、ページレイアウトでフィールドレベルのアクセシビリティを設定します。これらの手順に従うと、Marketo 同期ユーザはカスタムフィールドをアップデートできます。

1. ナビゲーション検索バーで「[!UICONTROL ページレイアウト]」と入力します。**[!UICONTROL Enter]** を押さず、**[!UICONTROL リード]**&#x200B;の下にある「**[!UICONTROL ページレイアウト]**」をクリックします。

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. ページレイアウトの横にある「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. 新しい&#x200B;**[!UICONTROL セクション]**&#x200B;をページレイアウトに追加します。

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. 「**[!UICONTROL セクション名]**」に「Marketo」と入力し、「**[!UICONTROL OK]**」をクリックします。

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. **[!UICONTROL 獲得日]**&#x200B;フィールドをクリックして **Marketo** セクションにドラッグします。

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. 次のフィールドに対して、上記の手順を繰り返します。

   * [!UICONTROL 新規顧客獲得プログラム]
   * [!UICONTROL 新規顧客獲得プログラム ID]
   * [!UICONTROL メールオプトアウト]
   * [!UICONTROL 推測される市区町村]
   * [!UICONTROL 推測される会社]
   * [!UICONTROL 推測される国]
   * [!UICONTROL 推測される都市圏]
   * [!UICONTROL 推測される市外局番]
   * [!UICONTROL 推測される郵便番号]
   * [!UICONTROL 推測される都道府県／地域]
   * [!UICONTROL リードのスコア]
   * [!UICONTROL オリジナルリファラー]
   * [!UICONTROL 元の検索エンジン]
   * [!UICONTROL 元の検索フレーズ]
   * [!UICONTROL 元のソース情報]
   * [!UICONTROL 元のソースのタイプ]

   >[!NOTE]
   >
   >Marketo が読み取り／書き込みできるように、これらのフィールドをページレイアウト上に配置する必要があります。

   >[!TIP]
   >
   >ページの右側に下にドラッグして、フィールドの列を 2 つ作成します。列の長さのバランスを取るために、フィールドを片側から他方に移動できます。

1. フィールドの追加が完了したら、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. Salesforce **[!UICONTROL 連絡先ページのレイアウト]**&#x200B;に対して上記の手順をすべて繰り返します。

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. **[!UICONTROL 連絡先ページのレイアウト]**&#x200B;での作業が終わったら忘れずに「**[!UICONTROL 保存]**」をクリックしてください。

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >**[!UICONTROL 終日イベント]**&#x200B;フィールドが&#x200B;**[!UICONTROL イベントページレイアウト]**&#x200B;に追加されていることを確認してください。

## 同期ユーザを作成 {#create-sync-user}

Marketo は、[!DNL Salesforce] にアクセスする資格情報が必要です。これは、次の手順で作成した専用ユーザで行うのが最適です。

>[!NOTE]
>
>組織に追加の Salesforce ライセンスがない場合は、システム管理者プロファイルを持つ既存のマーケティングユーザを使用できます。

1. ナビゲーション検索バーに「ユーザー」と入力し、「**[!UICONTROL ユーザーを管理]**」の下の「**[!UICONTROL ユーザー]**」をクリックします。

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. 「**[!UICONTROL 新規ユーザー]**」をクリックします。

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. 必須フィールドに入力し、「**[!UICONTROL ユーザライセンス：Salesforce]**」を選択して、「**[!UICONTROL プロファイル：システム管理者]**」を設定します。「**[!UICONTROL マーケティングユーザー]**」のチェックをオンにして、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >入力した電子メールアドレスが有効であることを確認します。パスワードをリセットするには、同期ユーザとしてログインする必要があります。

これで完了です。Marketo が [!DNL Salesforce] への接続に使用できるアカウントが作成されました。やってみましょう。

>[!MORELIKETHIS]
>
>[手順 3 / 3：Marketo と Salesforce の接続（Professional）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md){target="_blank"}
