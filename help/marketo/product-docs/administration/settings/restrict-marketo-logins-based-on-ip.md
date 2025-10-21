---
unique-page-id: 2360297
description: IP に基づく Marketo ログインの制限 - Marketo ドキュメント - 製品ドキュメント
title: IP に基づく Marketo ログインの制限
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: 3595cdc76a0f92da10dc5ddaac64c4cf83056e88
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 60%

---

# IP に基づく Marketo ログインの制限 {#restrict-marketo-logins-based-on-ip}

IP アドレスに基づいて、ユーザの Marketo へのアクセスを制限または有効にできます。手順は次のとおりです。

>[!NOTE]
>
>**管理者権限が必要**

>[!IMPORTANT]
>
>Adobe Admin Console（AAC）は、[IP ベースのアクセス制御 &#x200B;](https://helpx.adobe.com/enterprise/using/ip-based-access.html){target="_blank"} をサポートしています。 スムーズな移行を確実に行うために、この機能が有効になっている場合は、2026 年第 1 四半期まで、Adobe ID ユーザーを含む既存のMarketo Engage IP 制限が有効になります。
>
>* AAC IP ベースのアクセスはいつでも設定できます。
>* AAC とMarketo Engageの両方の制限を同時に実行できます。 互換性のために同じ IP 許可リストを使用します。
>
>2026 年第 1 四半期以降、Marketo Engageの IP 制限は廃止されます。 IP ベースのアクセスは AAC でのみ管理され、ログイン制限を適用するように設定する必要があります。 最終移行日は後日発表されます。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. 「**[!UICONTROL ログイン設定]**」をクリックします。

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. 「**[!UICONTROL IP 制限を編集]**」をクリックします。

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. 特定のアドレスを「**許可**」するまたは「**ブロック**」するかを選択し、「**[!UICONTROL 保存]**」をクリックします。

   >[!NOTE]
   >
   >**定義**
   >
   >* **[!UICONTROL 許可済み IP アドレス]**：許可済み IP アドレスの追加は包含的です。指定したすべての IP アドレスが含まれ、その他すべてが除外されます。
   >* **[!UICONTROL ブロック済み IP アドレス]**：特定の IP が Marketo にアクセスするのを防ぎます。
   >* **[!UICONTROL IP 制限の無効化]**：これをオンにすると、すべての制限ルールが機能を停止します。これはテスト目的で使用します。

   >[!NOTE]
   >
   >複数の制限を追加できますが、すべて許可されるか、すべてブロックされるかのいずれかとなります。許可済みとブロック済みを混在させて適合させることはできません。

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)
