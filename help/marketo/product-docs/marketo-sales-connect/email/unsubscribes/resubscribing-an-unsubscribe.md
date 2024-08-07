---
unique-page-id: 14746177
description: 登録解除の再登録 - Marketo ドキュメント - 製品ドキュメント
title: 登録解除の再登録
exl-id: 1c451ff7-c56f-477e-b287-898c359aedcf
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 100%

---

# 登録解除の再登録 {#resubscribing-an-unsubscribe}

メール受信に再びオプトインしたい場合があります。ここでは、登録解除したメールを再びメール可能にする方法を示します。

>[!NOTE]
>
>**管理者権限が必要**

>[!CAUTION]
>
>再登録する前に、再登録の承認がドキュメント化され、適用されるすべての法律に準拠していることを示す必要があります。

>[!NOTE]
>
>登録解除の同期をオンにしている場合、ToutApp から登録解除を削除し、ユーザーレコードが再び同期しないように Salesforce でオプトアウトをオフにする必要があります。

1. [web アプリケーション](https://toutapp.com/login)に移動して、「**ユーザー**」をクリックします。

1. 詳細表示を開くユーザーを選択します。

   ![](assets/two.png)

1. ユーザーの詳細表示の 3 つの点をクリックし、「**登録解除を削除**」を選択します。

   ![](assets/three.png)

1. メール受信に再登録する理由を選択し、「**登録解除を削除**」をクリックします。

   ![](assets/four.png)

>[!NOTE]
>
>登録解除同期をオンにしている場合、Salesforce のレコードのオプトアウトボックスもオフにする必要があります。オフにしないと、夜間同期で、そのユーザーが Salesforce でオプトアウトされていることが検出され、Sales Connect でそのユーザーの登録が解除されます。いずれかのレコードがオプトアウト／登録解除された場合、同期により、リンクされたレコードがそのようにマークされます。
