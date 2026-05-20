---
unique-page-id: 12981050
description: Marketo Sales Insightでセールステンプレートをロックする方法について説明します。 営業担当者が承認済みのバージョンを使用できるように、テンプレートの変更を防止します。
title: セールステンプレートのロック
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/PNWQ3RaspZ-Vf3LHoCqPRH3cVlV2grC8iDPo1s1sbvg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 227
ht-degree: 85%

---

# セールステンプレートのロック {#lock-sales-template}

CRM ユーザーがセールステンプレートを編集できないように、管理者はテンプレートをロックできるので、ユーザーはメールエディターでテンプレートを個別にロックできます。

>[!CAUTION]
>
>この機能は [!DNL Salesforce] でのみ機能し、[!DNL Microsoft Dynamics] やその他の CRM とは互換性がありません。 [!DNL Outlook] または Gmail プラグインからアクセスするテンプレートは、Marketo によってエディターは制御されないので、ロックされません。

## テンプレートのロックを有効にする {#enable-lock-template}

>[!NOTE]
>
>**管理者権限が必要**

1. 「**[!UICONTROL 管理者]**」に移動し、「**[!UICONTROL セールスインサイト]**」をクリックします。

   ![](assets/1.png)

1. 「**[!UICONTROL 設定]**」で、「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/2.png)

1. 「**[!UICONTROL テンプレートをロックする機能を有効化]**」をチェックします。 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>デフォルトでは、このボックスはオンになっており、テンプレートをロックする機能が有効になっています。 これをオフにすると、メールエディターのロックテンプレート機能が無効になります。

>[!NOTE]
>
>管理者がこの設定を変更しても、既存のテンプレートに遡って影響を与えることは&#x200B;**ありません**。つまり、既存のテンプレートは自動的にロックされません。

## メールエディターでテンプレートをロック {#lock-template-in-the-email-editor}

1. ロックするメールを選択し、「**[!UICONTROL ドラフトを編集]**」をクリックします。

   ![](assets/5.png)

1. メールエディターで、「**[!UICONTROL メール設定]**」をクリックします。

   ![](assets/6.png)

1. まだチェックされていない場合は、**[!UICONTROL Marketo Sales Insightへの公開]**&#x200B;を確認してください。 これで、「**[!UICONTROL CRM ユーザーにメールの編集を許可する]**」のチェックを外して、テンプレートをロックできます。 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/7.png)

   >[!NOTE]
   >
   >デフォルトでは、このボックスはオンになっており、CRM ユーザーはメールの編集が許可されています。
