---
unique-page-id: 2360287
description: Marketo Engageで新しいカスタムフィールドを作成し、個人または企業向けのデータを保存して取り込む手順。
title: Marketo でのカスタムフィールドの作成
exl-id: 6face1d7-6a4e-412b-9708-6aa7e43e8c11
feature: Field Management
TQID: https://experienceleague.adobe.com/xdG07VzIcNYcqCsR3wfXHTGE07nsLYAvbM8QZZJf0oo
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 203
ht-degree: 65%

---

# Marketo でのカスタムフィールドの作成 {#create-a-custom-field-in-marketo}

Marketo Engageでカスタムフィールドを作成して、データを保存および取り込む方法について説明します。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/create-a-custom-field-in-marketo-1.png)

1. 「**[!UICONTROL フィールド管理]**」をクリックします。

   ![](assets/create-a-custom-field-in-marketo-2.png)

   >[!TIP]
   >
   >フィールドを CRM と同期させる場合は、CRM で作成します。これらのフィールドは Marketo で自動的に作成されます。

1. 「**[!UICONTROL 新規カスタムフィールド]**」をクリックします。

   ![](assets/create-a-custom-field-in-marketo-3.png)

1. 「_[!UICONTROL オブジェクト]_」を選択します。

   ![](assets/create-a-custom-field-in-marketo-4.png)

   >[!NOTE]
   >
   >_会社_&#x200B;オブジェクトは自分で選択できませんが、[Marketo サポート](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}に連絡してリクエストできます。

1. 「_[!UICONTROL タイプ]_」フィールドを選択します。 これにより、Marketoのスマートリストおよびフォームでのレンダリング方法が変更されます。

   >[!TIP]
   >
   >[カスタムフィールドタイプ用語集](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md){target="_blank"}をご覧ください。

   ![](assets/create-a-custom-field-in-marketo-5.png)

1. Marketo に表示する&#x200B;_[!UICONTROL 名前]_&#x200B;を入力します（_[!UICONTROL API 名]_&#x200B;は自動的に生成されます）。 保存後は名前を変更できないので、慎重に選択します。 終了したら、「**[!UICONTROL 作成]**」をクリックします。

>[!CAUTION]
>
>フィールド名は次の文字で始めることはできません：**。 &amp; +[]**

![](assets/create-a-custom-field-in-marketo-6.png)

>[!NOTE]
>
>この API 名は、SOAP API および他のバックエンドプロセスで使用されます。

このカスタムフィールドを、フォーム、フローステップ、スマートリストで使用できるようになりました。
