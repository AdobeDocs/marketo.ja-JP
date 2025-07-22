---
description: カスタムドメイントラッキングの設定方法 - Marketo ドキュメント - 製品ドキュメント
title: カスタムドメイントラッキングの設定方法
exl-id: 6dea7f3d-d44d-4f67-af44-a8963c95c378
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 78%

---

# カスタムドメイントラッキングの設定方法 {#how-to-set-up-custom-domain-tracking}

カスタムドメイントラッキングを使用すると、チームはセールスメールに追加されたトラック可能なすべてのリンクに、自社の名前を使用できます。この設定が完了すると、メールに含まれているリンクが許可リストに加えられ、「go.yourcompany.com」と表示されるようになります。そのため、リンクにマウスポインターを置いたときに、go.toutapp.com ではなく go.yourcompany.com と表示されます。

go.toutapp.com を指すドメインの CNAME レコードを設定するには、IT チームのサポートが必要です。この CNAME は、すべてのトラッキングリンク（例：go.yourcompany.com）に表示されます。

CNAME が正しく設定されていることを IT チームに確認したら、アクションの [!UICONTROL  カスタムドメイントラッキング ] ページに追加できます。

>[!NOTE]
>
>CNAME が適切に設定されておらず、アクションでカスタムドメインとしてアクティブ化すると、トラッキングリンクとピクセルが壊れる場合があります。

## クロスドメイントラッキングの有効化 {#enable-custom-domain-tracking}

>[!NOTE]
>
>**管理者権限が必要。**

1. 歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. [!UICONTROL  管理設定 ] で、「**[!UICONTROL トラッキング]**」を選択します。

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. 「[!UICONTROL  カスタムドメイントラッキング ]」タブで、CNAME を入力し、「**[!UICONTROL 接続]**」をクリックします。

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
