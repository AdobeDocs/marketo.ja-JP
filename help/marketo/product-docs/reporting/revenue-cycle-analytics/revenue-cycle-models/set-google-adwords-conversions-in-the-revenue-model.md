---
unique-page-id: 6095029
description: 収益モデルでの  [!DNL Google AdWords]  コンバージョンの設定 - Marketo ドキュメント - 製品ドキュメント
title: 収益モデルでの  [!DNL Google AdWords]  コンバージョンの設定
exl-id: dd1259fc-d3f2-44ec-8055-f75d55263b36
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 100%

---

# 収益モデルでの [!DNL Google AdWords] コンバージョンの設定 {#set-google-adwords-conversions-in-the-revenue-model}

[!DNL Google AdWords] アカウントを Marketo にリンクして、オフラインのコンバージョンデータを Marketo から [!DNL Google AdWords] に自動的にアップロードします。[!DNL AdWords] に[カスタム列を追加](https://support.google.com/adwords/answer/3073556)した後、[!DNL AdWords] UI を使って、どのクリックが適格なリード、商談、新規顧客（またはトラックする収益ステージ）につながったかを簡単に確認できるようになります。

>[!NOTE]
>
>これは、Marketo から [!DNL Google AdWords] へのプッシュ統合です。コンバージョンデータは、[!DNL Google AdWords] のポータルで&#x200B;_のみ_&#x200B;表示され、Marketo のユーザインタフェイスでは表示&#x200B;_されません_。

詳しくは、[Google のオフラインコンバージョンの読み込み機能](https://support.google.com/adwords/answer/2998031?hl=en)を参照してください。[!DNL AdWords] オフラインコンバージョンを収益モデルの 1 つ以上のステージにマッピングします。マッピングを行う方法は 3 つあります。

* [!DNL AdWords] コンバージョン
* ステージアクション
* [!DNL AdWords] マッピング

ステージアクションを使用すると、Marketo から新しい [!DNL AdWords] オフラインコンバージョンを作成できます。

>[!PREREQUISITES]
>
>[ [!DNL Google AdWords]  を LaunchPoint サービスとして追加](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## [!DNL AdWords] コンバージョンの使用 {#use-adwords-conversion}

1. **[!UICONTROL Analytics]** エリアに移動します。

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. モデルを選択します。

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. **[!UICONTROL ドラフトの編集]**&#x200B;をクリックします。

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. [!DNL AdWords] コンバージョンにマッピングする収益ステージを選択します。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Marketo ステージにマッピングする **[!UICONTROL AdWords コンバージョン]**&#x200B;を選択します。

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   作業は以上です。[!DNL AdWords] コンバージョンデータは、選択したケイデンスで [!DNL Google AdWords] にアップロードされます。

## ステージアクションの使用 {#use-stage-action}

**[!UICONTROL ステージアクション]**&#x200B;で [!UICONTROL AdWords コンバージョン]をマッピングすることもできます。

1. [!DNL AdWords] コンバージョンにマッピングする手順を選択します。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. **[!UICONTROL ステージアクション]**&#x200B;ドロップダウンで、「**[!UICONTROL AdWords コンバージョンを設定]**」を選択します。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 「**[!UICONTROL AdWords コンバージョン]**」を選択します。

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **ヒント**：[!DNL AdWords] コンバージョンがない場合は、「**[!UICONTROL + 新しいコンバージョン]**」をクリックして作成します。

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. すべての [!DNL AdWords] コンバージョンを収益ステージにマッピングしたら、概要ページに戻ります。「**[!UICONTROL モデルアクション]**」を選択し、「**[!UICONTROL ステージを承認]**」を選択します。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## 上級ヒント：新しいコンバージョンを追加する {#pro-tip-add-a-new-conversion}

上級向けのヒントです。新しい [!DNL AdWords] オフラインコンバージョンは、Marketo から作成できます。

>[!CAUTION]
>
>Marketo から作成された新しいコンバージョンでは、「最適化」設定が有効になっています。つまり、このコンバージョンについては、[!DNL AdWords] の入札方針を利用して入札を最適化できるということです。この設定は、[!DNL AdWords] アカウントから変更できます。

1. **[!UICONTROL ステージアクション]**&#x200B;ドロップダウンで、「**[!UICONTROL AdWords コンバージョンを設定]**」を選択します。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 「**[!UICONTROL 新しいコンバージョン]**」を選択します。

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. **[!UICONTROL コンバージョン名]**&#x200B;を入力します。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   これで完了です。この新しいコンバージョンは、[!DNL AdWords] アカウントに表示されます。

## [!DNL AdWords] マッピングの使用 {#use-adwords-mapping}

[!DNL AdWords] マッピングを使用して、すべてのモデルステージを [!UICONTROL AdWords コンバージョン]に 1 か所で関連付けることができます。

1. 「**[!UICONTROL AdWords マッピングの編集]**」を選択します。

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. 追跡する各ステージで、目的の **[!UICONTROL AdWords コンバージョン]**&#x200B;を選択します。

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. ステージをマッピングしたら、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. すべての [!DNL AdWords] コンバージョンを収益ステージにマッピングしたら、概要ページに戻ります。「**[!UICONTROL モデルアクション]**」を選択し、「**[!UICONTROL ステージを承認]**」を選択します。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

オフラインのコンバージョンデータを表示するには、[!DNL AdWords] アカウントにログインする必要があります。[カスタム列機能](https://support.google.com/adwords/answer/3073556)を使用して、Marketo に読み込むオフラインコンバージョンごとにコンバージョン数の列を作成することをお勧めします。
