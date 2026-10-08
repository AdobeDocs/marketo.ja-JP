---
unique-page-id: 14746177
description: Sales Connectで購読を解除した連絡先を再度購読する方法について説明します。 必要に応じて、セールスメールを受信する能力を回復する。
title: 登録解除の再登録
exl-id: 1c451ff7-c56f-477e-b287-898c359aedcf
feature: Marketo Sales Connect
TQID: 'https://experienceleague.adobe.com/W215ia0s7e6sze5shnYJyExnzeezcmMRTKrXeJDcht4'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: ab9cc269-26ac-5c58-b645-e0736aefe9f3
    internal-label: Marketo Sales Connect
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 90%
---
# [!UICONTROL 登録解除]の再登録 {#resubscribing-an-unsubscribe}

メール受信に再びオプトインしたい場合があります。 ここでは、購読解除した相手に再びメールを送信できるようにする方法を説明します。

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

1. 人物を選択して、その人物の詳細ビューを開きます。

   ![](assets/two.png)

1. ユーザーの詳細表示の 3 つの点をクリックし、「**[!UICONTROL 登録解除を削除]**」を選択します。

   ![](assets/three.png)

1. メール受信に再登録する理由を選択し、「**[!UICONTROL 登録解除を削除]**」をクリックします。

   ![](assets/four.png)

>[!NOTE]
>
>登録解除同期をオンにしている場合、Salesforce のレコードのオプトアウトボックスもオフにする必要があります。オフにしないと、夜間同期で、そのユーザが [!DNL Salesforce] でオプトアウトされていることが検出され、[!DNL Sales Connect] でそのユーザの登録が解除されます。 いずれかのレコードがオプトアウト／購読解除になっている場合、同期によりリンクされたレコードも同様にマークされます。
