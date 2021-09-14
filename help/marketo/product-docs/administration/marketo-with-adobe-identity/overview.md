---
description: 概要 — Marketoドキュメント — 製品ドキュメント
title: 概要
hide: true
hidefromtoc: true
source-git-commit: 306e08b08bf63fe51778dc51ccb9cb971fed2f4b
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 1%

---

# 概要 {#overview}

AdobeMarketo Engageサブスクリプションが10/4/21以降にプロビジョニングされた場合は、AdobeIdentity Managementシステムに統合されます。 AIMSを使用すると、ユーザーは、共通のMarketo EngageIDを使用して、Experience Cloudやその他のAdobeアプリケーションにログインできます。

## プロファイルレベル

3つのプロファイルレベルがあります。

<table>
 <tr>
  <td><strong>システム管理者</strong></td>
  <td>Adobe Admin ConsoleのAdobe組織とMarketo Engage製品のID概念を設定します。</td>
 </tr>
 <tr>
  <td><strong>製品管理者</strong></td>
  <td>Adobe Admin Consoleでユーザーに対してMarketo Engage製品の使用権限を付与します。</td>
 </tr>
 <tr>
  <td><strong>ユーザ</strong></td>
  <td>Marketo Engage 管理者権限はありません。</td>
 </tr>
</table>

## FAQ

**AdobeIDとは**

AdobeIdentity Management Systemは、3つのコンポーネントで構成されています。

* AdobeIDサービス：フェデレーションとランタイムのシングルサインオン(SSO)を含む、エンドユーザーの認証と検証を処理します。

* Adobe Admin Console:Admin Consoleは、組織全体にわたるAdobeの使用権限を一元的に管理するための場所です。 ユーザー管理、クラウドサービス、デスクトップライセンスの資格、フェデレーション設定を処理し、データ損失防止のセキュリティ機能を提供します。

* Adobeユーザー管理API(UMAPI):組織がAdobe Admin ConsoleでAPIレベルでエンタープライズユーザーとエンタイトルメントを管理できるようにします。

**製品管理者とAdobe管理者の違いは何ですか。**

* Adobe製品管理者は、Marketoプラットフォームの新しい役割です。
* これは読み取り専用の役割で、Marketoから編集または削除することはできません。
* 標準のMarketo Adminと同じ権限と権限を持ちます。

**APIクライアントのサポートに変更はありますか？**

はい. Adobe IMSに転送されたユーザーは、既存のMarketo User Management APIを利用できません。 [IMS API](https://www.adobe.io/apis/experienceplatform/umapi-new.html)を使用します。

**サポートを受けるための連絡先は？**

[Marketoサポート](https://nation.marketo.com/t5/support/ct-p/Support)に連絡する際の標準的な手順に従います。

**Marketoユーザーの役割（ワークスペース内）はAdobe Admin Consoleで管理されますか？**

いいえ. （ワークスペース内の）ユーザーロールの管理は、Marketoで完了します。

**私はMarketo管理者で、そのAdmin Consoleへのアクセス権を持っていません。アクセスを得る方法は？**

組織のシステムにアクセスできるシステム管理者または製品Admin Consoleは、すべてユーザーにアクセス権を付与できます。 組織内の誰がコンソールの管理者権限を持っているかわからない場合は、[Adobeカスタマーケア](https://helpx.adobe.com/contact.html)にお問い合わせください。

**管理者がMarketo Sales Connectにユーザーを追加する方法を教えてください。**

Sales ConnectのACには製品カードがありますが、ACを使用してユーザーを追加/管理しないでください。 次のリンクをクリックすると、管理者はMarketo Sales Connectを使用してユーザーを管理できます。[https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management).

**Adobe Admin Consoleの詳細はどこで確認できますか？**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html)を参照してください。

**引き続きMarketoの「管理者」セクションに移動して、アカウントに変更を加えますか？**

いいえ。[account.adobe.com](https://account.adobe.com)に移動する必要があります。

**これはMarketoのユニバーサルIDとどのように連携しますか。**

AdobeIDに転送されたユーザーは、製品内の購読切り替えボタンを使用して、IMS対応のすべての購読にシームレスにアクセスできます。

**これはSSOで機能しますか？**

はい. MarketoとAdobe IMSの統合では、ユニバーサルIDユーザーとSSOがサポートされます。 SSOはAdobe IMSによって駆動され、Adobe Admin Consoleの組織レベルで設定されます。 [詳細はこちら](https://helpx.adobe.com/enterprise/using/set-up-identity.html)を参照してください。

**デバイスの承認はどのように機能しますか？**

Adobe IMSは、現在、Marketoのデバイス認証機能などをサポートしていません。

**電子メールからログインを一意にするために、「ユーザーを招待ダイアログでログイン」機能を引き続き使用できますか？**

いいえ. サブスクリプションがIMSに対応している場合、ユーザー招待ワークフローがアクティブでなくなったので、この機能は無効になりました。 AdobeIDは、ユーザーのIDをEメールで駆動する必要があります。

**Adobe IMSの場合、Adobe ID、Enterprise ID、Federated IDのどちらを使用できますか。**

はい、組織がサポートするIDのタイプを決定します。 詳細[ここ](https://helpx.adobe.com/enterprise/using/identity.html)と[ここ](https://helpx.adobe.com/enterprise/using/set-up-identity.html)。
