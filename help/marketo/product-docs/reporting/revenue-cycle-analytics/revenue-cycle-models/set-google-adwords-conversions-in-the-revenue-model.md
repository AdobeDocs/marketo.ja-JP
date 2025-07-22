---
unique-page-id: 6095029
description: 収益モデルでの Set [!DNL Google AdWords] Conversions - Marketo ドキュメント – 製品ドキュメント
title: 収益モデルでのセ  [!DNL Google AdWords]  トコンバージョン
exl-id: dd1259fc-d3f2-44ec-8055-f75d55263b36
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 38%

---

# 収益モデルでの [!DNL Google AdWords] コンバージョンの設定 {#set-google-adwords-conversions-in-the-revenue-model}

[!DNL Google AdWords] アカウントを Marketo にリンクして、オフラインのコンバージョンデータを Marketo から [!DNL Google AdWords] に自動的にアップロードします。その後、[!DNL AdWords] UI から、[ で ](https://support.google.com/adwords/answer/3073556) カスタム列を追加 [!DNL AdWords] した後、どのクリックが適格なリード、商談、新規顧客（または追跡したい収益ステージ）につながったかを簡単に確認できます。

>[!NOTE]
>
>これは、Marketoから [!DNL Google AdWords] へのプッシュ統合です。 コンバージョンデータは、_ポータルに_ のみ [!DNL Google AdWords] 表示され、Marketo UI には _表示されません_。

詳細は、[Google のオフラインコンバージョンインポート機能](https://support.google.com/adwords/answer/2998031?hl=en)を参照してください。収益モデル [!DNL AdWords]1 つ以上のステージにオフラインコンバージョンをマッピングします。 マッピングをおこなう方法は 3 つあります。

* [!DNL AdWords] Conversion
* ステージアクション
* [!DNL AdWords] マッピング

ステージアクションを使用する場合は [!DNL AdWords]Marketoから新しいオフラインコンバージョンを作成できます。

>[!PREREQUISITES]
>
>[LaunchPoint サ  [!DNL Google AdWords]  ビスとして追加 ](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## コンバージョン [!DNL AdWords] 使用 {#use-adwords-conversion}

1. **[!UICONTROL Analytics]** エリアに移動します。

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. モデルを選択します。

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. **[!UICONTROL ドラフトの編集]**&#x200B;をクリックします。

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. コンバージョンにマッピングする収益ステー [!DNL AdWords] を選択します。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Marketo ステージにマッピングする **[!UICONTROL AdWords コンバージョン]**&#x200B;を選択します。

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   作業は以上です。[!DNL AdWords] コンバージョンデータは、選択した頻度で [!DNL Google AdWords] にアップロードされます。

## ステージアクションを使用する {#use-stage-action}

また、「[!UICONTROL  ステージアクション ]」の下で **[!UICONTROL AdWords コンバージョン]** をマッピングすることもできます。

1. [!DNL AdWords] 変換にマッピングするステップを選択します。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. **[!UICONTROL ステージアクション]**&#x200B;ドロップダウンで、「**[!UICONTROL AdWords コンバージョンを設定]**」を選択します。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 「**[!UICONTROL AdWords コンバージョン]**」を選択します。

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **ヒント**:[!DNL AdWords] しいコンバージョンがない場合は、「**[!UICONTROL +新規コンバージョン]**」をクリックして作成します。

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. すべての [!DNL AdWords] コンバージョンの売上高ステージへのマッピングが完了したら、概要ページに戻ります。 「**[!UICONTROL モデルアクション]**」を選択し、「**[!UICONTROL ステージの承認]**」を選択します。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## 上級ヒント：新しいコンバージョンを追加する {#pro-tip-add-a-new-conversion}

上級向けのヒントです。新しい [!DNL AdWords] オフラインコンバージョンをMarketoから作成できます。

>[!CAUTION]
>
>Marketo から作成された新しいコンバージョンでは、「最適化」設定が有効になっています。つまり、入札戦略 [!DNL AdWords] よって、これらのコンバージョンに対する入札を最適化できます。 この設定は [!DNL AdWords] アカウントから変更できます。

1. **[!UICONTROL ステージアクション]**&#x200B;ドロップダウンで、「**[!UICONTROL AdWords コンバージョンを設定]**」を選択します。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 「**[!UICONTROL 新しいコンバージョン]**」を選択します。

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. **[!UICONTROL コンバージョン名]**&#x200B;を入力します。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   これで完了です。この新しいコンバージョンは、[!DNL AdWords] アカウントに表示されます。

## [!DNL AdWords] マッピングの使用 {#use-adwords-mapping}

[!UICONTROL  マッピングを使用すると、すべてのモデルステージを ]AdWords コンバージョン [!DNL AdWords] に 1 か所で関連付けることができます。

1. 「**[!UICONTROL AdWords マッピングの編集]**」を選択します。

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. 追跡する各ステージで、目的の **[!UICONTROL AdWords コンバージョン]**&#x200B;を選択します。

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. ステージをマッピングしたら、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. すべての [!DNL AdWords] コンバージョンの売上高ステージへのマッピングが完了したら、概要ページに戻ります。 「**[!UICONTROL モデルアクション]**」を選択し、「**[!UICONTROL ステージの承認]**」を選択します。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

オフラインコンバージョンデータを表示するには、[!DNL AdWords] アカウントにログインする必要があります。 [カスタム列機能](https://support.google.com/adwords/answer/3073556)を使用して、Marketo にインポートするオフラインコンバージョンごとにコンバージョン数の列を作成することをお勧めします。
