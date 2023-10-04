---
description: Marketo サブスクリプションと Adobe Admin Console へのユーザの移行について - Marketo ドキュメント - 製品ドキュメント
title: Marketo サブスクリプションと Adobe Admin Console へのユーザの移行について
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: c871be92ce61c37e9a8d198c1b3bae6588f6a94f
workflow-type: tm+mt
source-wordcount: '1172'
ht-degree: 3%

---

# Marketo サブスクリプションと Adobe Admin Console へのユーザの移行について {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

Adobeは、Adobe Marketo Engageのサブスクリプションとユーザーの管理方法を強化し、ユーザーと組織の生産性を高めています。 この変更の一環として、Adobeは、Marketo Engageの購読とユーザーをAdobe Admin Consoleに移行中です。 これは必要な移行であり、マーケティングワークフロー、コンテンツ、統合、アセットには影響しません。

Adobe Admin Consoleを使用して、 [エンタープライズ版およびチーム版管理ガイド](https://helpx.adobe.com/enterprise/admin-guide.html){target="_blank"}.

## 変更点 {#what-is-changing}

移行の一環として、サブスクリプションとユーザー管理が、Marketoアプリケーション内からAdobe Admin Consoleに移行します。

* **システム管理者がAdobe Admin Consoleの購読を管理します**. 1 つのコンソールですべてのAdobe製品を表示できます。

* **製品管理者は、Adobe Admin Consoleでユーザーとそのアクセスを管理します**. すべてのユーザー購読のユーザーを追加および削除するAdobe。

* **ユーザーはAdobeID でサインインします**. Adobeは、既存のユーザーをAdobe Admin Consoleに移行します。 ユーザーは、Adobe IDまたはAdobeFederated ID(SSO) の新しいAdobeID を使用してMarketoサブスクリプションにログインします。

* **その他のすべての機能の管理方法に変更はありません** 機能、Marketo Engageの役割、ワークスペース、機能、動作の管理を含む、ユーザーアプリケーション自体内。


## 移行ジャーニーのタイムライン {#migration-journey-timeline}

Adobeは、まずMarketo EngageサブスクリプションをAdobe Admin Consoleに移行してから、検証済みの電子メールアドレスを持つ既存のすべてのユーザーを移行します。 システム管理者またはMarketo製品管理者の方は、移行プロセスをガイドする電子メールが届きます。 以下に、期待できるタイムラインを示します。

### 配信登録の移行が完了しました {#subscription-migration-complete}

Adobe Admin Consoleへのサブスクリプションの移行が完了すると、システム管理者に電子メールが送信されます。

システム管理者は、ユーザーの移行を開始する前に、Marketoユーザーへの影響を最小限に抑えるために、必要な手順をいくつか完了する必要がある場合があります。

* Marketoユーザーが現在 SSO でログインしている場合は、Adobe Admin Consoleで SSO を設定して、ユーザーが SSO でログインを続行できるようにする必要があります。 Marketoユーザーが現在 SSO を利用していないのにAdobe Admin Consoleで設定したい場合は、移行ジャーニーのこの時点で設定できます。

* Adobe Admin Consoleで他のAdobe製品を既に管理している場合、Adobeは、既存のコンソールにユーザーを自動的に移行する同意を求める場合があります。 電子メールの「使用を開始」ボタンをクリックして、同意ページに移動します。

現時点では、ユーザー管理に変更はありません。 Marketo管理者は、引き続きMarketo Admin 領域でユーザーを管理します。ユーザーの移行が完了するまで、Marketo ID でログインし続けます。

### ユーザー移行のスケジュール設定 {#schedule-user-migration}

前の節で説明した前提条件をシステム管理者が完了すると、Adobeは 30 日前にユーザー移行のスケジュールを自動的に設定し、Marketoの製品管理者に連絡して、ユーザー移行を管理します。

Marketo製品管理者がおこなう操作：

* 30 日前に予定されているユーザー移行開始日を記載した電子メールを受け取ります。

* Marketo Admin 領域にあるMarketo Migration Console にアクセスできます。このコンソールでは、サブスクリプションの移行日を変更することができます。

>[!NOTE]
>
>移行が複雑なので、日付の変更はスケジュールされた日付から 30 日以内に制限されます。 後日が必要な場合は、marketocares@marketo.comに電子メールを送信してください。

* My Marketoのバナーに、「User Migration Start Date」へのカウントダウンが表示されます。

* ユーザー移行開始日の前日に、リマインダーの電子メールを受け取ります。

### 移行日のユーザー準備 {#prepare-users-for-migration-day}

Marketo製品管理者は、すべてのユーザーが移行に備えて 1 日以内に準備できるようにすることをお勧めします。

* チェック [電子メールの検証](/help/marketo/product-docs/administration/users-and-roles/email-verification.md){target="_blank"} 「 Marketo Admin 」領域のすべてのユーザーのステータス。 電子メールアドレスを検証していないユーザーに対して、検証プロセスを完了する際の課題を解決するよう促します。

* AdobeID への今後の移行に備えて、すべてのユーザーを準備します。

>[!NOTE]
>
>ユーザーが移行すると、Marketoへのログイン方法の変更をAdobeから通知する電子メールが送信されます。 AdobeID を使用したログインの招待を受け入れるよう、既存のAdobe IDでサインインするか、同じ電子メールアドレスを使用して新しいログインを設定して、初めて招待されます。

>[!IMPORTANT]
>
>Marketo Engageユーザーが E メールアドレスを検証しない場合、ユーザーはAdobe IDに移行されず、サブスクリプションの移行が完了した後でMarketoサブスクリプションにアクセスできなくなります。 Marketo製品管理者がアクセスを再度取得するには、新しいユーザーとして追加する必要があります。

### 移行日に期待される事項 {#what-to-expect-on-migration-day}

ユーザーの移行は、Marketoサブスクリプションで設定されたタイムゾーンの午前 0 時に開始されます。

**Adobeが最初にMarketo管理者を自動的に移行します**. Marketo管理者がAdobeID に移行されると、Marketoアプリケーション内でAdobe製品管理者の役割と、以前の役割が割り当てられます。

**Marketoサブスクリプションのユーザー数が 75 人未満の場合**&#x200B;の場合、Adobeは残りのユーザーを自動的に移行します。 このワークフローは、最高レベルの自動化を実現し、AdobeのMarketoユーザーのオーバーヘッドを最小限に抑えることを目的としています。 移行を実行するために必要なアクションはありません。

**Marketoサブスクリプションに 75 人を超えるユーザーがいる場合**&#x200B;を使用すると、Marketo製品管理者は、Marketo Admin Area にあるMarketo Migration Console のセルフサービスユーザー移行領域にアクセスできます。 ユーザー移行プロセス中により詳細な制御を必要とするユーザーに対して、Marketo製品管理者は、一括またはすべてを一度に移行するユーザーの選択を開始できます。 ユーザーを選択すると、管理者は、後日「今すぐ移行」または「移行をスケジュール」を選択できるので、管理者は極めて柔軟に移行でき、移行時にユーザーを制御できます。

>[!NOTE]
>
>ユーザーの移行中に、製品へのアクセス権が失われることはありません。 Adobeの移行中にユーザーがログインした場合、ユーザーはログアウトされ、移行が完了した後、ユーザー ID を使用して数分以内に再度ログインするよう求められます。

ユーザーが移行されると、Marketoへのログイン方法の変更をAdobeに通知する電子メールがユーザーに届きます。 AdobeID を使用したログインの招待を受け入れるよう、既存のAdobe IDでサインインするか、同じ電子メールアドレスを使用して新しいAdobe IDを設定して、初めて招待されます。 詳細は、 [Adobeを使用したユーザーサインイン](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"} 記事。

## ユーザー移行完了 {#user-migration-complete}

Adobeは、すべての管理者とユーザーが移行されると、電子メールですべてのシステム管理者と製品管理者に通知します。 現時点では、そのサブスクリプションのすべてのMarketoユーザーはAdobeID を使用してMarketoにログインし、製品管理者はAdobe Admin Consoleでのみユーザーを管理します。

## サポートを受ける {#get-support}

サブスクリプションまたはユーザー移行に関する追加サポートについては、marketocares@marketo.comまで電子メールでお問い合わせください。
