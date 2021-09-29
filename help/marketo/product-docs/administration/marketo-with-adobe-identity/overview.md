---
description: 概要 — Marketoドキュメント — 製品ドキュメント
title: 概要
hide: true
hidefromtoc: true
source-git-commit: 8ef7611e9a6b9756d35a9c8fbd439f25f5c714be
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 1%

---

# 概要 {#overview}

AdobeMarketo Engageサブスクリプションが10/4/21以降にプロビジョニングされた場合は、AdobeIdentity Managementシステムに統合されます。 AIMS を使用すると、ユーザーは、共通のMarketo EngageID を使用して、Experience Cloudやその他のAdobeアプリケーションにサインインできます。

## プロファイルレベル

3 つのプロファイルレベルがあります。

<table>
 <tr>
  <td><strong>システム管理者</strong></td>
  <td>Adobe Admin ConsoleのAdobe組織とMarketo Engage製品の ID 概念を設定します。</td>
 </tr>
 <tr>
  <td><strong>製品管理者</strong></td>
  <td>Adobe Admin Consoleでユーザーに対してMarketo Engage製品の使用権限を付与します。</td>
 </tr>
 <tr>
  <td><strong>ユーザ</strong></td>
  <td>Marketo Engage 管理者権限がありません。</td>
 </tr>
</table>

## FAQ

**AdobeID とは**

AdobeIdentity Management System は、3 つのコンポーネントで構成されています。

* AdobeID サービス：フェデレーションとランタイムのシングルサインオン (SSO) を含む、エンドユーザーの認証と検証を処理します。

* Adobe Admin Console:Admin Consoleは、組織全体にわたるAdobeの使用権限を一元的に管理できます。 ユーザー管理、クラウドサービス、デスクトップライセンスの資格、フェデレーション設定を処理し、データ消失防止のセキュリティ機能を提供します。

* Adobeユーザー管理 API(UMAPI):API レベルで企業のユーザーと権利をAdobe Admin Consoleで管理できます。

**製品管理者とAdobe管理者の違いは何ですか。**

* Adobe製品管理者は、Marketoプラットフォームの新しい役割です。
* これは読み取り専用の役割で、Marketoから編集または削除することはできません。
* 標準のMarketo Admin と同じ権限と権限を持ちます。

**API クライアントのサポートに何か変更はありますか？**

はい. Adobe IMSに転送されたユーザーは、既存のMarketo User Management API を利用できません。 [IMS API](https://www.adobe.io/apis/experienceplatform/umapi-new.html) を使用します。

**サポートを受けるための連絡先は？**

[Marketoサポート ](https://nation.marketo.com/t5/support/ct-p/Support) に問い合わせる際の標準的な手順に従います。

**Marketoのユーザーの役割（ワークスペース内）はAdobe Admin Consoleで管理されますか？**

いいえ. （ワークスペース内の）ユーザーロールの管理は、Marketoで完了します。

**私はMarketo管理者で、そのAdmin Consoleへのアクセス権を持っていません。アクセスを得る方法は？**

組織のシステムにアクセスできるシステム管理者または製品Admin Consoleは、すべてアクセス権を付与できます。 組織内で誰がコンソールの管理者権限を持っているかわからない場合は、[Adobeカスタマーケア ](https://helpx.adobe.com/contact.html) にお問い合わせください。

**管理者がMarketo Sales Connect にユーザーを追加する方法を教えてください。**

Sales Connect の AC には製品カードがありますが、AC を使用してユーザーを追加/管理しないでください。 次のリンクをクリックすると、管理者はMarketo Sales Connect を使用してユーザーを管理できます。[https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management).

**Adobe Admin Consoleの詳細はどこで確認できますか？**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html)を参照してください。

**アカウントに変更を加えるために、引き続きMarketoの「管理者」セクションに移動しますか？**

いいえ。[account.adobe.com](https://account.adobe.com) に移動する必要があります。

**これはMarketoのユニバーサル ID とどのように連携しますか。**

AdobeID に転送されたユーザーは、製品のサブスクリプション切り替えボタンを使用して、IMS 対応のすべてのサブスクリプションにシームレスにアクセスできます。

**これは SSO で機能しますか？**

はい. MarketoとAdobe IMSの統合では、ユニバーサル ID ユーザーと SSO がサポートされます。 SSO はAdobe IMSによって駆動され、Adobe Admin Consoleの組織レベルで設定されます。 [詳細はこちら](https://helpx.adobe.com/enterprise/using/set-up-identity.html)を参照してください。

**デバイスの承認はどのように機能しますか？**

Adobe IMSは、現在、Marketoのデバイス認証機能などをサポートしていません。

**「ユーザーを招待ダイアログでログイン」機能を使用して、ログインを電子メールから一意にすることは可能ですか？**

いいえ. サブスクリプションが IMS に対応している場合、ユーザー招待ワークフローがアクティブでなくなったので、この機能は無効になります。 AdobeID は、ユーザーの ID を E メールで駆動する必要があります。

**Adobe IMSの場合、Adobe ID、Enterprise ID、Federated IDのいずれを使用できますか。**

はい、組織がサポートする ID のタイプを決定します。 詳細 [ ここ ](https://helpx.adobe.com/enterprise/using/identity.html) と [ ここ ](https://helpx.adobe.com/enterprise/using/set-up-identity.html)。

>[!MORELIKETHIS]
>
>* [管理設定](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md)
>* [製品管理者の追加または削除](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md)
>* [ユーザーの追加または削除](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md)