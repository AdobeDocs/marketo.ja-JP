---
description: ランディングページのヘッダー - Marketo ドキュメント - 製品ドキュメント
title: ランディングページのヘッダー
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
source-git-commit: a3acf82afa894160b20dff76fdd5132a234dfbd3
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 100%

---

# ランディングページのヘッダー {#landing-page-headers}

ランディングページドメインの HTTP ヘッダーの一部をカスタマイズするには、次の手順に従います。

1. Marketo で、「**管理者**」をクリックします。

   ![](assets/landing-page-headers-1.png)

1. 「**ランディングページ**」をクリックします。

   ![](assets/landing-page-headers-2.png)

1. ランディングページの HTTP ヘッダーの横の「**編集**」をクリックします。

   ![](assets/landing-page-headers-3.png)

1. 目的の設定を選択し、完了したら「**保存**」をクリックします。

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>Strict-Transport-Security</strong></td>
  <td>ランディングページへの接続が常に HTTPS 経由で提供されることを保証するには、これを使用します（SSL で保護されたランディングページを含むサブスクリプションに対してのみ設定する必要があります）。</td>
 </tr>
 <tr>
  <td><strong>X-Frame-Options</strong></td>
  <td>Marketo Engage がホストするアセットを外部の web ページに埋め込むかどうかを定義できます</td>
 </tr>
</table>

>[!CAUTION]
>
>これらの設定を IT チームと確認して、組織のポリシーをどのように設定するかを決定することが重要です。設定が正しくないと、一部の訪問者がランディングページにアクセスできなくなる可能性があります。
