---
description: ログイン管理の設定 - Marketo ドキュメント - 製品ドキュメント
title: ログイン管理の設定
exl-id: 077f7f97-1413-4495-b2c9-94194e8dbcc2
feature: Sales Insight Actions
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 50%

---

# ログイン管理の設定 {#login-management-settings}

ログイン管理の設定を使用すると、管理者は、Sales Insight Actions のユーザに対して、グローバルレベルで認証設定を設定できます。

>[!NOTE]
>
>デフォルトでは、[!UICONTROL  つのインスタンスに対して「]0}Salesforceのみ }」オプションが選択されます。 [!DNL Sales Insight Actions]この設定は、ユーザーが [ から ](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md) 自動ログイン [!DNL Salesforce] できるようにすることをお勧めします。

## ログイン管理設定の更新 {#update-login-management-settings}

>[!NOTE]
>
>**管理者権限が必要**

ログイン管理の環境設定を更新するには、次の手順に従います。

1. 歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/login-management-settings-1.png)

1. [!UICONTROL  管理者設定 ] で **[!UICONTROL 一般]** をクリックします。

   ![](assets/login-management-settings-2.png)

1. [!UICONTROL Login Management] カードまでスクロールし、目的の設定を選択します（この例では、「Salesforceのみ」を選択しています）。 終了したら「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/login-management-settings-3.png)

## 「Salesforce のみ」についての FAQ {#salesforce-only-faq}

Salesforceのみ：[!DNL Sales Insight Actions] で [!DNL Salesforce] を使用する場合にのみ認証できます。 これは [!DNL Sales Insight Actions] インスタンスのデフォルトの選択であり、ユーザー名とパスワードを管理しなくてもシームレスに認証できるので、推奨されます。

### 「[!UICONTROL Salesforceのみ ]」が選択されている場合、インスタンスの新規ユーザーはアカウントをどのようにアクティブ化しますか？ {#activate-when-salesforce-only-is-selected}

招待メールの「**[!UICONTROL 使用を開始]**」ボタンをクリックすると、新規ユーザーはアカウントアクティベーション画面に送信され、Salesforce インスタンスに接続して [!DNL Sales Insight Actions] アカウントをアクティブ化する必要があります。

![](assets/login-management-settings-4.png)

### 「[!UICONTROL Salesforceのみ ]」が選択されている場合、ユーザーが認証できる認証方法は何ですか？ {#what-authentication-methods}

ログイン画面に移動する際、ユーザはまずメールアドレスを入力します。次に、「Salesforce ワンクリック [!UICONTROL  ログイン ]」ボタンをクリックし、ログイン中のSalesforce アカウントを使用して認証できます。

>[!NOTE]
>
>これは、ログイン画面に直接移動するユーザにのみ関係します。[!DNL Salesforce] からアクションにアクセスしているユーザーは、[ 自動ログイン ](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md) でログインします。

![](assets/login-management-settings-5.png)

### ユーザが Salesforce から Actions の機能にアクセスし、「Salesforce のみ」が選択されている場合、ユーザ認証は Actions でどのように処理されますか？ {#how-is-user-authentication-handled}

ユーザーがアクション（通話、メール、キャンペーン、タスク、キャンペーンリストなど）の 1 つをクリックすると、SFDC認証を使用して [!DNL Sales Insight Actions] アカウントに自動ログインされます。 この認証を、[自動ログイン](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md)と呼んでいます。

## 「すべてのログイン方法」に関する FAQ {#all-login-methods-faq}

### 「すべてのログイン方法」が選択されている場合、自分のインスタンスの新しいユーザは自分のアカウントをどのようにアクティブ化しますか？ {#activate-when-all-login-methods-is-selected}

新しいユーザがインスタンスに招待されると、アカウントのアクティベーションに関するメールが届きます。「開始する」というボタンをクリックすると、パスワードの作成と確認を求めるページが表示されます。作成されたアカウントはアクティブ化され、オンボーディングワークフローで使用されます。

![](assets/login-management-settings-6.png)

### 「[!UICONTROL  すべてのログイン方法」が選択されている場合、インスタンスのユーザーはど ] の方法でログインできますか？ {#what-are-users-allowed-to-log-in-with-all-login}

当社のログインページを使用する場合、ユーザはまず自分のメールアドレスを入力します。次に、すべてのログインオプション（ユーザ名／パスワード、SFDC、Gmail、SSO）を提供するページに送信されます。
