---
unique-page-id: 2360287
description: Marketo でのカスタムフィールドの作成 - Marketo ドキュメント - 製品ドキュメント
title: Marketo でのカスタムフィールドの作成
exl-id: 6face1d7-6a4e-412b-9708-6aa7e43e8c11
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '168'
ht-degree: 100%

---

# Marketo でのカスタムフィールドの作成 {#create-a-custom-field-in-marketo}

データを保存または取得するために Marketo で新しいカスタムフィールドが必要な場合は、次の方法で作成します。

1. 「管理者」に移動し、「**フィールド管理**」をクリックします。

   ![](assets/image2014-9-24-13-3a46-3a26.png)

   >[!TIP]
   >
   >フィールドを CRM と同期させる場合は、CRM で作成します。これらのフィールドは Marketo で自動的に作成されます。

1. 「**新規カスタムフィールド**」をクリックします。

   ![](assets/two.png)

1. 「タイプ」フィールドを選択します。これにより、Marketo のスマートリストおよびフォームでのレンダリング方法が変更されます。

   >[!TIP]
   >
   >[カスタムフィールドタイプ用語集](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md)をご覧ください。

   ![](assets/image2014-9-24-13-3a47-3a42.png)

1. Marketo に表示する名前を入力します。API 名は自動的に生成されます。調整は可能ですが、一度設定すると名前を変更することはできません。終了したら、「**作成**」をクリックします。

>[!CAUTION]
>
>フィールド名の先頭に次の文字を使用することはできません。**.&amp; +[]**

![](assets/image2014-9-24-13-3a48-3a26.png)

>[!NOTE]
>
>この API 名は、SOAP API および他のバックエンドプロセスで使用されます。

これで、フォーム、フローステップ、スマートリストでこのカスタムフィールドを使用できます。
