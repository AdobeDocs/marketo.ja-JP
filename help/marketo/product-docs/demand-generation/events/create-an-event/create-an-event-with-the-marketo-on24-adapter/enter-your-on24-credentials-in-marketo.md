---
unique-page-id: 10096671
description: Marketor - Marketto Docs — 製品ドキュメントにON24資格情報を入力します。
title: MarketorにON24資格情報を入力します
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---


# MarketorにON24資格情報を入力します {#enter-your-on-credentials-in-marketo}

ON24イベント統合を開始します。 資格情報を編集または削除する必要が生じた場合は、これらの手順も以下のとおりです。

## 資格情報を入力 {#enter-credentials}

1. Marketorにログインし、「 **管理者**」をクリックします。

   ![](assets/admin.png)

1. 統合で、「 **LaunchPoint**」をクリックします。

   ![](assets/image2015-12-22-13-3a15-3a38.png)

1. 「Installed Services」で、「 **New** 」、「 **New Service**」の順にクリックします。

   ![](assets/image2015-12-22-13-3a18-3a54.png)

1. New Serviceダイアログボックスで、次の情報を入力します。

   * **表示名** — マーケティング担当者で使用する名前を入力します。 資格情報を共有する場合は、自分の名前、またはグループの名前を指定できます。
   * **Service** — ドロップダウンメニュー **から「On24** 」を選択します。

   * **クライアントキー** — サインインに使用するON24クライアントキーを入力します。 クライアントキーは、文字と数字を組み合わせた32桁の文字列です。
   * **クライアントID** — サインインに使用する4桁のON24クライアントIDを入力します。 ON24アカウントマネージャーからクライアントIDとクライアントキーを直接取得できます。

   ![](assets/image2015-12-22-13-3a38-3a52.png)

1. 「 **作成**」をクリックします。

   ![](assets/image2015-12-22-13-3a28-3a55.png)

1. 資格情報は、検証が完了すると、インストール済みのサービスページに追加されます。 エラーが発生した場合は、資格情報を保存できません。

## 資格情報の編集 {#edit-credentials}

パスワードの有効期限が切れた場合や、既存の秘密鍵証明書を変更する必要がある場合は、秘密鍵証明書を編集できます。

1. 「インストール済みのサービス」タブで、編集する秘密鍵証明書を選択し、「 **サービスを編集**」をクリックします。

   ![](assets/six.png)

1. Edit Serviceダイアログボックスで情報を更新し、「 **Save**」をクリックします。

   ![](assets/seven.png)

## サービスの削除 {#delete-a-service}

1. 「インストール済みのサービス」タブで、削除するサービスを選択し、「 **サービスのアクション** 」ドロップダウンをクリックして、「サービス **の削除**」を選択します。

   ![](assets/eight.png)

1. 「 **削除**」をクリックします。

   ![](assets/nine.png)

次の手順は、ON24でウェビナーイベントを [作成することです](create-your-webinar-event-in-on24.md)。

>[!NOTE]
>
>**関連記事**
>
>* [ON24アダプタイベントについて](understanding-marketo-on24-adapter-events.md)

>



