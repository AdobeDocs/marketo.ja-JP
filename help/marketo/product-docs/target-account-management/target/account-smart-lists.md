---
unique-page-id: 11378814
description: アカウントスマートリスト - Marketo ドキュメント - 製品ドキュメント
title: アカウントスマートリスト
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
feature: Target Account Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 100%

---

# アカウントスマートリスト {#account-smart-lists}

ここでは、価値の高いアカウントを迅速かつ正確に特定する方法を説明します。

>[!NOTE]
>
>この機能は、[!UICONTROL ターゲットアカウント管理]アドオンと TAM のライセンスが発行されたユーザのみが使用できます。

## [!UICONTROL アカウントスマートリスト]の作成 {#create-an-account-smart-list}

1. Marketo で、**[!UICONTROL マーケティングアクティビティ]**&#x200B;に移動します。

   ![](assets/account-smart-lists-1.png)

1. 目的のプログラムを見つけて選択します。

   ![](assets/account-smart-lists-2.png)

1. **[!UICONTROL 新規作成]**&#x200B;ドロップダウンをクリックし、**[!UICONTROL 新規ローカルアセット]**&#x200B;を選択します。

   ![](assets/account-smart-lists-3.png)

1. 「**[!UICONTROL アカウントスマートリスト]**」をクリックします。

   ![](assets/account-smart-lists-4.png)

1. 名前を入力し、「**[!UICONTROL 作成]**」をクリックします（説明とラベルはオプションです）。

   ![](assets/account-smart-lists-5.png)

[!UICONTROL アカウントスマートリスト]が作成されました。ルールの定義手順について詳しくは、以下を参照してください。

## [!UICONTROL アカウントスマートリスト]のルール {#account-smart-list-rules}

[!UICONTROL アカウントスマートリスト]は、標準のスマートリストと同様に機能しますが、コンテナという顕著な例外があります。

1. [!UICONTROL アカウントスマートリスト]を定義するには、「**[!UICONTROL アカウントスマートリストのルール]**」タブをクリックします。

   ![](assets/account-smart-lists-6.png)

1. 目的の「アカウントフィルター」を選択します。この例では、_[!UICONTROL 業種]は「[!UICONTROL 医療]_」を選択します。

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

   >[!NOTE]
   >
   >[アカウントプロファイリングのランキングと調整](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md)で使用された ICP 指標データは、アカウントスマートリストで使用するカスタムアカウント属性として表示されます。このカスタム属性データは、アカウントプロファイルモデルが作成または更新された日時に基づいています。

1. 「一致するリード」フィルターを選択します。この例では、「_州はカリフォルニア_」を選択します。

   ![](assets/account-smart-lists-9.png)

**オプションの手順**：ここにコンテナを配置します。追加の「一致するリードフィルター」を選択する場合は、最初のフィルターの下にドロップするか、フィルターの&#x200B;_中_&#x200B;にドロップすると、コンテナを作成できます。この例では、「_職位は CFO_」を追加してコンテナを作成します。

![](assets/account-smart-lists-10.png)

コンテナは以下のように表示されます。

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>フィルターのコンテナを作成すると、「and」ルールが作成され、結合された結果のみが返されます。この例では、業種が医療業界で、カリフォルニア州に所在し、_さらに_ CFO として登録されているアカウントが返されます。コンテナを利用しない場合は、既存のコンテナの下または上にフィルターをドロップします。

これで完了です。[!UICONTROL アカウントスマートリスト]の活用方法について詳しくは、以下の節を参照してください。

>[!TIP]
>
>標準のスマートリストと同様に、高度なロジックを使用して結果をさらに絞り込むことができます。これを行うには、3 つ以上のフィルターが必要です。[!UICONTROL アカウントスマートリスト]では、1 つのコンテナ（自身に含まれるフィルターの数に関係なく）が 1 つのフィルターと等しくなります。

## [!UICONTROL アカウントスマートリスト]アクション {#account-smart-list-actions}

[!UICONTROL アカウントスマートリスト]の「概要」タブには、アクションのオプションがいくつか表示されます。

**[!UICONTROL 書き出し]**：[!UICONTROL アカウントスマートリスト]の結果が CSV として書き出されます。

**[!UICONTROL 複製]**：[!UICONTROL アカウントスマートリスト]のコピーを作成します。

**[!UICONTROL 広告ネットワークに送信]**：新しい一致オーディエンスとして、リストを [!DNL LinkedIn] に送信します。

また、「_[!UICONTROL アカウントスマートリストのユーザメンバー]_」フィルターを使用して、標準のスマートキャンペーン／リストで[!UICONTROL アカウントスマートリスト]を参照することもできます。

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>「[!UICONTROL アカウントスマートリストのユーザメンバー]」の結果は、アカウントスマートリストの「一致するリード」フィルターで見つかった人だけでなく、識別されたアカウントのすべての人を表示します。

>[!NOTE]
>
>**定義**
>
>**[!UICONTROL アカウントスマートリストのリードメンバー]**：この場合、「メンバー」という単語はアカウント自体を表すので、「リードメンバー」とはアカウント内の実際のリード（Marketo レコード）を表します。
