---
description: 概要 — Marketoドキュメント — 製品ドキュメント
title: 概要
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
source-git-commit: 7eff888c0fdebf31da4706f70d1e99e8327807ca
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 2%

---

# 概要 {#overview}

2022 年 2 月 15 日現在、AdobeMarketo Engageの新しいアカウント（既存のアカウントの新しいインスタンスだけでなく、新しいアカウント）をお持ちの場合、購入した製品パッケージに応じて、AdobeIdentity Management System と統合される場合があります。 既にアクセスしているかどうかを確認するには、Marketo管理者またはアカウントのカスタマーサクセスマネージャーにお問い合わせください。

既存のMarketoサブスクリプションは、今年後半からAdobeIdentity Managementシステムに移行されます。

>[!NOTE]
>
>Marketoサポートでは、Adobe IMSの移行に関する更新を提供できません。 カスタマーサクセスマネージャーは、今後数ヶ月の予定タイムラインを提示します。

## プロファイルレベル

AdobeMarketo EngageをAdobeIdentity Management System に転送した場合、様々なプロファイルがサポートされます。 この統合に関連するユーザープロファイルのタイプは次のとおりです。

<table>
 <tr>
  <td><strong>Adobe Admin Console System Admin</strong></td>
  <td>Adobe Admin ConsoleでAdobe組織とMarketo Engage製品の ID 概念を設定します。 ロールをAdobe組織設定で付与</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console製品管理者</strong></td>
  <td>Adobe Admin Consoleでのユーザー製品に対するMarketo Engageの権限を付与します。 Adobe Admin Consoleでの役割を付与しました。</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage製品管理者</strong></td>
  <td>管理者権限を持つMarketo Engageへのアクセス権を付与された人。 Adobe Admin Consoleではなく、Marketo Engageでの役割を付与しました。</td>
 </tr>
 <tr>
  <td><strong>Marketo Engageユーザ</strong></td>
  <td>Marketo Engageへのアクセス権を付与された人。 管理者権限がありません。</td>
 </tr>
</table>

## よくある質問

**AdobeID とは**

AdobeIdentity Management System は、3 つのコンポーネントで構成されています。

* AdobeID サービス：フェデレーションとランタイムシングルサインオン (SSO) を含む、エンドユーザーの認証と検証を処理します。

* Adobe Admin Console:Admin Consoleでは、組織全体にわたるAdobeの使用権限を一元的に管理できます。 ユーザー管理、クラウドサービス、デスクトップライセンスの使用権限、フェデレーション設定を処理し、データ消失防止のセキュリティ機能を提供します。

* Adobeユーザー管理 API(UMAPI):組織がAdobe Admin Consoleで API レベルでエンタープライズユーザーとエンタイトルメントを管理できるようにします。

**既存のMarketo Engage購読は、いつ IMS と統合されますか？**

既存のMarketoサブスクリプションは、今年後半にAdobeIdentity Managementシステムに移行されます。 Marketoサポートでは、Adobe IMSの移行に関する更新を提供できません。 カスタマーサクセスマネージャーは、今後数ヶ月の予定タイムラインを提示します。

**製品管理者とAdobe管理者の違いは何ですか。**

* Adobe製品管理者は、Marketoプラットフォームの新しい役割です。
* Adobe製品管理者の役割は、Adobe Admin Consoleで製品管理者として追加されたユーザーに付与されます。
* Adobe製品管理者は読み取り専用のロールで、Marketo Engageから編集または削除することはできません。
* Adobe製品管理者は、標準のMarketo管理者と同じ権限を持っています。
* Marketo Engage管理者の役割は、引き続き管理者で、ユーザーに付与されます。Marketo Engage。

**User Management API クライアントのサポートに何か変更はありますか？**

はい.。Adobe IMSに転送されたユーザーは、既存のMarketo User Management API をすべて利用できません。 ユーザーの招待、更新、削除のアクションの場合は、Adobe [IMS API](https://www.adobe.io/apis/experienceplatform/umapi-new.html) を使用する必要があります。 ロール管理の場合、Marketo User Management API は引き続き適用されます。 これ以外に、Marketo REST API クライアントのサポートに対する他の変更はありません。

**IMS と統合されている場合、サポートに問い合わせる相手は誰ですか？**

連絡の標準手順に従います [Marketoサポート](https://nation.marketo.com/t5/support/ct-p/Support).

**Marketoのユーザーの役割（ワークスペース内）はAdobe Admin Consoleで管理されますか？**

いいえ.（ワークスペース内の）ユーザーロール管理は、Marketo Engageで完了します。

**IMS 統合サブスクリプションのMarketo管理者で、Admin Consoleへのアクセス権がありません。 アクセス権を取得する方法を教えてください。**

組織のAdobeにアクセスできるAdmin Consoleシステム管理者または製品管理者が、ユーザーにアクセス権を付与できます。 組織内で誰がコンソールの管理者権限を持っているかが不明な場合は、にお問い合わせください。 [Adobeカスタマーケア](https://helpx.adobe.com/contact.html).

**管理者はMarketo Sales Connect にユーザーを追加しますか。**

セールスコネクトのAdmin Consoleには製品カードがありますが、Admin Consoleを使用してユーザーを追加/管理することはできません。 次のリンクをクリックすると、管理者はMarketo Sales Connect を使用してユーザーを管理できます。 [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management).

**Adobe Admin Consoleの詳細はどこで確認できますか？**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html).

**引き続きMarketoの「管理者」セクションに移動して、自分のアカウントに対してユーザーアカウントを変更しますか？**

いいえ、次の場所に移動する必要があります： [account.adobe.com](https://account.adobe.com).

**Marketo Universal ID との連携方法**

AdobeID に転送されたユーザーは、製品の購読切り替えボタンを使用して、IMS 対応のすべての購読にシームレスにアクセスできます。

**これは SSO で機能しますか？**

はい.。MarketoとAdobe IMSの統合では、ユニバーサル ID ユーザーと SSO がサポートされます。 SSO はAdobe IMSによって駆動され、Adobe Admin Consoleで組織レベルで設定されます。 [詳細はこちら](https://helpx.adobe.com/enterprise/using/set-up-identity.html)を参照してください。

**デバイス認証はどのように機能しますか？**

Adobe IMSは、現在、Marketoのデバイス認証機能などをサポートしていません。

**ユーザーのログインをメールで一意にするために、「ユーザーを招待ダイアログでログイン」機能を使用することは可能ですか？**

いいえ.サブスクリプションが IMS 有効の場合、ユーザー招待ワークフローはアクティブでなくなったので、この機能は無効になりました。 AdobeID は、E メールでユーザーの ID を駆動する必要があります。

**Adobe IMSの場合、Adobe ID、Enterprise ID、Federated IDのどちらを使用できますか。**

はい、組織がサポートする ID のタイプを決定します。 詳しくは、以下を参照してください。 [ID の概要](https://helpx.adobe.com/enterprise/using/identity.html) そしてここに [ID の設定](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

>[!MORELIKETHIS]
>
>* [管理者の設定](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md)
>* [製品管理者の追加または削除](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md)
>* [ユーザーの追加または削除](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md)

