---
unique-page-id: 4719316
description: ユーザーアカウントの使用 — Marketoドキュメント — 製品ドキュメント
title: 個人アカウントの使用
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# 個人アカウントの使用 {#using-person-accounts}

組織のニーズに合わせて、Salesforceでユーザーアカウントを設定できます。 Marketoが個人アカウントを扱う方法を次に示します。

>[!NOTE]
>
>デフォルトのSalesforceアカウントは、ビジネスアカウントです。 Salesforce管理者は、個人アカウントを個別に設定する必要があります。

## 個人アカウントとは {#what-is-a-person-account}

個人アカウントは、Salesforceのアカウントオブジェクトと非常に似ています。 ただし、個人アカウントは、アカウントフィールドと連絡先フィールドの両方にアクセスできます。

## ユーザーアカウントがMarketoに同期されるとどうなりますか？ {#what-happens-when-a-person-account-is-synced-to-marketo}

ユーザーアカウントは、会社としてMarketoに、または個人として同期されます。

>[!NOTE]
>
>個人アカウントのカスタムフィールドは、Marketoの会社と個人の両方にコピーされます。

## ビジネスアカウントと個人アカウントを区別する方法を教えてください。 {#how-do-i-differentiate-business-accounts-and-person-accounts}

スマートリストで「**個人アカウント**」フィルターを使用して、個人アカウントを標準のビジネスアカウントと区別します。

## Marketo Sales Insightの個人アカウント情報はどこに表示されますか。 {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

個人アカウントに関連するアクティビティは、**アカウント**&#x200B;パネルに表示されます。

>[!NOTE]
>
>Marketo Sales Insightの「 Marketoキャンペーンに追加&#x200B;**」と「**&#x200B;電子メールを送信&#x200B;**」の各オプションは、現在、個人のアカウントでは使用できません。**

## 個人アカウントにオポチュニティを関連付ける方法を教えてください。 {#how-do-i-associate-opportunities-to-a-person-account}

Marketoは、オポチュニティを関連付ける担当者を決定するために、オポチュニティの連絡先の役割に依存します。 商談をMarketoの適切な個人に接続するには、各個人アカウントに商談の連絡先の役割を追加する必要があります。 営業案件の連絡先の役割を自動的に追加するワークフローを設定することをお勧めします。

## 個人アカウントに使用する必要がある電子メールフィールドは何ですか？ {#which-email-field-should-i-use-for-person-accounts}

1人のユーザーアカウントに対して2つのEメールフィールドがあります。 Marketoでの重複排除や他の電子メール処理が正しく機能するよう、フォームの「**電子メールアドレス**」フィールド（**個人の電子メールアドレス**&#x200B;ではなく）を使用します。
