---
unique-page-id: 2360287
description: Marketo-Marketoドキュメント — 製品ドキュメントでのカスタムフィールドの作成
title: Marketoでカスタムフィールドを作成
exl-id: 6face1d7-6a4e-412b-9708-6aa7e43e8c11
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# Marketoでのカスタムフィールドの作成{#create-a-custom-field-in-marketo}

データを保存/取り込むためにMarketoに新しいカスタムフィールドが必要な場合は、次の方法で作成します。

1. 管理者に移動し、**フィールド管理**&#x200B;をクリックします。

   ![](assets/image2014-9-24-13-3a46-3a26.png)

   >[!TIP]
   >
   >CRMと同期させるフィールドは、CRMで作成すると、自動的にMarketoで作成されます。

1. 「**新しいカスタムフィールド**」をクリックします。

   ![](assets/two.png)

1. フィールドの種類を選択します。 これは、Marketoのスマートリストやフォームでのレンダリング方法を変更します。

   >[!TIP]
   >
   >[カスタムフィールドタイプ用語集](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md)をご覧ください。

   ![](assets/image2014-9-24-13-3a47-3a42.png)

1. Marketoで表示する名前を入力します。 API名は自動的に生成されます。 ツイークは可能ですが、一度設定すると名前を変更することはできません。 完了したら「**作成**」をクリックします。

>[!CAUTION]
>
>フィールド名に次の文字を開始することはできません。**. &amp; +[]**

![](assets/image2014-9-24-13-3a48-3a26.png)

>[!NOTE]
>
>API名は、SOAP APIおよび他のバックエンドプロセスで使用されます。

フォーム、フローステップ、スマートリストでこのカスタムフィールドを使用できるようになりました。
