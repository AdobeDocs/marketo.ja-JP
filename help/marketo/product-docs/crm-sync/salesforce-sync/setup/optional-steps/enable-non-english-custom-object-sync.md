---
unique-page-id: 4719302
description: 英語以外のカスタムオブジェクト同期の有効化 - Marketo ドキュメント - 製品ドキュメント
title: 英語以外のカスタムオブジェクト同期の有効化
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 70%

---

# 英語以外のカスタムオブジェクト同期の有効化 {#enable-non-english-custom-object-sync}

Marketo 同期ユーザーが英語以外の言語に設定されている場合、カスタムオブジェクト同期を有効にしようとするとエラーが発生することがあります。

## エラー {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## 回避 {#getting-around-it}

1. Marketo 同期ユーザーを使用して [!DNL Salesforce] にログインします。

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

1. Marketoに戻り、{ 管理者 **[!UICONTROL /]** 2}Salesforce **[!UICONTROL /]** オブジェクト **[!UICONTROL の下の]** スキーマを更新 **[!UICONTROL をクリックします。]**

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. これにより、英語でオブジェクトリストが取り込まれます。次に、目的のオブジェクトを選択し、「**[!UICONTROL 同期を有効にする]**」をクリックします。

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. カスタムオブジェクトが有効になり同期中であることを確認します。

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. 次に、[!DNL Salesforce] に戻り、上記の手順を使用して同期ユーザーを優先言語に戻します。

>[!NOTE]
>
>オブジェクトを元の言語に戻すには、最後に、スキーマを更新するのを忘れないでください。
