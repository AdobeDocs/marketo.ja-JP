---
description: 電子メールトラッキングリンクヘッダー — Marketoドキュメント — 製品ドキュメント
title: メール追跡リンクヘッダー
exl-id: 2db1f1b3-3afe-4710-a8b1-b06fbf09ec8c
source-git-commit: e9a41359a4a03f323312b61ab5afc820140b6fee
workflow-type: tm+mt
source-wordcount: '103'
ht-degree: 26%

---

# メール追跡リンクヘッダー {#email-tracking-link-headers}

以下の手順に従って、電子メールトラッキングリンクヘッダーをカスタマイズします。

1. Marketo で、「**管理者**」をクリックします。

   ![](assets/email-tracking-link-headers-1.png)

1. 「**メール**」をクリックします。

   ![](assets/email-tracking-link-headers-2.png)

1. 下にスクロールして「Custom Header Options」を表示します。 目的の設定を選択し、 **変更を保存**.

   ![](assets/email-tracking-link-headers-3.png)

<table>
 <tr>
  <td><strong>Strict-Transport-Security</strong></td>
  <td>トラッキングリンクが常に HTTPS 経由で提供されるようにするには、これを使用します（SSL で保護されたトラッキングリンクを持つ購読に対してのみ設定する必要があります）。</td>
 </tr>
</table>

>[!CAUTION]
>
>これらの設定を IT チームと確認して、組織のポリシーをどのように設定するかを決定することが重要です。設定が正しくないと、一部の訪問者が電子メールリンクにアクセスできなくなる可能性があります。
