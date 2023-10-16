---
unique-page-id: 1147108
description: プログラムのインポート - Marketo ドキュメント - 製品ドキュメント
title: プログラムのインポート
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
feature: Programs
source-git-commit: e49860ae611f2f77789bb491aeccbee46a911a2c
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 74%

---

# プログラムのインポート {#import-a-program}

プログラムは、ある Marketo サブスクリプションから別のサブスクリプションにインポートできます。例えば、サンドボックスでプログラムを作成し、ライブサブスクリプションにインポートできます。また、事前に作成されたプログラムを [Marketo Program Library](/help/marketo/product-docs/core-marketo-concepts/programs/program-library/program-import-library-overview.md){target="_blank"}.

## プログラムのインポート {#importing-a-program}

1. 「**[!UICONTROL マーケティングアクティビティ]**」に移動します。

   ![](assets/import-a-program-1.png)

1. 次をクリック： **[!UICONTROL 新規]** ドロップダウンして「 」を選択します。 **[!UICONTROL プログラムの読み込み]**.

   ![](assets/import-a-program-2.png)

   >[!NOTE]
   >
   >プログラムのインポートは、「プログラムのインポート」権限が有効になっているロールを持つユーザのみが使用できます。詳しくは、[ユーザのロールと権限の管理](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}を参照してください。
   >
   >Sandbox アカウントを Live サブスクリプションに接続するには、にお問い合わせください。 [Marketoサポート](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. Marketo **[!UICONTROL サブスクリプション]**&#x200B;を選択してインポートするプログラムを選択します。「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/import-a-program-3.png)

1. インポートされたプログラム用の&#x200B;**[!UICONTROL キャンペーンフォルダー]**&#x200B;を指定します。「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/import-a-program-4.png)

   >[!NOTE]
   >
   >「**[!UICONTROL デフォルトの競合を使用]**」ルールが選択されている事を確認します。同じ名前のアセットを持つインスタンスにプログラムを読み込む場合は、競合ルールが必要です。

1. 目的の競合の詳細を選択し、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/import-a-program-5.png)

   >[!NOTE]
   >
   >互換性のあるサービスプロバイダーが複数ある宛先インスタンスに、カスタムフローステップまたはフローステップから派生したスマートリストルールを使用するプログラムをインポートすると、宛先インスタンスの正しいサービスプロバイダーに割り当てるよう求められます。

1. 詳細をプレビューし、プログラムを「**[!UICONTROL インポート]**」します。

   ![](assets/import-a-program-6.png)

インポートが完了すると、確認のメールが送信されます。

>[!NOTE]
>
>インポートしたバッチキャンペーンを再スケジュールし、トリガーキャンペーンを有効にする必要があります。インポートされたプログラム内のキャンペーンスケジュールおよびトリガーキャンペーンが自動的に無効化されます。

## プログラムインポート中の外部アセットへの影響 {#impact-on-external-assets-during-program-imports}

プログラムは、電子メールテンプレート、ランディングページテンプレート、画像、フォーム、トークン、プログラムタグなどの外部アセットを使用します。 ランディングページのテンプレートとプログラムタグの処理方法を設定でき、残りはMarketoが自動的に管理します。

**メール／ランディングページテンプレート：**&#x200B;メール／ランディングページテンプレートがデザインスタジオに読み込まれます。同じ名前のテンプレートが存在する場合、競合ルールを使用して動作を設定できます。同じ名前が存在する場合は、デフォルトのルールを使用して、テンプレートに数字が追加されます。例えば、「標準テンプレート」という名前のテンプレートが既に存在する場合、新しいテンプレートの名前は「標準テンプレート - 1」になります。

**ランディングページ/Forms:** 同じ名前のフォームまたはランディングページが Design Studio に存在する場合、それらは引き続き読み込まれますが、名前に数字が追加されます（例：ランディングページ — 1）。

**画像：** ランディングページで使用される画像は、同じ名前の画像が存在しない限り、デザインスタジオに読み込まれます。

**トークン：**&#x200B;プログラム外に存在するトークンは、インポートプロセス中にローカルトークンに変換されます。

>[!CAUTION]
>
>プログラムのインポートでは、イメージタイプマイトークンはサポートされていません。マイトークンのイメージタイプを含むプログラムがインポートされる場合、すべてのトークンが&#x200B;_インポートされません_。

**プログラムタグ：**&#x200B;競合ルールを使用して、宛先アカウントに存在しないプログラムタグの処理方法を制御できます。デフォルトのルールを使用すると、プログラムタグが作成されます。または、タグを無視するように選択することもできます。

>[!CAUTION]
>
>プログラムをインポートする際に、 [動的コンテンツ](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md){target="_blank"} がスキップされます。
