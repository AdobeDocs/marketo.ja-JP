---
description: 概要 - Marketo ドキュメント - 製品ドキュメント
title: 概要
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
source-git-commit: 0d1762d9a5607d72af625aafbf7b9f412d6713c1
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 68%

---

# 概要 {#overview}

2022 年 2 月 15 日現在、Adobe Marketo Engageの新しいアカウント（既存のアカウントの新しいインスタンスだけでなく、新しいアカウント）をお持ちの場合、購入した製品パッケージに応じて、AdobeIdentity Management System と統合される場合があります。 既にアクセスしているかどうかを確認するには、Marketo管理者またはアカウントのカスタマーサクセスマネージャーにお問い合わせください。

既存のMarketoサブスクリプションは、今年後半からAdobeIdentity Managementシステムに移行されます。

>[!NOTE]
>
>Marketoサポートでは、Adobe IMSの移行に関する更新を提供できません。 カスタマーサクセスマネージャーは、今後数ヶ月の予定タイムラインを提示します。

## プロファイルレベル {#profile-levels}

Adobe Marketo Engage を Adobe Identity Management System に転送した場合、様々なプロファイルがサポートされます。この統合に関連するユーザープロファイルのタイプは次のとおりです。

<table>
 <tr>
  <td><strong>Adobe Admin Console システム管理者</strong></td>
  <td>Adobe Admin Console で Adobe 組織と Marketo Engage 製品の ID 概念を設定します。Adobe 組織設定での役割を付与。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console 製品管理者</strong></td>
  <td>Adobe Admin Console でのユーザー製品に対する Marketo Engage の権限を付与します。Adobe Admin Console での役割を付与。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console製品プロファイル管理</strong></td>
  <td>管理者および関連するすべての管理機能に割り当てられている製品プロファイルの説明を管理します。</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage 製品管理者</strong></td>
  <td>管理者権限を持つ Marketo Engage へのアクセス権を付与されたユーザー。Adobe Admin Console ではなく、Marketo Engage での役割を付与。</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage ユーザー</strong></td>
  <td>Marketo Engage へのアクセス権を付与されたユーザー。管理者権限はありません。</td>
 </tr>
</table>

## よくある質問 {#faq}

**Adobe Identity とは何ですか？**

Adobe Identity Management System は、3 つのコンポーネントで構成されています。

* Adobe Identity サービス：フェデレーションとランタイムシングルサインオン（SSO）を含む、エンドユーザーの認証と検証を処理します。

* Adobe Admin Console：Admin Console では、組織全体にわたる Adobe の使用権限を一元的に管理できます。ユーザー管理、クラウドサービス、デスクトップライセンスの使用権限、フェデレーション設定を処理し、データ消失防止のセキュリティ機能を提供します。

* Adobe User Management API（UMAPI）：組織が Adobe Admin Console で API レベルでエンタープライズユーザーとエンタイトルメントを管理できるようにします。

**既存のMarketo Engage購読は、いつ IMS と統合されますか？**

既存のMarketoサブスクリプションは、今年後半にAdobeIdentity Managementシステムに移行されます。 Marketoサポートでは、Adobe IMSの移行に関する更新を提供できません。 カスタマーサクセスマネージャーは、今後数ヶ月の予定タイムラインを提示します。

**製品管理者と Adobe 管理者の違いは何ですか。**

* Adobe 製品管理者は、Marketo プラットフォームの新しい役割です。
* Adobe 製品管理者の役割は、Adobe Admin Console で製品管理者として追加されたユーザーに付与されます。
* Adobe 製品管理者の役割は読み取り専用で、Marketo Engage から編集または削除することはできません。
* Adobe 製品管理者は、標準の Marketo 管理者と同じ権限を持っています。
* Marketo Engage 管理者の役割は、引き続き管理者で、Marketo Engage でユーザーに付与されます。

**User Management API クライアントのサポートに何か変更はありますか？**

はい。Adobe IMS に転送されたユーザーは、既存の Marketo User Management API の一部を利用できます。ユーザーの招待、更新、削除のアクションの場合は、Adobe [IMS API](https://www.adobe.io/apis/experienceplatform/umapi-new.html) を使用する必要があります。 役割管理の場合、Marketo User Management API は引き続き適用されます。これ以外に、Marketo REST API クライアントのサポートに対する他の変更はありません。

**IMS と統合されている場合、サポートに問い合わせる相手は誰ですか？**

[Marketo サポート](https://nation.marketo.com/t5/support/ct-p/Support)に問い合わせる標準手順に従ってください。

**AdobeID を使用して他のAdobeアプリケーションにアクセスする場合、それを使用してMarketoにアクセスできますか。**

他のAdobe製品がある場合でも、サブスクリプションが IMS に移行されるまで、AdobeID を使用してMarketoにアクセスできません。

**Marketo のユーザーの役割（ワークスペース内）は Adobe Admin Console で管理されますか？**

いいえ。（ワークスペース内の）ユーザーの役割管理は、Marketo Engage で完了します。

**IMS 統合サブスクリプションのMarketo管理者で、Admin Consoleへのアクセス権がありません。 アクセス権を取得する方法を教えてください。**

組織の Admin Console にアクセスできるアドビシステムまたは製品管理者なら誰でもアクセスを許可できます。組織内で誰がコンソールの管理者権限を持っているかが不明な場合は、[アドビカスタマーケア](https://helpx.adobe.com/contact.html)にお問い合わせください。

**管理者はどのように Marketo Sales Connect にユーザーを追加しますか？**

Sales Connect の Admin Console には製品カードがありますが、Admin Console を使用してユーザーを追加／管理することはできません。[https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management) をクリックすると、管理者は Marketo Sales Connect を使用してユーザーを管理できます。

**Adobe Admin Console の詳細はどこで確認できますか？**

[Https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html) にアクセスしてください。

**引き続きMarketoの「管理者」セクションに移動して、自分のアカウントに対してユーザーアカウントを変更しますか？**

いいえ、[account.adobe.com](https://account.adobe.com).にアクセスする必要があります。

**Marketo Universal ID との連携方法を教えてください。**

AdobeID に転送されたユーザーは、製品の購読切り替えボタンを使用して、IMS 対応のすべての購読にシームレスにアクセスできます。

**SSO はサポートされていますか？**

はい。Marketo と Adobe IMS の統合では、ユニバーサル ID ユーザーと SSO がサポートされています。SSO は Adobe IMS によって駆動され、Adobe Admin Console で組織レベルで設定されます。[詳細はこちら](https://helpx.adobe.com/enterprise/using/set-up-identity.html)を参照してください。

**デバイス認証はどのように機能しますか？**

Adobe IMS は、現在、Marketo のデバイス認証機能などをサポートしていません。

**ユーザーのログインをメールで一意にするために、「ユーザーを招待ダイアログでログイン」機能を使用することは可能ですか？**

いいえ。サブスクリプションが IMS 有効の場合、ユーザー招待ワークフローはアクティブでなくなったので、この機能は無効になりました。Adobe ID では、ユーザーの ID としてメールを使用します。

**Adobe IMS の場合、Adobe ID、Enterprise ID、Federated ID を使用できますか？**

はい、サポートする ID のタイプを決定するのは組織です。詳しくは、[ID の概要](https://helpx.adobe.com/enterprise/using/identity.html)と [ID の設定](https://helpx.adobe.com/enterprise/using/set-up-identity.html)を確認してください。

>[!MORELIKETHIS]
>
>* [管理者設定](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md)
>* [製品管理者の追加または削除](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md)
>* [ユーザーの追加または削除](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md)

