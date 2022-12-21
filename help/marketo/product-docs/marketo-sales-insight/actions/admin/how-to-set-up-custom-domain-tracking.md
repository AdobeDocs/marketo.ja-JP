---
description: カスタムドメイントラッキングの設定方法 - Marketo ドキュメント - 製品ドキュメント
title: カスタムドメイントラッキングの設定方法
exl-id: 6dea7f3d-d44d-4f67-af44-a8963c95c378
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 100%

---

# カスタムドメイントラッキングの設定方法 {#how-to-set-up-custom-domain-tracking}

カスタムドメイントラッキングを使用すると、チームはセールスメールに追加されたトラック可能なすべてのリンクに、自社の名前を使用できます。この設定が完了すると、メールに含まれているリンクが許可リストに加えられ、「go.yourcompany.com」と表示されるようになります。そのため、リンクにマウスポインターを置いたときに、go.toutapp.com ではなく go.yourcompany.com と表示されます。

go.toutapp.com を指すドメインの CNAME レコードを設定するには、IT チームのサポートが必要です。この CNAME は、すべてのトラッキングリンク（例：go.yourcompany.com）に表示されます。

CNAME が正しく設定されていることを IT チームに確認したら、「アクション」のカスタムドメイントラッキングページに追加できます。

>[!NOTE]
>
>CNAME が適切に設定されておらず、アクションでカスタムドメインとしてアクティブ化すると、トラッキングリンクとピクセルが壊れる場合があります。

## クロスドメイントラッキングの有効化 {#enable-custom-domain-tracking}

>[!NOTE]
>
>**管理者権限が必要。**

1. 歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. 「管理者設定」で、「**トラッキング**」を選択します。

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. 「カスタムドメイントラッキング」タブで、CNAME を入力し、「**接続**」をクリックします。

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
