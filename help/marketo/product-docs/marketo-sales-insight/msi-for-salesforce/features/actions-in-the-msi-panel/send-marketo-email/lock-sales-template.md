---
unique-page-id: 12981050
description: セールステンプレートのロック - Marketo ドキュメント - 製品ドキュメント
title: セールステンプレートのロック
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 84%

---

# セールステンプレートのロック {#lock-sales-template}

CRM ユーザーがセールステンプレートを編集できないように、管理者はテンプレートをロックできるので、ユーザーはメールエディターでテンプレートを個別にロックできます。

>[!CAUTION]
>
>この機能は [!DNL Salesforce] でのみ機能し、[!DNL Microsoft Dynamics] または他の CRM とは互換性がありません。 エディターはMarketoで制御されないので、[!DNL Outlook] または Gmail プラグインからアクセスするテンプレートはロックされません。

## テンプレートのロックを有効にする {#enable-lock-template}

>[!NOTE]
>
>**管理者権限が必要**

1. 「**[!UICONTROL 管理者]**」に移動し、「**[!UICONTROL Sales Insight]**」をクリックします。

   ![](assets/1.png)

1. 「**[!UICONTROL 設定]**」で、「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/2.png)

1. 「**[!UICONTROL テンプレートをロックする機能を有効化]**」をチェックします。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>デフォルトでは、このボックスはオンになっており、テンプレートをロックする機能が有効になっています。これをオフにすると、メールエディターのロックテンプレート機能が無効になります。

>[!NOTE]
>
>管理者がこの設定を変更しても、既存のテンプレートに遡って影響を与えることは&#x200B;**ありません**。つまり、既存のテンプレートは自動的にロックされません。

## メールエディターでテンプレートをロック {#lock-template-in-the-email-editor}

1. ロックするメールを選択し、「**[!UICONTROL ドラフトを編集]**」をクリックします。

   ![](assets/5.png)

1. メールエディターで、「**[!UICONTROL メール設定]**」をクリックします。

   ![](assets/6.png)

1. まだチェックされていない場合は、「**[!UICONTROL Marketo Sales Insight に公開]**」にチェックを入れます。これで、「**[!UICONTROL CRM ユーザーにメールの編集を許可する]**」のチェックを外して、テンプレートをロックできます。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/7.png)

   >[!NOTE]
   >
   >デフォルトでは、このボックスはオンになっており、CRM ユーザーはメールの編集が許可されています。
