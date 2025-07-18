---
unique-page-id: 2360287
description: Marketo でのカスタムフィールドの作成 - Marketo ドキュメント - 製品ドキュメント
title: Marketo でのカスタムフィールドの作成
exl-id: 6face1d7-6a4e-412b-9708-6aa7e43e8c11
feature: Field Management
source-git-commit: dcc2af51726db6f503486fb0553fb32fc65495ce
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 58%

---

# Marketo でのカスタムフィールドの作成 {#create-a-custom-field-in-marketo}

データを保存または取得するために Marketo Engage で新しいカスタムフィールドが必要な場合は、以下の方法で作成します。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/create-a-custom-field-in-marketo-1.png)

1. 「**[!UICONTROL フィールド管理]**」をクリックします。

   ![](assets/create-a-custom-field-in-marketo-2.png)

   >[!TIP]
   >
   >フィールドを CRM と同期させる場合は、CRM で作成します。これらのフィールドは Marketo で自動的に作成されます。

1. 「**[!UICONTROL 新規カスタムフィールド]**」をクリックします。

   ![](assets/create-a-custom-field-in-marketo-3.png)

1. _[!UICONTROL オブジェクト]_ を選択します。

   ![](assets/create-a-custom-field-in-marketo-4.png)

   >[!NOTE]
   >
   >_会社_ オブジェクトは自分で選択できませんが、[Marketo サポート ](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} に連絡してリクエストできます。

1. フィールド _[!UICONTROL タイプ]_ を選択します。 これにより、Marketoのスマートリストおよびフォームでのレンダリング方法が変わります。

   >[!TIP]
   >
   >[カスタムフィールドタイプ用語集](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md){target="_blank"}をご覧ください。

   ![](assets/create-a-custom-field-in-marketo-5.png)

1. Marketoに表示する _[!UICONTROL 名前]_ を入力します（_[!UICONTROL API 名]_ は自動的に生成されます）。 保存後は名前を変更できないので、慎重に選択してください。 終了したら、「**[!UICONTROL 作成]**」をクリックします。

>[!CAUTION]
>
>フィールド名の先頭に、以下の文字を使用することはできません。**.&amp; +[]**

![](assets/create-a-custom-field-in-marketo-6.png)

>[!NOTE]
>
>この API 名は、SOAP API および他のバックエンドプロセスで使用されます。

これで、このカスタムフィールドをフォーム、フローステップ、スマートリストで使用できるようになります。
