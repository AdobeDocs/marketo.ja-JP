---
unique-page-id: 1147064
description: スマートキャンペーンへの通信制限の適用 - Marketo ドキュメント - 製品ドキュメント
title: スマートキャンペーンへの通信制限の適用
exl-id: b33885ba-6811-47ab-9db9-099d35ca49df
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '136'
ht-degree: 100%

---

# スマートキャンペーンへの通信制限の適用 {#apply-communication-limits-to-smart-campaign}

>[!PREREQUISITES]
>
>[通信制限の有効化](/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md)

1 日に何度もメールを送ったり、1 週間に送信するメールが多すぎたりするのは適切とは言えません。Marketo の通信制限が役立ちます。ここでは、その仕組みについて説明します。

>[!NOTE]
>
>任意の人が設定された通信制限を超えると、Marketo は非オペレーショナルメールをブロックします（オペレーショナルメールは常に送信されます）。

1. スマートキャンペーンで、「**スケジュール**」タブをクリックし、「**設定を編集**」をクリックします。

   ![](assets/programeditsettings-hands-1.png)

1. 「**非オペレーショナルメールをブロックする**」チェックボックスをオンにし、「**保存**」をクリックします。

   ![](assets/apply-communication-limits-to-smart-campaign.png)

>[!NOTE]
>
>制限は、条件を満たす人物のうち、スマートキャンペーンが影響を及ぼす可能性のある人数を示します。

>[!TIP]
>
>これをデフォルトにするには、「管理者」セクションの「[通信制限](/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md)」をクリックします。

これで完了です。誤ってオーディエンスに大量のメールを送信しすぎないようにすることができます。
