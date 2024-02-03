---
description: Adobe Identity Management の概要 - Marketo ドキュメント - 製品ドキュメント
title: Adobe Identity Management の概要
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: 6f9790c2243407f2622970d228c9de6be7697df6
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 54%

---

# Adobe Identity Management の概要 {#adobe-identity-management-overview}

すべての新しいAdobe Marketo Engageサブスクリプション（2023 年 7 月 31 日以降）は、AdobeIdentity Managementシステムと統合されます。 既存のMarketoサブスクリプションは、現在、更新または再契約イベント時にAdobeIdentity Managementシステムに移行中です。 現時点では、更新または再契約イベント以外の移行はサポートされていません。

>[!NOTE]
>
>Marketoサポートでは、Adobe IMSの移行に関する更新を提供できません。 Adobeアカウントチームは、今後数ヶ月以内に予定される予定日程で連絡を取ります。 詳しくは、 [この記事](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console.md){target="_blank"}, and the [Frequently Asked Questions](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

AdobeID に転送されたサブスクリプションの場合、Adobe Admin Consoleがユーザー管理に使用されます。 シングルサインオンなどの ID 関連の概念も、Admin Consoleで管理されます。

* 詳しくは、 [Adobe Admin Console](https://helpx.adobe.com/jp/enterprise/using/admin-console.html){target="_blank"}.
* 次の情報を検索： [Marketoサブスクリプションに関連するAdobe組織の設定](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

>[!NOTE]
>
>シングルサインオンを実装し、Adobe組織に SSO を実装せずにサブスクリプションがAdobeID に転送された場合は、にチケットを送信してください。 [Marketoサポート](https://nation.marketo.com/){target="_blank"} 「Marketo onAdmin Console、SSO の実装」というトピックを指定します。

## プロファイルレベル {#profile-levels}

Adobe Marketo Engage を Adobe Identity Management システムに転送した場合、様々なプロファイルがサポートされます。この統合に関連するユーザープロファイルのタイプは以下のとおりです。

<table>
 <tr>
  <td><strong>Adobe Admin Console システム管理者</strong></td>
  <td>Adobe Admin Console でアドビ組織と Marketo Engage 製品の ID 概念を設定します。アドビ組織の設定で付与されたロールです。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console 製品管理者</strong></td>
  <td>Adobe Admin Console でのユーザー製品に対する Marketo Engage の権限を付与します。Adobe Admin Console で付与されたロールです。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console 製品プロファイル管理者</strong></td>
  <td>製品プロファイル内のユーザーの管理を担当します。特定のプロファイル以外のユーザーは管理できません。製品プロファイル管理者は、製品プロファイルにユーザーとして追加されない限り、Marketo アプリケーションにアクセスできません。ロールは標準ユーザーのままです（複数のワークスペースがある場合はデフォルトのワークスペース）。
</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage 製品管理者</strong></td>
  <td>管理者権限を持つ Marketo Engage へのアクセス権を付与されたユーザー。Adobe Admin Console ではなく、Marketo Engage で付与されたロール。</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage ユーザー</strong></td>
  <td>Marketo Engage へのアクセス権を付与されたユーザー。管理者権限はありません。</td>
 </tr>
</table>

## よくある質問 {#faq}

よくある質問 [ここにあります](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [管理者設定](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [製品管理者の追加または削除](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md){target="_blank"}
>* [ユーザーの追加または削除](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}
