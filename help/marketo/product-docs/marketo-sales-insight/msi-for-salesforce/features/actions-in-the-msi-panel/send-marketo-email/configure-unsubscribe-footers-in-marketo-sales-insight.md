---
unique-page-id: 2953373
description: Marketto Sales Insight - Marketto Docs — 製品ドキュメントでの登録解除フッターの設定
title: Marketor Sales Insightでの登録解除フッターの設定
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---


# Marketor Sales Insightでの登録解除フッターの設定 {#configure-unsubscribe-footers-in-marketo-sales-insight}

販売用の電子メールでは、自動的に登録解除フッターが下部に配置されます。 ただし、必要に応じて設定を調整できます。

>[!NOTE]
>
>**必要な管理者権限**

>[!NOTE]
>
>**定義**
>
>**販売用の電子メール** は、Sales Insightから送信された電子メールです。 （Marketo Outlookプラグインから送信されたものは含まれません。）

1. 「 **管理者** 」領域に移動します。

   ![](assets/one-1.png)

1. 「**Sales Insight」、「**」、「 **設定の編集**」の順にクリックします。

   ![](assets/two-1.png)

   いくつかのオプションがあります。 まず、設定を変更できる電子メールのタイプを見てみましょう。

   ![](assets/three-1.png)

   * **テンプレートなし** — 販売ユーザーが手動で作成。
   * **標準電子メール** — テンプレートに基づく電子メールです。
   * **操作上の電子メール** — 購読解除、マーケティングの一時停止、通信の制限を無視する電子メール（何があっても送信される）。

   タイプごとに異なる動作を設定するオプションがあります。

   >[!CAUTION]
   >
   >**登録解除設定を適用：**登録解除されたリードは、公開された電子メールが「運用中」であっても電子メールを受信しません
   >
   >
   >**登録解除設定を無視：** 未登録のリードがEメールを受信

   必要な変更を行い、「保存」をクリックします。

   >[!TIP]
   >
   >最後の2つの選択肢では、受信者数に応じて（「1より大きい」または「5より大きい」）、購読解除フッターを動的に含める/除外できます。

   ![](assets/four-1.png)

フー！ 少し複雑ですが、かなり柔軟ですね。

>[!NOTE]
>
>**ディープダイブ**
>
>Marketor Sales Insightの詳細 [を説明します](http://docs.marketo.com/display/docs/marketo+sales+insight)。

