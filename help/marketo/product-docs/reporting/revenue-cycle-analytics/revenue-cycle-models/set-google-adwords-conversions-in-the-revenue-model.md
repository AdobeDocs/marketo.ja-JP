---
unique-page-id: 6095029
description: 売上高モデルで Google AdWords コンバージョンを設定する — Marketo ドキュメント — 製品ドキュメント
title: 売上高モデルで Google AdWords コンバージョンを設定する
exl-id: dd1259fc-d3f2-44ec-8055-f75d55263b36
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '503'
ht-degree: 100%

---

# 売上高モデルで Google AdWords コンバージョンを設定する {#set-google-adwords-conversions-in-the-revenue-model}

Google AdWords のアカウントを Marketo とリンクすると、オフラインのコンバージョンデータが Marketo から GoogleAdWords に自動的にアップロードされます。[カスタム列を追加した後には](https://support.google.com/adwords/answer/3073556)、AdWords UI を使って、どのクリックが資格を満たすリード、商談、新規顧客 (あるいは追跡した売上高ステージ) につながったかを簡単に確認できるようになります。

>[!NOTE]
>
>これは、Marketo から Google AdWords へのプッシュ統合です。コンバージョンデータは、Google AdWords のポータルで&#x200B;_のみ_&#x200B;表示され、Marketo のユーザーインタフェイスでは表示&#x200B;_されません_。

詳細は、[Google のオフラインコンバージョンインポート機能](https://support.google.com/adwords/answer/2998031?hl=en)を参照してください。AdWords オフラインコンバージョンを売上高モデルの 1 つ以上のステージにマッピングします。マッピングをおこなう方法は 3 つあります。

* AdWords コンバージョン
* ステージアクション
* AdWords マッピング

ステージアクションを使用すると、Marketo から新しい AdWords オフラインコンバージョンを作成できます。

>[!PREREQUISITES]
>
>[Google AdWords を LaunchPoint サービスとして追加する](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## AdWords コンバージョンを使用する {#use-adwords-conversion}

1. **Analytics** エリアに移動します。

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. モデルを選択します。

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. **ドラフトの編集**&#x200B;をクリックします。

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. AdWords コンバージョンにマッピングする売上高ステージを選択します。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Marketo ステージにマッピングする **AdWords コンバージョン**&#x200B;を選択します。

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   作業は以上です。AdWords コンバージョンデータは、選択したサイクルで Google AdWords にアップロードされます。

## ステージアクションを使用する {#use-stage-action}

ステージアクションで AdWords コンバージョンをマッピングすることもできます。

1. AdWords コンバージョンにマッピングする手順を選択します。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. **ステージアクション**&#x200B;ドロップダウンで、「**AdWords コンバージョンを設定**」を選択します。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 「**AdWords コンバージョン**」を選択します。

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **ヒント**：AdWords 変換がない場合は、「**+新しいコンバージョン**」をクリックして作成します。

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. 「**保存**」をクリックします。

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. すべての AdWords コンバージョンを売上高ステージにマッピングしたら、概要ページに戻ります。「**モデルアクション**」を選択し、「**ステージの承認**」を選択します。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## 上級ヒント：新しいコンバージョンを追加する {#pro-tip-add-a-new-conversion}

上級向けのヒントです。新しい AdWords オフラインコンバージョンは、Marketo から作成できます。

>[!CAUTION]
>
>Marketo から作成された新しいコンバージョンでは、「最適化」設定が有効になっています。つまり、このコンバージョンについては、AdWords の入札方針を利用して入札を最適化できるということです。この設定は、AdWords アカウントから変更できます。

1. **ステージアクション**&#x200B;ドロップダウンで、「**AdWords コンバージョンを設定**」を選択します。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 「**新しいコンバージョン**」を選択します。

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. **コンバージョン名**&#x200B;を入力します。「**保存**」をクリックします。

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   これで完了です。この新しいコンバージョンは、AdWords アカウントに表示されます。

## AdWords マッピングを使用する {#use-adwords-mapping}

AdWords マッピングを使用して、すべてのモデルステージを AdWords コンバージョンに 1 か所で関連付けることができます。

1. 「**AdWords マッピングの編集**」を選択します。

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. 追跡する各ステージで、目的の **AdWords コンバージョン**&#x200B;を選択します。

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. ステージをマッピングしたら、「**保存**」をクリックします。

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. すべての AdWords コンバージョンを売上高ステージにマッピングしたら、概要ページに戻ります。「**モデルアクション**」を選択し、「**ステージの承認**」を選択します。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

オフラインのコンバージョンデータを表示するには、AdWords アカウントにログインする必要があります。[カスタム列機能](https://support.google.com/adwords/answer/3073556)を使用して、Marketo にインポートするオフラインコンバージョンごとにコンバージョン数の列を作成することをお勧めします。
