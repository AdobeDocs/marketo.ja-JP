---
unique-page-id: 2953373
description: Marketo Sales Insight の配信停止フッターの設定 - Marketo ドキュメント - 製品ドキュメント
title: Marketo Sales Insight の配信停止フッターの設定
exl-id: 16c1fcba-6826-400c-ab7c-371d8653d4ad
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 89%

---

# [!DNL Marketo Sales Insight] での購読解除フッターの設定 {#configure-unsubscribe-footers-in-marketo-sales-insight}

セールスメールでは、配信停止フッターが自動的に下部に表示されます。ただし、必要に応じて設定を調整できます。

>[!NOTE]
>
>**管理者権限が必要**

>[!NOTE]
>
>**定義**
>
>**営業メール** は、[!DNL Sales Insight] から送信されたものです（Marketo Outlook プラグインから送信されたメールは含まれません）。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/one-1.png)

1. 「**[!UICONTROL Sales Insight]**」をクリックし、「**[!UICONTROL 設定を編集]**」をクリックします。

   ![](assets/two-1.png)

   いくつかのオプションがあります。まず、設定を変更できるメールのタイプを見てみましょう。

   ![](assets/three-1.png)

   * **[!UICONTROL テンプレートなし]** - セールスユーザーが手動で作成。
   * **[!UICONTROL 標準メール]** - テンプレートに基づくメール。
   * **[!UICONTROL オペレーショナルメール]** - 配信停止、マーケティングの中断、通信制限を無視するメール（何があっても送信されます）

   タイプごとに異なる動作を設定するオプションがあります。

   >[!CAUTION]
   >
   >**[!UICONTROL 配信停止設定を優先]**：配信停止済みのリードは、公開されたメールが「オペレーショナル」の場合でもメールを受信しません
   >
   >**[!UICONTROL 配信停止設定を無視]**：配信停止済みのリードはメールを受信します

1. 必要な変更を行い、「**[!UICONTROL 保存]**」をクリックします。

   >[!TIP]
   >
   >最後の 2 つの選択肢を使用すると、受信者の数（「1 より大きい」または「5 より大きい」）に応じて、配信停止フッターを動的に含めたり除外したりできます。

   ![](assets/four-1.png)

お疲れさまでした。少し複雑ですが柔軟ですね。
