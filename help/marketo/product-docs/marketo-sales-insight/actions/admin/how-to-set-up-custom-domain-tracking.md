---
description: カスタムドメイントラッキングを設定する方法 - Marketo ドキュメント - 製品ドキュメント
title: カスタムドメイントラッキングを設定する方法
hide: true
hidefromtoc: true
source-git-commit: ec78e047c9dc126553fe8a4b6a4c21b0d11aea5c
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 16%

---

# カスタムドメイントラッキングを設定する方法 {#how-to-set-up-custom-domain-tracking}

カスタムドメイントラッキングを使用すると、チームはセールスメールに追加された追跡可能なすべてのリンクで、自分の会社名を使用できます。 この設定が完了したら、メールに含まれているリンクが go.yourcompany.com と表示されるようにしま許可リストす。そのため、誰かがリンクにマウスポインターを置いたときに、go.toutapp.com ではなく go.yourcompany.com と表示されます。

go.toutapp.com を指すドメインの CNAME レコードを設定するには、IT チームのサポートが必要です。 この CNAME は、すべてのトラッキングリンク（例：go.yourcompany.com）に表示されます。

CNAME が正しく設定されていることを IT チームに確認したら、「アクション」のカスタムドメイントラッキングページに追加できます。

>[!NOTE]
>
>CNAME が適切に設定されておらず、アクションでカスタムドメインとしてアクティブ化すると、トラッキングリンクとピクセルが壊れる場合があります。

## カスタムドメイン追跡の有効化 {#enable-custom-domain-tracking}

>[!NOTE]
>
>**管理者権限が必要です。**

1. 歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. 「管理者設定」で、「 **トラッキング**.

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. 「カスタムドメイントラッキング」タブで、CNAME を入力し、「 **接続**.

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
