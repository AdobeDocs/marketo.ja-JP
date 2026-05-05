---
description: HTTPS向けの厳格なトランスポートセキュリティを含む、メールの下の管理者のメールトラッキングリンクヘッダーをIT レビューガイダンスを使用してカスタマイズする方法。
title: メールトラッキングリンクのヘッダー
exl-id: 2db1f1b3-3afe-4710-a8b1-b06fbf09ec8c
feature: Administration
source-git-commit: c06481152e88b8760a4539842a91aea90ab07fa1
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 64%

---

# メールトラッキングリンクのヘッダー {#email-tracking-link-headers}

以下の手順に従って、メールトラッキングリンクのヘッダーをカスタマイズします。

1. Marketo で、「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/email-tracking-link-headers-1.png)

1. 「**[!UICONTROL メール]**」をクリックします。

   ![](assets/email-tracking-link-headers-2.png)

1. 下にスクロールして「カスタムヘッダーオプション」を表示します。 目的の設定を選択し、完了したら「**[!UICONTROL 変更を保存]**」をクリックします。

   ![](assets/email-tracking-link-headers-3.png)

<table>
 <tr>
  <td><strong>Strict-Transport-Security</strong></td>
  <td>トラッキングリンクが常に HTTPS 経由で提供されることを保証するには、これを使用します（SSL で保護されたトラッキングリンクを含むサブスクリプションに対してのみ設定する必要があります）。</td>
 </tr>
</table>

>[!CAUTION]
>
>これらの設定をIT部門と確認して、組織のポリシーを決定することが重要です。 設定が正しくないと、一部の訪問者がメールリンクにアクセスできなくなる可能性があります。
