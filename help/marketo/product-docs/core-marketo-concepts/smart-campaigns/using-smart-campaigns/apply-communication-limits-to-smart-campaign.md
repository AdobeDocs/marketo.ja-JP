---
unique-page-id: 1147064
description: スマートキャンペーンに通信制限を適用する方法を説明します。 ユーザーがキャンペーンを実行できるメールの数または時間の上限。
title: スマートキャンペーンへの通信制限の適用
exl-id: b33885ba-6811-47ab-9db9-099d35ca49df
feature: Smart Campaigns
source-git-commit: 3efcb529cd3e35027f35e51dfd91f95e94af9d61
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 70%

---

# スマートキャンペーンへの通信制限の適用 {#apply-communication-limits-to-smart-campaign}

>[!PREREQUISITES]
>
>[通信制限の有効化](/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md){target="_blank"}

1 日に何度もメールを送ったり、1 週間に送信するメールが多すぎたりするのは適切とは言えません。幸いにも、Marketo Engageには支援を行うためのコミュニケーションの制限があります。

>[!NOTE]
>
>任意の人が設定された通信制限を超えると、Marketo は非オペレーショナルメールをブロックします（オペレーショナルメールは常に送信されます）。

1. スマートキャンペーンで、「**[!UICONTROL スケジュール]**」タブをクリックし、「**[!UICONTROL 設定を編集]**」をクリックします。

   ![](assets/apply-communication-limits-to-smart-campaign-1.png)

1. 「**[!UICONTROL 非オペレーショナルメールをブロック]**」チェックボックスをオンにし、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/apply-communication-limits-to-smart-campaign-2.png)

>[!NOTE]
>
>制限は、条件を満たす人物のうち、スマートキャンペーンが影響を及ぼす可能性のある人数を示します。

>[!TIP]
>
>これをデフォルトにするには、「管理者」セクションで [&#x200B; 通信の制限 &#x200B;](/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md){target="_blank"} を編集します。

誤ってオーディエンスに大量のメールを送信しないようにすることができます。
