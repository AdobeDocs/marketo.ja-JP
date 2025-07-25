---
unique-page-id: 4719316
description: 個人取引先の使用 -  Marketo ドキュメント - 製品ドキュメント
title: 個人取引先の使用
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 82%

---

# 個人取引先の使用 {#using-person-accounts}

組織のニーズに合わせて、Salesforce で個人取引先を設定できます。Marketo Engageでの人物アカウントの扱い方を次に示します。

>[!NOTE]
>
>デフォルトの [!DNL Salesforce] アカウントはビジネスアカウントです。 [!DNL Salesforce] 管理者は、個別にユーザーアカウントを設定する必要があります。

## 個人取引先とは {#what-is-a-person-account}

人物アカウントは、[!DNL Salesforce] のアカウントオブジェクトに非常に似ています。 ただし、個人取引先は、アカウントフィールドと連絡先フィールドの両方にアクセスできます。

## 個人取引先が Marketo に同期されるとどうなりますか？ {#what-happens-when-a-person-account-is-synced-to-marketo}

個人取引先は、会社としておよび個人として Marketo に同期されます。

>[!NOTE]
>
>個人取引先のカスタムフィールドは、Marketo の会社と個人の両方にコピーされます。

## ビジネスアカウントと個人取引先を区別する方法を教えてください。 {#how-do-i-differentiate-business-accounts-and-person-accounts}

スマートリストの「ユーザーアカウント」フィルターを使用して、標準のビジネスアカウントからユーザーアカウントを分離します。

## 個人取引先情報は Marketo Sales Insight でどこに表示されますか？ {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

個人取引先に関連するアクティビティは、**[!UICONTROL アカウント]**&#x200B;パネルに表示されます。

>[!NOTE]
>
>Marketo Sales Insight の「**[!UICONTROL Marketo キャンペーンに追加]**」と「**[!UICONTROL メールを送信]**」の各オプションは、現在、個人取引先では使用できません。

## 個人取引先に商談を関連付ける方法を教えてください。 {#how-do-i-associate-opportunities-to-a-person-account}

Marketo は、商談連絡先の役割に依存して商談を関連付ける個人を決定します。商談を Marketo の適切な個人に接続するには、各個人取引先に商談連絡先の役割を追加する必要があります。商談連絡先の役割を自動的に追加するワークフローを設定することをお勧めします。

## 個人取引先に使用する必要があるメールフィールドは何ですか？ {#which-email-field-should-i-use-for-person-accounts}

1 つの個人取引先に対して 2 つのメールフィールドがあります。Marketo での重複排除や他のメール処理が正しく機能するよう、フォームの「**[!UICONTROL メールアドレス]**」フィールド（**[!UICONTROL 個人のメールアドレス]**&#x200B;ではなく）を使用します。
