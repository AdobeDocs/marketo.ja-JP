---
unique-page-id: 4720215
description: wordpress への rtp の実装を含め、Marketo Engageの wordpress enterprise への rtp の実装について説明します。 このガイドを使用して、次の手順を完了します。
title: Wordpress Enterprise での RTP の実装
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
source-git-commit: 50befbf7339cd7a8b25b0942515497f6acc8f9ab
workflow-type: tm+mt
source-wordcount: '120'
ht-degree: 80%

---

# Wordpress Enterprise での RTP の実装 {#implementing-rtp-on-wordpress-enterprise}

[!UICONTROL RTP タグ]を実装するには、次のインストール手順に従います。

1. 「**[!UICONTROL アカウント設定]**」に移動します。

   a サポートから既に JavaScript タグを受け取っている場合は、手順 3 に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. 「[!UICONTROL ドメイン]」で、該当するドメインを選択し、「**[!UICONTROL タグを生成]**」をクリックします。

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. RTP JavaScript タグをコピーします。

1. [!DNL WordPress] アカウントに管理者ユーザとしてログインします。

   a. **[!UICONTROL 表示方法]**&#x200B;の下にある「**[!UICONTROL カスタム JavaScript]**」に移動します。b. RTP JavaScript タグを既存のコードの直後にペーストします。

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >コードをペーストすると、次のタグが除外されます。
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`
   >
   >スクリプト自体のみを挿入します。

1. 「**[!UICONTROL 更新]**」をクリックします。
