---
description: Strict-Transport-SecurityやX-Frame-Optionsを含むランディングページドメインのHTTP ヘッダーをカスタマイズする方法。
title: ランディングページのヘッダー
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
feature: Administration, Landing Pages
TQID: https://experienceleague.adobe.com/ecRuR4V-YCsesHZpm9UrP1rPlOjBCediq-9DtXZRfBo
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 147
ht-degree: 61%

---

# ランディングページのヘッダー {#landing-page-headers}

ランディングページドメインの HTTP ヘッダーの一部をカスタマイズするには、以下の手順に従います。

1. Marketo で、「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/landing-page-headers-1.png)

1. 「**[!UICONTROL ランディングページ]**」をクリックします。

   ![](assets/landing-page-headers-2.png)

1. ランディングページの HTTP ヘッダーの横の「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/landing-page-headers-3.png)

1. 目的の設定を選択し、完了したら「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>[!UICONTROL Strict-Transport-Security]</strong></td>
  <td>ランディングページへの接続が常に HTTPS 経由で提供されることを保証するには、これを使用します（SSL で保護されたランディングページを含むサブスクリプションに対してのみ設定する必要があります）。</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL X-Frame-Options]</strong></td>
  <td>Marketo Engageでホストされているアセットを外部web ページに埋め込めるかどうかを定義できます</td>
 </tr>
</table>

>[!CAUTION]
>
>これらの設定をIT部門と確認して、組織のポリシーを決定することが重要です。 設定が正しくないと、一部の訪問者がランディングページにアクセスできなくなる可能性があります。
