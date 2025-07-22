---
unique-page-id: 12983101
description: カスタムフィールドの Marketo へのマッピング — Marketo ドキュメント — 製品ドキュメント
title: カスタムフィールドの Marketo へのマッピング
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 54%

---

# カスタムフィールドの Marketo へのマッピング {#map-custom-fields-to-marketo}

オンライン配信サービスを使用する頻度など、デフォルトで保存されてい [!DNL Facebook] 標準情報以上の情報を収集したい場合があります。 これを実現するには、[ リード広告で ](https://ja-jp.facebook.com/business/help/774623835981457?&helpref=uf_permalink) カスタム質問を作成 [!DNL Facebook] します。

ただし、**Marketo は、このデータの収集を自動的に開始しません**。Marketo でカスタムフィールド値の取得を開始するには、それらのカスタムフィールドを Marketo のフィールドに&#x200B;**マッピングする必要があります**。

次に、管理の LaunchPoint 領域でこれを設定する方法を示します。

>[!NOTE]
>
>**管理者権限が必要**

1. 管理領域に移動して、**[!UICONTROL LaunchPoint]** をクリックします。「インストール済みのサービス」で、「**[!UICONTROL Facebook リード広告]**」を探して編集します。

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. 許可されたアカウントはそのままにします。**変更を加えないでください**。「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. 先ほどと同様に、選択されたページはそのままにします。**変更を加えないでください**。「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. ここで、カスタム [!DNL Facebook] フィールドをMarketo フィールドにマッピングします。 **[!UICONTROL 追加 &#x200B;].** をクリックします。

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. 新しい行に、[!DNL Facebook] のカスタムフィールドの名前を入力します。

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >ここには、フォームテンプレートに保存され [!DNL Facebook] フィールドのみがオプションとして表示されます。

1. 「**[!UICONTROL Marketo フィールド]**」列をクリックします。マッピングしたいフィールドを入力して検索します。フィールドを選択したら、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >[!DNL Facebook] フィールドをマッピングするMarketoにフィールドがまだない場合は、[ カスタムフィールドの作成 ](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) を参照してください。

>[!CAUTION]
>
>Marketoでデータを収集するには **新しい** フィールドに対してこのプロセスを実行する [!DNL Facebook] 必要があります）。
