---
unique-page-id: 6095029
description: 売上高モデル —Marketoドキュメント — 製品ドキュメントでのGoogle AdWordsコンバージョンの設定
title: 売上高モデルでのGoogle AdWordsコンバージョンの設定
exl-id: dd1259fc-d3f2-44ec-8055-f75d55263b36
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# 売上高モデルでのGoogle AdWordsコンバージョンの設定{#set-google-adwords-conversions-in-the-revenue-model}

Google AdWordsアカウントをMarketoにリンクして、オフラインコンバージョンデータをMarketoからGoogle AdWordsに自動的にアップロードします。 次に、AdWords UIから、AdWordsにカスタム列](https://support.google.com/adwords/answer/3073556)を追加した後、条件を満たしたリード、オポチュニティ、新規顧客（または追跡したい任意の売上高ステージ）に導いたクリックを簡単に確認できます。[

>[!NOTE]
>
>これは、MarketoからGoogle AdWordsへのプッシュ統合です。 コンバージョンデータは、Google AdWordsポータルに&#x200B;__&#x200B;のみ&#x200B;_表示され、MarketoのUI_&#x200B;には表示されません。

[Googleのオフラインコンバージョンインポート機能](https://support.google.com/adwords/answer/2998031?hl=en)の詳細を表示します。 AdWordsのオフラインコンバージョンを売上高モデルの1つ以上のステージにマッピングします。 マッピングを行う方法は3つあります。

* AdWordsコンバージョン
* Stage Action
* AdWordsマッピング

Stage Actionを使用する場合は、Marketoから新しいAdWordsオフラインコンバージョンを作成できます。

>[!PREREQUISITES]
>
>[LaunchPoint追加サービスとしてのGoogle AdWords](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## AdWordsコンバージョンを使用{#use-adwords-conversion}

1. 「**Analytics**」領域に移動します。

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. モデルを選択します。

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. 「**ドラフトを編集**」をクリックします。

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. AdWordsコンバージョンにマップする売上高ステージを選択します。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Marketoのステージにマップする&#x200B;**AdWordsコンバージョン**&#x200B;を選択します。

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   ナイス！ AdWordsコンバージョンデータは、選択したカデンスでGoogle AdWordsにアップロードされます。

## Use Stage Action {#use-stage-action}

「Stage Actions」でAdWordsコンバージョンをマッピングすることもできます。

1. AdWordsコンバージョンにマッピングする手順を選択します。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. 「**ステージアクション**」ドロップダウンで、「**AdWordsコンバージョンを設定**」を選択します。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. **AdWordsコンバージョン**&#x200B;を選択します。

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **ヒント**:AdWordsのコンバージョンがない場合は、「 **+新規コンバージョン**」をクリックして作成します。

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. 「**保存**」をクリックします。

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. すべてのAdWordsコンバージョンの売上高ステージへのマッピングが完了したら、サマリページに戻ります。 「**モデルアクション**」を選択し、「**ステージを承認**」を選択します。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## プロのヒント：追加新しいコンバージョン{#pro-tip-add-a-new-conversion}

プロチップ！ 新しいAdWordsオフラインコンバージョンは、Marketoから作成できます。

>[!CAUTION]
>
>Marketoから作成された新しいコンバージョンでは、「最適化」設定が有効になっています。 つまり、AdWords入札戦略では、これらのコンバージョンに対する入札を最適化できます。 この設定は、AdWordsアカウントで変更できます。

1. 「**ステージアクション**」ドロップダウンで、「**AdWordsコンバージョンを設定**」を選択します。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 「**新しいコンバージョン**」を選択します。

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. **コンバージョン名**&#x200B;を入力します。 「**保存**」をクリックします。

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   素晴らしい！ この新しいコンバージョンは、AdWordsアカウントに表示されます。

## AdWordsマッピングを使用{#use-adwords-mapping}

AdWordsのマッピングを使用して、すべてのモデルステージをAdWordsコンバージョンに1か所で関連付けることができます。

1. 「**AdWordsのマッピングを編集**」を選択します。

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. 追跡する各ステージに対して、目的の&#x200B;**AdWordsコンバージョン**&#x200B;を選択します。

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. ステージをマッピングしたら、「**保存**」をクリックします。

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. すべてのAdWordsコンバージョンの売上高ステージへのマッピングが完了したら、サマリページに戻ります。 「**モデルアクション**」を選択し、「**ステージを承認**」を選択します。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

オフラインコンバージョンデータを表示するには、AdWordsアカウントにログインする必要があります。 [カスタム列機能](https://support.google.com/adwords/answer/3073556)を使用して、Marketoからインポートしたオフラインコンバージョンごとにコンバージョン数列を作成することをお勧めします。
