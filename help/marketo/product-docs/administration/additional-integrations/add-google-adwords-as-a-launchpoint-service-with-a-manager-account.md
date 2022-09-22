---
unique-page-id: 7504893
description: マネージャーアカウントによる Google AdWords を LaunchPoint サービスとして追加 - Marketo ドキュメント - 製品ドキュメント
title: マネージャーアカウントによる Google AdWords を LaunchPoint サービスとして追加
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
source-git-commit: 457b4aadac47b0a8614c3e6025d2e1ae287b5ecc
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 71%

---

# マネージャーアカウントによる Google AdWords を LaunchPoint サービスとして追加 {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

Google AdWords アカウントを Marketo にリンクすることで、オフラインのコンバージョンデータを Marketo から Google AdWords に自動的にアップロードできます。その後、AdWords UI から、どのクリックが選定リード、商談、新規顧客（または追跡したい収益ステージ）につながったかを簡単に確認できます  [カスタム列を追加](https://support.google.com/adwords/answer/3073556)AdWords の {target=&quot;_blank&quot;}。 この情報は、Marketo UI には表示されません。

複数のGoogle Adwords アカウントがある場合、 [Google AdWords Manager アカウント](https://www.google.com/adwords/manager-accounts/){target=&quot;_blank&quot;}（旧称：マイクライアントセンター）を使用して、Marketoと統合できます。

詳細情報： [Googleのオフライン変換インポート機能](https://support.google.com/adwords/answer/2998031?hl=ja){target=&quot;_blank&quot;}。

>[!AVAILABILITY]
>
>すべての顧客がこの機能を購入したわけではありません。詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

>[!NOTE]
>
>**管理者権限が必要**

>[!NOTE]
>
>また、 [スタンドアロンのGoogle AdWords は Launchpoint サービスとしてアカウントされる](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md){target=&quot;_blank&quot;}。

1. 「**管理者**」セクションに移動します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-1.png)

1. 「**LaunchPoint**」を選択します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-2.png)

1. 「**新規**」ドロップダウンをクリックして、「**新規サービス**」を選択します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-3.png)

1. 表示名を入力し、「**Google AdWords**」を選択します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-4.png)

1. 「**Marketo を承認**」を選択します。

   >[!NOTE]
   >
   >個人の Gmail アカウントからログアウトし、ポップアップを有効にします。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-5.png)

1. **Google AdWords** に関連付けられたアカウントを選択します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-6.png)

1. 「**確定**」をクリックします。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-7.png)

1. ステータスは「**成功**」と表示されます。「**次へ**」を選択します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-8.png)

1. Marketo から Google AdWords にオフラインコンバージョンをアップロードする送信頻度として、「**毎週**」または「**毎日**」を選択します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-9.png)

1. 属性コンバージョンで、「**最初のクリック**」または「**最後のクリック**」を選択します。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-10.png)

   | タイプ | 定義 |
   |---|---|
   | 最初のクリック | オフラインコンバージョンは、過去 90 日間にユーザーが最初にクリックした AdWords に関連付けられます |
   | 最後のクリック | オフラインコンバージョンは、最後にクリックした AdWords とユーザーがクリックした広告に関連付けられます |

   >[!NOTE]
   >
   >[自動タグ付け](https://support.google.com/adwords/answer/1752125?hl=ja)この機能を動作させるには、{target=&quot;_blank&quot;} を選択する必要があります。 AdWords 内で有効化する必要があります。

1. 「**次へ**」をクリックします。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-11.png)

1. 更新しないアカウントの選択を解除します。「**作成**」をクリックします。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-12.png)

   以下の関連記事を参照して、売上高モデルで AdWords のオフラインコンバージョンをマッピングする方法をご確認ください。

   >[!MORELIKETHIS]
   >
   >[マネージャーアカウントを使用した売上高モデルでの Google AdWords コンバージョンの設定](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md){target=&quot;_blank&quot;}
