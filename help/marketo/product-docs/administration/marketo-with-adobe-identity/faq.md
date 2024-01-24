---
description: AdobeIdentity Management FAQ - Marketoドキュメント — 製品ドキュメント
title: AdobeIdentity Managementの FAQ
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: ab1ea483998d6cb37277b18adf2c1d3371bb40e6
workflow-type: tm+mt
source-wordcount: '1202'
ht-degree: 60%

---

# AdobeIdentity Managementの FAQ {#adobe-identity-management-faq}

**Adobe ID とは何ですか？**

Adobe Identity Management システムは、3 つのコンポーネントで構成されています。

* [!DNL Adobe Identity Service]：フェデレーションとランタイムシングルサインオン（SSO）を含む、エンドユーザーの認証と検証を処理します。

* Adobe Admin Console：Admin Console では、組織全体にわたるアドビの使用権限を一元的に管理できます。ユーザー管理、クラウドサービス、デスクトップライセンスの使用権限、フェデレーション設定を処理し、データ消失防止のセキュリティ機能を提供します。

* Adobe User Management API（UMAPI）：組織が Adobe Admin Console で API レベルでエンタープライズユーザーとエンタイトルメントを管理できるようにします。

**既存の Marketo Engage サブスクリプションは、いつ IMS と統合されますか？**

既存の Marketo サブスクリプションは、今年後半に Adobe Identity Management システムに移行されます。Marketo サポートでは、Adobe IMS の移行に関する更新を提供できません。アドビアカウントチームは、今後数か月以内に予定のタイムラインをお知らせします。

**製品管理者とアドビ管理者の違いは何ですか。**

* アドビ製品管理者は、Marketo プラットフォームの新しいロールです。
* アドビ製品管理者のロールは、Adobe Admin Console で製品管理者として追加されたユーザーに付与されます。
* アドビ製品管理者のロールは読み取り専用で、Marketo Engage から編集または削除することはできません。
* アドビ製品管理者は、標準の Marketo 管理者と同じ権限を持っています。
* Marketo Engage 管理者のロールは、引き続き管理者で、Marketo Engage でユーザーに付与されます。

**User Management API クライアントのサポートに何か変更はありますか？**

はい。Adobe IMS に転送されたユーザーは、既存の Marketo User Management API の一部を利用できます。ユーザーの招待、更新、削除アクションには、Adobe [IMS API](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} を使用する必要があります。ロール管理の場合は、Marketo User Management API が引き続き適用されます。これ以外には、Marketo REST API クライアントのサポートに対する変更はありません。

**IMS と統合された場合、サポートの問い合わせ先はどこですか？**

[Marketo サポート](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}に問い合わせる標準手順に従ってください。

**Adobe ID を使用して他のアドビアプリケーションにアクセスする場合、それを使用して Marketo にアクセスできますか？**

他のアドビ製品がある場合でも、サブスクリプションが IMS に移行されるまで、Adobe ID を使用して Marketo にアクセスできません。

**Marketo のユーザーのロール（ワークスペース内）は Adobe Admin Console で管理されますか？**

いいえ。（ワークスペース内の）ユーザーのロール管理は、Marketo Engage で完了します。

**私は IMS 統合サブスクリプションの Marketo 管理者ですが、Admin Console へのアクセス権がありません。アクセス権を取得する方法を教えてください。**

組織の Admin Console にアクセスできるアドビシステムまたは製品管理者なら誰でもアクセスを許可できます。組織内で誰がコンソールの管理者権限を持っているかが不明な場合は、[アドビカスタマーケア](https://helpx.adobe.com/contact.html){target="_blank"}にお問い合わせください。

**管理者はどのように Marketo [!DNL Sales Connect] にユーザーを追加しますか？**

[!DNL Sales Connect] の Admin Console には製品カードがありますが、Admin Console を使用してユーザーを追加／管理することはできません。[https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"} を使用すると、管理者は Marketo [!DNL Sales Connect] を使用してユーザーを管理できます。

**Adobe Admin Console の詳細はどこで確認できますか？**

[https://helpx.adobe.com/jp/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html){target="_blank"} を参照してください。

**マイアカウントのユーザーアカウントに変更を加えるためには、Marketo の管理者セクションにアクセスするのでしょうか？**

いいえ、[account.adobe.com](https://account.adobe.com){target="_blank"} に移動する必要があります。

**Marketo Universal ID との連携方法を教えてください。**

Adobe ID に転送されたユーザーは、製品の購読切り替えボタンを使用して、IMS 対応のすべての購読にシームレスにアクセスできます。

**SSO はサポートされていますか？**

はい。Marketo と Adobe IMS の統合では、ユニバーサル ID ユーザーと SSO がサポートされています。SSO は Adobe IMS によって駆動され、Adobe Admin Console で組織レベルで設定されます。[詳しくは、こちらを参照してください](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}。

* **既にAdobeID に転送されていますが、SSO を実装したいと思います。 どうすればいい？**

シングルサインオンを実装し、Adobe組織に SSO を実装せずにサブスクリプションがAdobeID に転送された場合は、にチケットを送信してください。 [Marketoサポート](https://nation.marketo.com/){target="_blank"} 「Marketo onAdmin Console、SSO の実装」というトピックを指定します。

**デバイス認証はどのように機能しますか？**

Adobe IMS は、現在、Marketo のデバイス認証機能などをサポートしていません。

**「ユーザーを招待ダイアログでログイン」機能を使用して、ユーザーのログインをメールから一意にすることは可能ですか？**

いいえ。サブスクリプションが IMS 有効の場合、ユーザー招待ワークフローはアクティブでなくなったので、この機能は無効になりました。Adobe ID では、ユーザーの ID としてメールを使用します。

**Adobe IMS の場合、Adobe ID、Enterprise ID、Federated ID を使用できますか？**

はい、サポートする ID のタイプを決定するのは組織です。詳しくは、[ID の概要](https://helpx.adobe.com/enterprise/using/identity.html)と [ID を設定](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}を確認してください。

**Adobe Admin Console でサポートされている製品カードは何ですか。**

サポートされる製品カードは、Marketo Engage、Marketo Measure、Marketo Dynamic Chat、Marketo Sales Connect、Marketo Sales Insight Actions です。

**ユーザー ID に移行した際に、ユーザーログインが電子メールと一致しない場合、AdobeID はどうなりますか？**

電子メールアドレスとは異なるログイン情報を持つ現在のMarketoユーザーは、AdobeID に移行すると、その資格情報を使用してログインしなくなります。 AdobeID は、常にユーザーの電子メールアドレスで認証されます。

**サブスクリプションで IP 制限設定が使用されている場合、AdobeID の移行後はどうなりますか。**

サブスクリプションがAdobeID に転送された場合、IP 制限設定はAdobe Admin Consoleに移行されません。 Marketoの IP 制限設定では、特定の IP アドレスからのアクセスのみを許可し、特定の IP アドレスへのアクセスをブロックします。 現時点では、AdobeIdentity Managementシステムは IP 制限機能をサポートしていません。

2024 年に、AdobeIdentity Management System は、特定の IP アドレスのみをサポートする機能をリリースし、現在この機能を使用しているMarketoユーザーへの移行をサポートします。 現在この機能を使用しているユーザーは、この機能がリリースされるまでユーザー移行を行いません。 機能が配信されると、移行がスケジュールされたことがユーザーに通知されます。 この機能の詳細は、利用可能になった時点で提供されます。

現在 IP 制限を使用しているユーザーは、特定のアドレスをアクセスからブロックして、AdobeID に移行後はこの機能を使用できなくなります。AdobeのIdentity Management System ではこの機能はサポートされないからです。

**「シングルサインオンをバイパス」を選択できる役割を持つユーザーがいる場合、AdobeID 移行後はどうなりますか？**

サブスクリプションがAdobeID に転送されると、すべてのユーザーのAdobe組織レベルでシングルサインオン (SSO) が設定されます。 SSO が設定されると、そのAdobe組織内のすべてのMarketoユーザー/すべてのMarketoインスタンスに対して適用されます。以前は、Marketoでは、ユーザーの役割の設定で「シングルサインオンをバイパス」オプションを使用できるようになりました。 これは、AdobeIdentity Management System ではサポートされていません。

**複数のサブスクリプションを持っていますが、すべてシングルサインオンが有効になっていません。 AdobeID の移行後はどうなりますか？**

サブスクリプションがAdobeID に転送されると、シングルサインオン (SSO) がAdobe組織レベルで設定されます。 つまり、SSO はAdobe組織内のすべての製品インスタンスに適用されます。SSO が設定されると、そのAdobe組織内のすべてのMarketoインスタンスに適用されます。以前は、Marketoは、インスタンスレベルでこの設定をサポートしていました。 これは、AdobeIdentity Management System ではサポートされていません。
