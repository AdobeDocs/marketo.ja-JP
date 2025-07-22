---
unique-page-id: 14746177
description: 登録解除の再登録 - Marketo ドキュメント - 製品ドキュメント
title: 登録解除の再登録
exl-id: 1c451ff7-c56f-477e-b287-898c359aedcf
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 62%

---

# 購読の再登録 [!UICONTROL  購読解除 ] {#resubscribing-an-unsubscribe}

メール受信に再びオプトインしたい場合があります。ここでは、登録解除したメールを再びメール可能にする方法を示します。

>[!NOTE]
>
>**管理者権限が必要**

>[!CAUTION]
>
>再登録する前に、再登録の承認がドキュメント化され、適用されるすべての法律に準拠していることを示す必要があります。

>[!NOTE]
>
>購読解除同期を有効にしている場合、ToutApp の購読解除を削除し、人物レコードのオプトアウトの [!DNL Salesforce] をオフにして、再び同期しないようにする必要があります。

1. [web アプリケーション](https://toutapp.com/login)に移動して、「**[!UICONTROL ユーザー]**」をクリックします。

1. 詳細表示を開くユーザーを選択します。

   ![](assets/two.png)

1. ユーザーの詳細表示の 3 つの点をクリックし、「**[!UICONTROL 登録解除を削除]**」を選択します。

   ![](assets/three.png)

1. メール受信に再登録する理由を選択し、「**[!UICONTROL 登録解除を削除]**」をクリックします。

   ![](assets/four.png)

>[!NOTE]
>
>購読解除同期をオンにしている場合、Salesforceのレコードのオプトアウトボックスもオフにする必要があります。オフにすると、[!DNL Sales Connect] でユーザーがオプトアウトされたことを検出するため、夜間同期によって [!DNL Salesforce] でユーザーの登録が再度解除されます。 いずれかのレコードがオプトアウト／登録解除された場合、同期により、リンクされたレコードがそのようにマークされます。
