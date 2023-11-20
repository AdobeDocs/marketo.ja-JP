---
unique-page-id: 4719302
description: 英語以外のカスタムオブジェクト同期の有効化 - Marketo ドキュメント - 製品ドキュメント
title: 英語以外のカスタムオブジェクト同期の有効化
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 82%

---

# 英語以外のカスタムオブジェクト同期の有効化 {#enable-non-english-custom-object-sync}

Marketo 同期ユーザーが英語以外の言語に設定されている場合、カスタムオブジェクト同期を有効にしようとするとエラーが発生することがあります。

## エラー {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## 回避 {#getting-around-it}

1. にログインします。 [!DNL Salesforce] marketo 同期ユーザーを使用しています。

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. ユーザー名の下にある「**[!UICONTROL 設定]**」に移動します。

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. 「**[!UICONTROL 個人情報]**」で、「**[!UICONTROL 個人情報]**」をクリックします。

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. 「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. 「**[!UICONTROL 言語]**」を&#x200B;**[!UICONTROL 英語]**&#x200B;に変更します。

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. Marketo、の下に戻る **[!UICONTROL 管理者]** > **[!UICONTROL Salesforce]** > **[!UICONTROL オブジェクト]**&#x200B;をクリックし、 **[!UICONTROL スキーマを更新]**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. これにより、英語でオブジェクトリストが取り込まれます。次に、目的のオブジェクトを選択し、「**[!UICONTROL 同期を有効にする]**」をクリックします。

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. カスタムオブジェクトが有効になり、同期されます。

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. 次に、Salesforce に戻り、上記の手順を使用して、同期ユーザーを希望の言語に戻します。

>[!NOTE]
>
>オブジェクトを元の言語に戻すには、最後に、スキーマを更新するのを忘れないでください。
