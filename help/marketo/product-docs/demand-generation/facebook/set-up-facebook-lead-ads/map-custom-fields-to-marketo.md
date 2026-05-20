---
unique-page-id: 12983101
description: Facebook リード広告のカスタムフィールドをMarketoにマッピングする方法について説明します。 Marketoの適切な人物フィールドに、リードとデータがマッピングされていることを確認します。
title: カスタムフィールドの Marketo へのマッピング
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
feature: Integrations
TQID: https://experienceleague.adobe.com/whJl1biZjBUAZp0w3kkmM5AplWTDXcV3-2KayHmsMnE
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 266
ht-degree: 71%

---

# カスタムフィールドの Marketo へのマッピング {#map-custom-fields-to-marketo}

オンライン配信サービスの利用頻度など、[!DNL Facebook] がデフォルトで保存する標準的な情報よりも多くの情報を収集したい場合があります。 これは、[!DNL Facebook] リード広告で[カスタムの質問を作成](https://ja-jp.facebook.com/business/help/774623835981457?&helpref=uf_permalink)することで実現できます。

ただし、**Marketo は、このデータの収集を自動的に開始しません**。 Marketo でカスタムフィールド値の取得を開始するには、それらのカスタムフィールドを Marketo のフィールドに&#x200B;**マッピングする必要があります**。

AdminのLaunchPoint エリアで設定するには、次の手順に従います。

>[!NOTE]
>
>**管理者権限が必要**

1. 管理領域に移動して、**[!UICONTROL LaunchPoint]** をクリックします。 「インストール済みのサービス」で、「**[!UICONTROL Facebook リード広告]**」を探して編集します。

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. 承認済みアカウントをそのままにしておきます。**は**&#x200B;に変更を加えません。 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. 以前と同様に、選択したページをそのまま残し、**は**&#x200B;変更を行いません。 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. カスタム [!DNL Facebook] フィールドをMarketo フィールドにマッピングします。 「**[!UICONTROL 追加]」をクリックします。**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. 新しい行に、[!DNL Facebook] カスタムフィールドの名前を入力します。

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >ここには、[!DNL Facebook] のフォームテンプレートに保存されたフィールドのみがオプションとして表示されます。

1. 「**[!UICONTROL Marketo フィールド]**」列をクリックします。 マッピングしたいフィールドを入力して検索します。 フィールドを選択したら、**[!UICONTROL 保存]**&#x200B;をクリックします。

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >[!DNL Facebook] フィールドのマッピング先のフィールドが Marketo にまだない場合は、[カスタムフィールドを作成](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)する方法を参照してください。

>[!CAUTION]
>
>Marketo でデータを収集するには、新しい [!DNL Facebook] フィールドに対してこの処理を実行する&#x200B;**必要があります**。
