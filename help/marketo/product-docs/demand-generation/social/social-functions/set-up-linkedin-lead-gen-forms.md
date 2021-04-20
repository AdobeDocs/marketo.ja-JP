---
unique-page-id: 12976798
description: LinkedInリードジェネレーションFormsの設定 —Marketoドキュメント — 製品ドキュメント
title: LinkedInリードジェネレーションFormsの設定
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# LinkedInリードジェネレーションFormsの設定{#set-up-linkedin-lead-gen-forms}

LinkedInリードジェネレーションFormsを使用して、LinkedInで広告キャンペーンを実施し、Marketoのリードを生み出します。

>[!NOTE]
>
>**必要な管理者権限**

1. Marketo **管理者**&#x200B;に移動します。

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. **LaunchPoint**&#x200B;に移動し、「**新規**」をクリックして、「**新しいサービス**」を選択します。

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. サービスの&#x200B;**表示名**&#x200B;を入力し、ドロップダウンから&#x200B;**LinkedInリードジェネレーション**&#x200B;サービスを選択して、**次へ**&#x200B;をクリックします。

   ![](assets/linkedin-lead-gen.png)

1. Marketoは同じブラウザで[linkedin.com](https://www.linkedin.com)に新しいタブを開きます。 統合に使用するアカウントを使用して、LinkedInにログインします。

   >[!NOTE]
   >
   >LinkedInアカウントは、スポンサーキャンペーンを作成するすべてのLinkedInビジネスアカウントにアクセスする必要があります。

   ![](assets/linkedin-login.png)

1. LinkedInにログインした後、Marketoに戻り、**許可**&#x200B;をクリックします。

   ![](assets/linkedin-lead-gen-authorize.png)

1. プロンプトが表示されたら、「****&#x200B;許可」をクリックして、LinkedInへのMarketoアプリケーションのインストールを受け入れます。

   ![](assets/linkedin-marketo-allow.png)

1. これで認証が完了したことに気づくでしょう。 「**次へ**」をクリックします。

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >サービスの有効期限は、認証後1年で自動的に切れます。 アクセスを取り戻すには、「**再認証**」をクリックします。 ブラウザの設定に応じて、LinkedInのパスワードを再入力する必要がある場合があります。

1. LinkedInリードジェネレーションのリードがMarketoに来る元のアカウントを選択し、**次へ**&#x200B;をクリックします。

   >[!TIP]
   >
   >想定しているビジネスアカウントが表示されない場合は、承認されるユーザーのLinkedInアカウントに、LinkedInのビジネスアカウントに対するリードジェネレーションフォームマネージャ権限があることを確認してください。

   ![](assets/linkedin-pages-to-capture.png)

1. デフォルトのLinkedInとMarketoのフィールドのマッピングを受け入れるには、「**作成**」をクリックします。 デフォルトのフィールドマッピングの変更、フィールドマッピングの削除、新しいフィールドマッピングの追加を行う場合は、以下のモーダルを使用して、フィールド単位でこれを行うことができます。

   >[!CAUTION]
   >
   >Marketoは、2つのLinkedInフィールドを1つのMarketoフィールド&#x200B;**にマッピングするのをサポートしていますが、2つのLinkedInフィールドが同じフォーム上にない場合のみ**&#x200B;にマッピングします。 同じLinkedIn形式の2つのフィールドを1つのMarketoフィールドにマップすると、Marketoのデータベースにユーザーが入力できない場合があります。

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >LinkedInキャンペーンマネージャーの[フォームテンプレート](https://www.linkedin.com/help/lms/answer/79634)に既に保存されているLinkedInフィールドのみが、MarketoフィールドにマップできるLinkedInフィールドとして表示されます。

   ![](assets/linkedin-installed-services.png)

うまくいった！ LinkedInリードジェネレーションフォームを送信する人は、LinkedIn側で成功したキャンペーンを実行する際に、Marketoに流れ込む開始を送信します。

>[!NOTE]
>
>認証できるのは、1つのLinkedInユーザーアカウントのみです。 Marketoにリンクする複数のビジネスアカウントがある場合は、承認するユーザーのLinkedInアカウントに、LinkedInのビジネスアカウントに対するリードジェネレーションフォームマネージャの権限があることを確認してください。

>[!MORELIKETHIS]
>
>[スマートキャンペーンでのLinkedInリードジェネレーションフォームのフィルターとトリガーの使用](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)
