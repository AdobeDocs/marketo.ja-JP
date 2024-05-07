---
description: Marketo サブスクリプションと Adobe Admin Console へのユーザの移行について - Marketo ドキュメント - 製品ドキュメント
title: Marketo サブスクリプションと Adobe Admin Console へのユーザの移行について
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: 04544aacaf1eeec4ee60d0c09cae87ad591a1c9c
workflow-type: ht
source-wordcount: '1370'
ht-degree: 100%

---

# Marketo サブスクリプションと Adobe Admin Console へのユーザの移行について {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

アドビでは、Adobe Marketo Engage のサブスクリプションとユーザの管理方法を強化し、ユーザと組織の生産性向上を実現しています。この変更の一環として、アドビは Marketo Engage のサブスクリプションとユーザを Adobe Admin Console に移行中です。この移行は必須であり、マーケティングワークフロー、コンテンツ、統合、アセットには影響しません。

>[!TIP]
>
>Adobe Admin Console を使用して組織全体のアドビ資格を管理する方法については、[エンタープライズ版およびチーム版の管理者ガイド](https://helpx.adobe.com/jp/enterprise/admin-guide.html){target="_blank"}を参照してください。

## 変更点 {#what-is-changing}

移行の一環として、Marketo アプリケーション内のサブスクリプションとユーザ管理が、Adobe Admin Console に移行します。

* **システム管理者が Adobe Admin Console でサブスクリプションを管理します**。1 つのコンソールですべてのアドビ製品を確認できます。

* **製品管理者が Adobe Admin Console でユーザとそのアクセスを管理します**。すべてのアドビサブスクリプションのユーザを追加および削除します。Adobe Admin Console は、ユーザベースのアクセス有効期限をサポートしていません。移行後に期限切れになる予定の Marketo Engage アクセス権を持つユーザも移行され、無期限のアクセス権が付与されます。移行後は、目的の有効期限日に（またはその日付前に）手動で削除する必要があります。

* **ユーザは Adobe ID でログインします**。アドビでは、既存のユーザを Adobe Admin Console に移行します。ユーザは、新しい Adobe ID（Adobe ID または Adobe Federated ID（SSO）のいずれか）を使用して、Marketo サブスクリプションにログインします。

## 変更されていない点 {#what-is-not-changing}

* Marketo Engage アプリケーション自体では、**それ以外のすべての機能の管理方法に変更はありません**（ユーザロール、ワークスペース、動作の管理など）。

## 移行ジャーニーのタイムライン {#migration-journey-timeline}

アドビでは、まず Marketo Engage サブスクリプションを Adobe Admin Console に移行したあと、検証済みのメールアドレスを持つすべての既存ユーザを移行します。システム管理者または Marketo 製品管理者には、移行ジャーニーをガイドするメールが届きます。以下に、予想できる作業のタイムラインを示します。

![](assets/understanding-marketo-subscription-and-user-migration-1.png)

### サブスクリプション移行の完了 {#subscription-migration-complete}

Adobe Admin Console へのサブスクリプションの移行が完了すると、システム管理者にメールが届きます。

システム管理者は、Marketo ユーザへの影響を最小限に抑えるために、場合によっては、ユーザの移行を開始する前にいくつかの必要な手順を完了する必要があります。

* Marketo ユーザが現在 SSO でログインしている場合は、Adobe Admin Console で SSO を設定して、ユーザが引き続き SSO でログインできるようにする必要があります。Marketo ユーザが現在 SSO を利用していないが、Adobe Admin Console で SSO を設定したい場合は、移行ジャーニーのこの時点で設定できます。

* Adobe Admin Console で他のアドビ製品を既に管理している場合、アドビは、既存のコンソールにユーザを自動的に移行する同意を求める場合があります。メールの「使用を開始」ボタンをクリックして、同意ページに移動します。

現時点では、ユーザ管理に変更はありません。Marketo 製品は Admin Console に表示されますが、Marketo 管理者は引き続き Marketo 管理者エリアでユーザを管理し、ユーザは移行が完了するまで、引き続き Marketo ID でログインします。この間、ユーザの移行が開始されるまで、Marketo 製品を Admin Console で管理することはできません。これには、サブスクリプションに関連付けられた Dynamic Chat インスタンスが含まれます。

>[!NOTE]
>
>現在 SSO を使用していないが実装を検討している場合は、ユーザ移行を行う前に実装することをお勧めします。シングルサインオンの実装を希望しており、アドビ組織に SSO が実装されていない状態でサブスクリプションが Adobe ID に既にオンボードされている場合は、[Marketo サポート](https://nation.marketo.com/){target="_blank"}にチケットを送信し、「Admin Console での Marketo、SSO の実装」というトピックを指定してください。

### ユーザ移行のスケジュール設定 {#schedule-user-migration}

前の節で説明した前提条件をシステム管理者が完了すると、アドビは 30 日前にユーザ移行のスケジュールを自動的に設定し、Marketo の製品管理者に連絡して、ユーザ移行を管理します。

Marketo 製品管理者の手順：

* 予定されているユーザ移行開始日が記載されたメールを 30 日前に受け取ります。

* Marketo 管理エリア内にある Marketo Migration Console にアクセスできます。このコンソールでは、サブスクリプションの移行日を変更することもできます。

>[!NOTE]
>
>移行が複雑なので、日付の変更は予定日から 30 日以内に制限されます。もっと後の日付にする必要がある場合は、`marketocares@marketo.com` までメールを送信してください。

* My Marketo のバナーに、ユーザ移行開始日までのカウントダウンが表示されるのを確認します。

* ユーザ移行開始日の前日に、リマインダーメールが届きます。

### 移行日に向けてユーザの準備 {#prepare-users-for-migration-day}

Marketo 製品管理者は、すべてのユーザが移行日に向けて準備ができていることを確認してください。

* Marketo 管理エリアですべてのユーザの[メール検証](/help/marketo/product-docs/administration/users-and-roles/email-verification.md){target="_blank"}ステータスを確認します。メールアドレスを検証していないユーザに対して、検証を行うように促し、検証プロセスを完了する際の課題を解決できるように支援します。

* すべてのユーザに、今後行われる Adobe ID への移行の準備をさせます。

>[!NOTE]
>
>ユーザが移行すると、Marketo へのログイン方法の変更を通知するメールがアドビから届きます。ユーザは Adobe ID を使用した初回ログインの招待を受け入れるよう求められます。既存の Adobe ID でログインするか、同じメールアドレスを使用して新しい Adobe ID を設定して行います。

>[!IMPORTANT]
>
>Marketo Engage ユーザがメールアドレスを検証しない場合、Adobe ID に移行されず、サブスクリプションの移行が完了しても Marketo サブスクリプションにアクセスできなくなります。再度アクセスできるようにするには、Marketo 製品管理者によって新しいユーザとして追加される必要があります。

### 移行日に行われること {#what-to-expect-on-migration-day}

米国タイムゾーンのすべての Marketo サブスクリプションは、移行開始日の午前 0 時（太平洋標準時）から移行されます。その他すべてのサブスクリプションのユーザ移行は、サブスクリプションの指定タイムゾーンの午前 0 時に開始されます。

**アドビは最初に Marketo 管理者を自動的に移行します**。Marketo 管理者が Adobe ID に移行されると、以前に割り当てられていた他のロールとともに、Marketo アプリケーション内のアドビ製品管理者ロールが割り当てられます。

**Marketo サブスクリプションのユーザ数が 75 人未満で、Marketo やアドビ組織で SSO を使用していない場合**、アドビは残りのユーザを自動的に移行します。このワークフローは、最高レベルの自動化を実現して、Adobe Marketo ユーザのオーバーヘッドを最小限に抑えることを目的としています。移行を実行するためにユーザ側で必要なアクションはありません。

**Marketo サブスクリプションのユーザ数が 75 人を超える場合、または Marketo やアドビ組織で SSO を使用している場合**、Marketo 製品管理者は、Marketo 管理者領域にある Marketo Migration Console のセルフサービスユーザ移行領域にアクセスできるようになります。ユーザ移行プロセス中により詳細な制御を必要とするユーザに対して、Marketo 製品管理者はいつかのグループに分けてまたは一度にすべてを移行するユーザの選択を開始できます。ユーザを選択すると、管理者は「今すぐ移行」または後日の「移行をスケジュール」を選択できるので、どのユーザをいつ移行するかを非常に柔軟に制御できます。

>[!NOTE]
>
>ユーザの移行中に、製品にアクセスできなくなることはありません。ユーザの移行中にユーザがログインしていた場合、ユーザはログアウトされ、移行が完了した後、Adobe ID を使用して数分以内に再度ログインするように促されます。

ユーザが移行されると、Marketo へのログイン方法の変更を通知するメールがアドビからユーザに届きます。ユーザは Adobe ID を使用した初回ログインの招待を受け入れるよう求められます。既存の Adobe ID でログインするか、同じメールアドレスを使用して新しい Adobe ID を設定して行います。

詳しくは、[Adobe ID への移行](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}, [User Sign-in with Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"}, and [Adobe Identity Management FAQ](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}を参照してください。

## ユーザ移行の完了 {#user-migration-complete}

すべての管理者とユーザが移行されると、アドビはすべてのシステム管理者と製品管理者にメールで通知します。現時点では、そのサブスクリプションのすべての Marketo ユーザは Adobe ID を使用して Marketo にログインし、製品管理者はユーザの管理を Adobe Admin Console でのみ行います。

## サポートを受ける {#get-support}

サブスクリプションまたはユーザ移行に関する追加サポートについては、`marketocares@marketo.com` までメールでお問い合わせください。

>[!MORELIKETHIS]
>
>* [Adobe ID への移行](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}
>* [Adobe ID を使用したユーザログイン](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"}
>* [Adobe Identity Management に関するよくある質問](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}
