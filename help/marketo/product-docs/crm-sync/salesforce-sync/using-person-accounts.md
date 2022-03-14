---
unique-page-id: 4719316
description: 個人アカウントの使用 -  Marketo ドキュメント - 製品ドキュメント
title: 個人アカウントの使用
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: ht
source-wordcount: '291'
ht-degree: 100%

---

# 個人アカウントの使用 {#using-person-accounts}

組織のニーズに合わせて、Salesforce で個人アカウントを設定できます。Marketo が個人アカウントを扱う方法を次に示します。

>[!NOTE]
>
>デフォルトの Salesforce アカウントは、ビジネスアカウントです。Salesforce 管理者は、個人アカウントを個別に設定する必要があります。

## 個人アカウントとは {#what-is-a-person-account}

個人アカウントは、Salesforce のアカウントオブジェクトと非常に似ています。ただし、個人アカウントは、アカウントフィールドと連絡先フィールドの両方にアクセスできます。

## 個人アカウントが Marketo に同期されるとどうなりますか？ {#what-happens-when-a-person-account-is-synced-to-marketo}

個人アカウントは、会社としておよび個人として Marketo に同期されます。

>[!NOTE]
>
>個人アカウントのカスタムフィールドは、Marketo の会社と個人の両方にコピーされます。

## ビジネスアカウントと個人アカウントを区別する方法を教えてください。 {#how-do-i-differentiate-business-accounts-and-person-accounts}

スマートリストで「**個人アカウント**」フィルターを使用して、個人アカウントを標準のビジネスアカウントと区別します。

## 個人アカウント情報は Marketo Sales Insight でどこに表示されますか？ {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

個人アカウントに関連するアクティビティは、**アカウント**&#x200B;パネルに表示されます。

>[!NOTE]
>
>Marketo Sales Insight の「**Marketo キャンペーンに追加**」と「**メールを送信**」の各オプションは、現在、個人アカウントでは使用できません。

## 個人アカウントに商談を関連付ける方法を教えてください。 {#how-do-i-associate-opportunities-to-a-person-account}

Marketo は、商談連絡先の役割に依存して商談を関連付ける個人を決定します。商談を Marketo の適切な個人に接続するには、各個人アカウントに商談連絡先の役割を追加する必要があります。商談連絡先の役割を自動的に追加するワークフローを設定することをお勧めします。

## 個人アカウントに使用する必要があるメールフィールドは何ですか？ {#which-email-field-should-i-use-for-person-accounts}

1 つの個人アカウントに対して 2 つのメールフィールドがあります。Marketo での重複排除や他のメール処理が正しく機能するよう、フォームの「**メールアドレス**」フィールド（**個人のメールアドレス**&#x200B;ではなく）を使用します。
