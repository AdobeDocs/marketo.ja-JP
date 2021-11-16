---
unique-page-id: 7504893
description: Google AdWords を Manager アカウントで Launchpoint サービスとして追加する — Marketoドキュメント — 製品ドキュメント
title: マネージャーアカウントによる Google AdWords を LaunchPoint サービスとして追加
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
source-git-commit: ab8eb044b89c925accc3b6a4ac4def53e3927321
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 70%

---

# マネージャーアカウントによる Google AdWords を LaunchPoint サービスとして追加 {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

Google AdWords アカウントを Marketo にリンクすることで、オフラインのコンバージョンデータを Marketo から Google AdWords に自動的にアップロードできます。[カスタム列を追加した後には](https://support.google.com/adwords/answer/3073556)、AdWords UI を使って、どのクリックが資格を満たすリード、商談、新規顧客 (あるいは追跡した売上高ステージ) につながったかを簡単に確認できるようになります。この情報は、Marketo UI には表示されません。

複数のGoogle Adwords アカウントがある場合、 [Google AdWords Manager アカウント](https://www.google.com/adwords/manager-accounts/) （旧称：マイクライアントセンター）を使用して、Marketoと統合できます。

詳細は、[Google のオフラインコンバージョンのインポート機能](https://support.google.com/adwords/answer/2998031?hl=ja)に関する説明を参照してください。

>[!AVAILABILITY]
>
>すべての顧客がこの機能を購入したわけではありません。詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

>[!NOTE]
>
>**管理者権限が必要**

>[!NOTE]
>
>また、 [スタンドアロンのGoogle AdWords は Launchpoint サービスとしてアカウントされる](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md).

1. **管理**&#x200B;セクションに移動します。

   ![](assets/login-admin-1.png)

1. 「**LaunchPoint**」を選択します。

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. 「**新規**」と「**新規サービス**」を選択します。

   ![](assets/image2015-2-23-14-3a54-3a50.png)

1. 表示名を入力し、「 」を選択します。 **Google AdWords**.

   ![](assets/new-service-google-1.png)

1. 「**Marketo を承認**」を選択します。

   >[!NOTE]
   >
   >個人の Gmail アカウントからログアウトし、ポップアップを有効にします。

   ![](assets/image2015-2-26-20-3a54-3a1.png)

1. 次に関連するアカウントを選択 **Google AdWords**.

   ![](assets/image2015-2-23-15-3a31-3a16.png)

1. 「**承認**」を選択します。

   ![](assets/image2015-2-23-16-3a32-3a45.png)

1. ステータスは「**成功**」と表示されます。「**次へ**」を選択します。

   ![](assets/image2015-2-26-20-3a55-3a21.png)

1. Marketo から Google AdWords にオフラインコンバージョンをアップロードする送信頻度として、「**毎週**」または「**毎日**」を選択します。

   ![](assets/image2015-3-27-14-3a7-3a45.png)

1. 属性コンバージョンで、「**最初のクリック**」または「**最後のクリック**」を選択します。

   | タイプ | 定義 |
   |---|---|
   | 最初のクリック | オフラインコンバージョンは、過去 90 日間にユーザーが最初にクリックした AdWords に関連付けられます |
   | 最後のクリック | オフラインコンバージョンは、最後にクリックした AdWords とユーザーがクリックした広告に関連付けられます |

   ![](assets/image2015-3-27-14-3a10-3a46.png)

   >[!NOTE]
   >
   >この機能を使用するには、[自動タグ付け](https://support.google.com/adwords/answer/1752125?hl=ja)を選択する必要があります。AdWords 内で有効化する必要があります。

1. 「**次へ**」をクリックします。

   ![](assets/image2015-3-27-14-3a11-3a31.png)

1. 更新しないアカウントの選択を解除します。 「**作成**」をクリックします。

   ![](assets/image2015-3-27-14-3a12-3a51.png)

   次に、収益モデルで AdWords オフラインコンバージョンをマッピングする方法について、以下の関連記事を参照してください。

   >[!MORELIKETHIS]
   >
   >[マネージャーアカウントを使用した売上高モデルでの Google AdWords コンバージョンの設定](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md)
