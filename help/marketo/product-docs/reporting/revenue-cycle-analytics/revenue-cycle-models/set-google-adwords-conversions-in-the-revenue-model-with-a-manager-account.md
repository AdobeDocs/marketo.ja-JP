---
unique-page-id: 7504923
description: マネージャーアカウントを使用した収益モデルでの  [!DNL Google AdWords]  コンバージョンの設定 - Marketo ドキュメント - 製品ドキュメント
title: マネージャーアカウントを使用した収益モデルでの  [!DNL Google AdWords]  コンバージョンの設定
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 100%

---

# マネージャーアカウントを使用した収益モデルでの [!DNL Google AdWords] コンバージョンの設定 {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

[!DNL Google AdWords] アカウントを Marketo にリンクして、オフラインのコンバージョンデータを Marketo から [!DNL Google AdWords] に自動的にアップロードします。[!DNL AdWords] に[カスタム列を追加](https://support.google.com/adwords/answer/3073556)した後、[!DNL AdWords] UI を使って、どのクリックが適格なリード、商談、新規顧客（またはトラックする収益ステージ）につながったかを簡単に確認できるようになります。

複数の [!DNL Google Adwords] アカウントがある場合、[[!DNL Google AdWords]  マネージャーアカウント](https://www.google.com/adwords/manager-accounts/)（旧称：マイクライアントセンター）を使用して、Marketo と統合できます。

[!DNL AdWords] オフラインコンバージョンを収益モデルの 1 つ以上のステージにマッピングできます。次の 2 つの方法があります。

* ステージアクション
* [!DNL AdWords] マッピング

>[!PREREQUISITES]
>
>[マネージャーアカウントで  [!DNL Google AdWords]  を Launchpoint サービスとして追加](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## ステージアクションの使用 {#use-stage-action}

ステージアクションで [!DNL AdWords] コンバージョンをマッピングします。

1. [!DNL AdWords] コンバージョンにマッピングする手順を選択します。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. **[!UICONTROL ステージアクション]**&#x200B;ドロップダウンで、「**[!UICONTROL AdWords コンバージョンを設定]**」を選択します。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. **[!DNL AdWords]コンバージョン**&#x200B;を設定します。

   >[!NOTE]
   >
   >子アカウントごとに異なる [!DNL AdWords] コンバージョンを選択できます。

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   ヒント：[!DNL AdWords] コンバージョンがない場合は、「**[!UICONTROL + 新しいコンバージョン]**」をクリックして作成します。

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-3-27-17-3a21-3a15.png)

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

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. **コンバージョン名**&#x200B;を入力します。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   これで完了です。この新しいコンバージョンは、[!DNL AdWords] アカウントに表示されます。

## [!DNL AdWords] マッピングの使用 {#use-adwords-mapping}

[!DNL AdWords] マッピングを使用して、すべてのモデルステージを [!DNL AdWords] コンバージョンに 1 か所で関連付けることができます。

1. 「**[!UICONTROL AdWords マッピングを編集]**」を選択します。

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. 追跡する各ステージで、目的の **[!DNL AdWords]アカウント**&#x200B;と目的の **[!DNL AdWords]コンバージョン**&#x200B;を選択します。

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. ステージをマッピングしたら、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. すべての [!DNL AdWords] コンバージョンを収益ステージにマッピングしたら、概要ページに戻ります。「**[!UICONTROL モデルアクション]**」を選択し、「**[!UICONTROL ステージを承認]**」を選択します。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

オフラインのコンバージョンデータを表示するには、[!DNL AdWords] アカウントにログインする必要があります。[カスタム列機能](https://support.google.com/adwords/answer/3073556)を使用して、Marketo に読み込むオフラインコンバージョンごとにコンバージョン数の列を作成することをお勧めします。
