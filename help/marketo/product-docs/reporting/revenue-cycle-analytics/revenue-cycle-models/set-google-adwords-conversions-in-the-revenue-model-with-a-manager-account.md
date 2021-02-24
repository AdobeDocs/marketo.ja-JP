---
unique-page-id: 7504923
description: マネージャーアカウント — Marketto Docs — 製品ドキュメントを使用した売上高モデルでのGoogle AdWordsコンバージョンの設定
title: マネージャーアカウントを使用した売上高モデルでのGoogle AdWordsコンバージョンの設定
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---


# マネージャーアカウント{#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}を使用した売上高モデルでのGoogle AdWordsコンバージョンの設定

Google AdWordsアカウントをMarketorにリンクして、オフラインコンバージョンデータをMarketoからGoogle AdWordsに自動的にアップロードします。 次に、AdWords UIから、AdWordsにカスタム列](https://support.google.com/adwords/answer/3073556)を追加した後、条件を満たしたリード、オポチュニティ、新規顧客（または追跡したい任意の売上高ステージ）に導いたクリックを簡単に確認できます。[

複数のGoogle Adwordsアカウントがある場合は、[Google AdWords Managerアカウント](https://www.google.com/adwords/manager-accounts/)（旧称My Client Center）を使用して、Marketoと統合できます。

AdWordsのオフラインコンバージョンを、売上高モデルの1つ以上のステージにマッピングできます。 次の2つの方法があります。

* Stage Action
* AdWordsマッピング

>[!PREREQUISITES]
>
>[マネージャーアカウントを追加持つLaunchpointサービスとしてのGoogle AdWords](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## Use Stage Action {#use-stage-action}

「ステージアクション」の下のAdWordsコンバージョンのマッピングを参照してください。

1. AdWordsコンバージョンにマッピングする手順を選択します。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. 「**ステージアクション**」ドロップダウンで、「**AdWordsコンバージョンを設定**」を選択します。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. **AdWordsコンバージョン**&#x200B;を設定します。

   >[!NOTE]
   >
   >子アカウントごとに異なるAdWordsコンバージョンを選択できます。

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   ヒント：AdWordsの変換がない場合は、**+新しい変換**&#x200B;をクリックして作成します。

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. 「**保存**」をクリックします。

   ![](assets/image2015-3-27-17-3a21-3a15.png)

1. すべてのAdWordsコンバージョンの売上高ステージへのマッピングが完了したら、サマリページに戻ります。 「**モデルアクション**」を選択し、「**ステージを承認**」を選択します。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## プロのヒント：追加新しいコンバージョン{#pro-tip-add-a-new-conversion}

プロチップ！ 新しいAdWordsオフラインコンバージョンは、Marketoから作成できます。

>[!CAUTION]
>
>Marketorから作成された新しいコンバージョンでは、「最適化」設定が有効になっています。 つまり、AdWords入札戦略では、これらのコンバージョンに対する入札を最適化できます。 この設定は、AdWordsアカウントで変更できます。

1. 「**ステージアクション**」ドロップダウンで、「**AdWordsコンバージョンを設定**」を選択します。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 「**新しいコンバージョン**」を選択します。

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. **コンバージョン名**&#x200B;を入力します。 「**保存**」をクリックします。

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   素晴らしい！ この新しいコンバージョンは、AdWordsアカウントに表示されます。

## AdWordsマッピングを使用{#use-adwords-mapping}

AdWordsのマッピングを使用して、すべてのモデルステージをAdWordsコンバージョンに1か所で関連付けることができます。

1. 「**AdWordsのマッピングを編集**」を選択します。

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. 追跡する各ステージに対して、目的の&#x200B;**AdWordsアカウント**&#x200B;と、目的の&#x200B;**AdWordsコンバージョン**&#x200B;を選択します。

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. ステージをマッピングしたら、「**保存**」をクリックします。

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. すべてのAdWordsコンバージョンの売上高ステージへのマッピングが完了したら、サマリページに戻ります。 「**モデルアクション**」を選択し、「**ステージを承認**」を選択します。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

オフラインコンバージョンデータを表示するには、AdWordsアカウントにログインする必要があります。 [カスタム列機能](https://support.google.com/adwords/answer/3073556)を使用して、Marketoからインポートしたオフラインコンバージョンごとにコンバージョン数の列を作成することをお勧めします。
