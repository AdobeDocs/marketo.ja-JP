---
description: ブロックされたドメインまたは許可されたドメインを使用してDynamic Chat セキュリティを設定する方法について説明します。 担当者に表示されるメールドメインと、チャットスクリプトを使用できるサイトを制限します。
title: セキュリティ設定
feature: Dynamic Chat
exl-id: 68a53986-6f42-4aa2-86f6-0b2097f94963
TQID: https://experienceleague.adobe.com/7ans6J5WCXbTalK7ubMCrWBLWaJm3prPCoxsrCWEKtg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 88949407423d12a95bf39470e3c29835d934e2f6
workflow-type: tm+mt
source-wordcount: 238
ht-degree: 3%

---

# セキュリティ設定 {#security-settings}

セキュリティ設定では、ブロックまたは許可リストにドメインを追加できます。

![](assets/security-settings-1.png)

>[!IMPORTANT]
>
>「電子メールドメインをブロックおよび許可」フィルターは、訪問者がDynamic Chat内で直接、チャットボットまたは会話フローで電子メールアドレスを入力した場合にのみ適用されます。 Marketo Engageなどの統合製品からDynamic Chatが受け取るメールアドレスには適用されません。 詳しくは、以下の表を参照してください。

| シナリオ | フィルタリングは適用されますか？ |
|---|---|
| 訪問者はメールを直接Dynamic Chatのチャットボットに入力します | はい |
| 訪問者はメールをDynamic Chatの会話フローに直接入力します | はい |
| メールは、Marketo フォーム送信から事前入力されます（フォーム入力後に会話フローが表示されます） | いいえ |
| メールは、他の統合システムからDynamic Chatに渡されます | いいえ |

## ブロックされたメールドメイン {#blocked-email-domains}

担当者に電子メールドメインを使用させたくない訪問者（競合他社など）がある場合は、電子メールドメインをメールブロックリストに追加します。

1. 「**検証を有効にする**」スライダーを選択して、{}ブロックリストに加えるを有効にします。 最大50 ドメインを入力し、**保存**&#x200B;をクリックします。

   ![](assets/security-settings-2.png)

## 許可ドメイン {#allowed-domains}

許可されたドメインを追加すると、サードパーティがサイトからJavaScriptをスクレイピングして独自に追加できないようにします。

1. 「**検証を有効にする**」スライダーを選択して、{}許可リストに加えるを有効にします。 許可されたドメインを入力し、**保存**&#x200B;をクリックします。

   ![](assets/security-settings-3.png)
