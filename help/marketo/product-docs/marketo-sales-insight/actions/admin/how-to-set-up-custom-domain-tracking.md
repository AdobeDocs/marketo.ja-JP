---
description: トラッキング可能なリンクが企業ドメインを使用するようにカスタムドメイントラッキングを設定する方法について説明します。
title: カスタムドメイントラッキングの設定方法
exl-id: 6dea7f3d-d44d-4f67-af44-a8963c95c378
feature: Sales Insight Actions
TQID: 'https://experienceleague.adobe.com/gn3uC4uxpwp35IVYcUs-cZJFqbmPc-7vTmgbIPm8lTk'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: 412786a7-b8da-5b9d-8c3f-2539a3faad9f
    internal-label: Sales Insight Actions
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 92%
---
# カスタムドメイントラッキングの設定方法 {#how-to-set-up-custom-domain-tracking}

カスタムドメイントラッキングを使用すると、チームでセールスメールに追加されたすべてのトラッキング可能なリンクに自社の会社名を使用できます。 この設定が完了すると、メールに含まれているリンクが許可リストに加えられ、「go.yourcompany.com」と表示されるようになります。そのため、リンクにマウスポインターを置いたときに、go.toutapp.com ではなく go.yourcompany.com と表示されます。

go.toutapp.com を指すドメインの CNAME レコードを設定するには、IT チームのサポートが必要です。 この CNAME は、すべてのトラッキングリンク（例：go.yourcompany.com）に表示されます。

CNAME が正しく設定されていることを IT チームに確認したら、「アクション」の[!UICONTROL カスタムドメイントラッキング]ページに追加できます。

>[!NOTE]
>
>CNAME が適切に設定されておらず、アクションでカスタムドメインとしてアクティブ化すると、トラッキングリンクとピクセルが壊れる場合があります。

## カスタムドメイントラッキングの有効化 {#enable-custom-domain-tracking}

>[!NOTE]
>
>**管理者権限が必要。**

1. 歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. 「[!UICONTROL 管理者設定]」で、「**[!UICONTROL トラッキング]**」を選択します。

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. 「[!UICONTROL カスタムドメイントラッキング]」タブで、CNAME を入力し、「**[!UICONTROL 接続]**」をクリックします。

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
