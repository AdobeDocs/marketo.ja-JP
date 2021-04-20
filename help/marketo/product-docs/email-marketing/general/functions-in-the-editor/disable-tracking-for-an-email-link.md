---
unique-page-id: 1900579
description: 電子メールリンクの追跡の無効化 —Marketoドキュメント — 製品ドキュメント
title: 電子メールリンクの追跡の無効化
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# 電子メールリンクの追跡を無効にする{#disable-tracking-for-an-email-link}

電子メール内のリンクで&#x200B;**MarketoトラッキングURL**&#x200B;を有効にしたくない場合があります。 これは、リンク先ページがURLパラメーターをサポートしていないため、リンクが壊れる場合に役立ちます。

1. 電子メールを選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/one-7.png)

1. リンクを含む編集可能なセクションを重複キーを押しながらクリックします。

   ![](assets/two-6.png)

1. 該当するリンクをクリックし、「**リンクを挿入/編集**」ボタンをクリックします。

   ![](assets/three-6.png)

1. リンクを編集ポップアップで、「**リンクを追跡**」チェックボックスをオフにします。

   ![](assets/four-4.png)

1. **「mkt_tokを含める」ボックス**&#x200B;が消えているのがわかります。 「**適用**」をクリックします。

   ![](assets/five-3.png)

   >[!TIP]
   >
   >**Include mkt_tok**&#x200B;をオフにしてもリンクは追跡できますが、リダイレクト後はリンク先URLにmkt_tokクエリ文字列パラメータは含まれません。 このパラメーターは、個人アクティビティの適切な追跡（例えば、人が電子メールから登録解除した場合）を確実に行うために、MarketoランディングページおよびMunchkinで使用されます。 パラメーターの存在が原因でWebサイト上で奇妙な動作が見られない限り、この機能の使用は避けてください。

1. 「**保存**」をクリックします。

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >電子メール&#x200B;**テンプレート**内のリンクのクリック追跡を無効にしますか？ 次の形式を使用します。
   >`<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`\
   >この導入に関するヘルプが必要な場合は、Web開発者にお問い合わせください。

ナイス！ リンクの追跡を無効にしています。
