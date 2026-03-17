---
unique-page-id: 14746177
description: Sales Connect のサブスクリプションを解除した連絡先を再登録する方法について説明します。 必要に応じて、販売メールを受信する機能を復元します。
title: 登録解除の再登録
exl-id: 1c451ff7-c56f-477e-b287-898c359aedcf
feature: Marketo Sales Connect
source-git-commit: 15427eacd2fc42a02f6a4c59d9102bacba02e57b
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 90%

---

# [!UICONTROL 登録解除]の再登録 {#resubscribing-an-unsubscribe}

メール受信に再びオプトインしたい場合があります。ここでは、登録解除したメールを再びメール可能にする方法を示します。

>[!NOTE]
>
>**管理者権限が必要**

>[!CAUTION]
>
>再登録する前に、再登録の承認がドキュメント化され、適用されるすべての法律に準拠していることを示す必要があります。

>[!NOTE]
>
>登録解除の同期をオンにしている場合、ToutApp から登録解除を削除し、ユーザレコードが再び同期しないように [!DNL Salesforce] でオプトアウトをオフにする必要があります。

1. [web アプリケーション](https://toutapp.com/login)に移動して、「**[!UICONTROL ユーザー]**」をクリックします。

1. 詳細表示を開くユーザーを選択します。

   ![](assets/two.png)

1. ユーザーの詳細表示の 3 つの点をクリックし、「**[!UICONTROL 登録解除を削除]**」を選択します。

   ![](assets/three.png)

1. メール受信に再登録する理由を選択し、「**[!UICONTROL 登録解除を削除]**」をクリックします。

   ![](assets/four.png)

>[!NOTE]
>
>登録解除同期をオンにしている場合、Salesforce のレコードのオプトアウトボックスもオフにする必要があります。オフにしないと、夜間同期で、そのユーザが [!DNL Salesforce] でオプトアウトされていることが検出され、[!DNL Sales Connect] でそのユーザの登録が解除されます。いずれかのレコードがオプトアウト／登録解除された場合、同期により、リンクされたレコードがそのようにマークされます。
