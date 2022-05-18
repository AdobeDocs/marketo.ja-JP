---
unique-page-id: 12976798
description: LinkedIn リード生成フォームの設定 - Marketo ドキュメント - 製品ドキュメント
title: LinkedIn リード生成フォームの設定
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
source-git-commit: 41d8762203786bac9aea03ac978daa0549ac8e93
workflow-type: ht
source-wordcount: '433'
ht-degree: 100%

---

# LinkedIn リード生成フォームの設定 {#set-up-linkedin-lead-gen-forms}

LinkedIn リード生成フォームを使用して、LinkedIn で広告キャンペーンを実行し、Marketo のリードを生成します。

>[!NOTE]
>
>**管理者権限が必要**

1. 「**管理**」に移動します。

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. 「**LaunchPoint**」に移動します。「**新規**」をクリックして、「**新規サービス**」を選択します。

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. サービスの&#x200B;**表示名**&#x200B;を入力し、ドロップダウンから「**LinkedIn リード生成**」サービスを選択し、「**次へ**」をクリックします。

   ![](assets/linkedin-lead-gen.png)

1. Marketo は同じブラウザーで新しい [linkedin.com](https://www.linkedin.com) タブを開きます。統合に使用するアカウントを使用して LinkedIn にログインします。

   >[!NOTE]
   >
   >LinkedIn アカウントは、スポンサーキャンペーンを作成するすべての LinkedIn ビジネスアカウントにアクセスできる必要があります。

   ![](assets/linkedin-login.png)

1. LinkedIn にログインした後、Marketo に戻り、「**許可**」をクリックします。

   ![](assets/linkedin-lead-gen-authorize.png)

1. プロンプトが表示されたら、「**許可**」をクリックして、LinkedIn への Marketo アプリケーションのインストールを受け入れます。

   ![](assets/linkedin-marketo-allow.png)

1. これで、権限が与えられたことに気が付くでしょう。「**次へ**」をクリックします。

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >サービスの有効期限は、認証後 1 年で自動的に切れます。アクセスを再開するには、「**再認証**」をクリックするだけです。ブラウザーの設定に応じて、LinkedIn のパスワードを再入力する必要が生じる場合があります。

1. LinkedIn リード生成のリードを Marketo に表示させるアカウントを選択し、「**次へ**」をクリックします。

   >[!TIP]
   >
   >予期するビジネスアカウントが表示されない場合は、許可されているユーザーの LinkedIn アカウントに、LinkedIn のビジネスアカウントに対するリード生成フォームのマネージャー権限があることを確認してください。

   ![](assets/linkedin-pages-to-capture.png)

1. デフォルトの LinkedIn から Marketo へのフィールドマッピングを受け入れるには、「**作成**」をクリックします。デフォルトのフィールドマッピングの変更、フィールドマッピングの削除、新しいフィールドマッピングの追加をおこなう場合は、以下のモーダルを通じて、フィールド単位でこれを実行できます。

   >[!CAUTION]
   >
   >Marketo は、2 つの LinkedIn フィールドの単一の Marketo フィールドへのマッピングをサポートしています。**ただし**、2 つの LinkedIn フィールドが同じフォーム上にないときに限ります。同じ LinkedIn フォームの 2 つのフィールドを 1 つの Marketo フィールドにマッピングした場合、Marketo データベースにユーザーが入力されないことがあります。

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >LinkedIn Campaign Manager の[フォームテンプレート](https://www.linkedin.com/help/lms/answer/79634)にすでに保存されている LinkedIn フィールドのみが、Marketo フィールドにマップできる LinkedIn フィールドとして表示されます。

   ![](assets/linkedin-installed-services.png)

これで完了です。LinkedIn リード生成フォームを送信するユーザーは、LinkedIn 側でキャンペーンを正常に実行すると、Marketo に入力されます。

>[!NOTE]
>
>1 つの LinkedIn ユーザーアカウントのみを認証できます。Marketo にリンクする複数のビジネスアカウントがある場合は、許可されているユーザーの LinkedIn アカウントに、LinkedIn のビジネスアカウントに対するリード生成フォームマネージャー権限があることを確認してください。

>[!MORELIKETHIS]
>
>[スマートキャンペーンでの LinkedIn リード生成フォームのフィルターとトリガーの使用](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)
