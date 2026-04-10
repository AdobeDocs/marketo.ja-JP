---
description: 移行のタイミング、Admin Consoleのユーザー管理、システム管理者や製品管理者などのプロファイルレベルなど、Marketo Engage向けAdobe Identity Managementの概要。
title: Adobe Identity Management の概要
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: 9e21f8a6a95717b1c9794fd7819a2230105370ec
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 66%

---

# Adobe Identity Management の概要 {#adobe-identity-management-overview}

Adobe Marketo Engageのすべての新規サブスクリプション（2023年7月31日以降）は、Adobe Identity Management システムと統合されます。

Adobe ID にオンボードされたサブスクリプションの場合、Adobe Admin Console がユーザ管理に使用されます。シングルサインオンなどのID関連の概念も、Admin Consoleで管理されます。

* 詳しくは、[Adobe Admin Console](https://helpx.adobe.com/jp/enterprise/using/admin-console.html){target="_blank"}を参照してください。
* Marketo サブスクリプションに関連する[Adobe組織の設定](https://helpx.adobe.com/jp/enterprise/using/set-up-identity.html){target="_blank"}の詳細をご覧ください。

>[!NOTE]
>
>シングルサインオンを導入し、サブスクリプションがAdobe組織でSSOを実装せずにAdobe Identityにオンボーディングされている場合は、[Marketo サポート ](https://nation.marketo.com/){target="_blank"}にチケットを送信し、トピックを「Marketo Admin Console版、SSOを実装」に指定してください。

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
  <td><strong>Marketo Engage 管理者</strong></td>
  <td>管理者権限を持つ Marketo Engage へのアクセス権を付与されたユーザ。Adobe Admin Console ではなく、Marketo Engage でロールが付与されます（<b>ユーザを編集</b>モーダルでは単に「管理者」として表示されます）。</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage ユーザー</strong></td>
  <td>Marketo Engage へのアクセス権を付与されたユーザー。管理者権限はありません。</td>
 </tr>
</table>

>[!MORELIKETHIS]
>
>* [管理者設定](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [製品管理者の追加または削除](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-product-admin.md){target="_blank"}
>* [ユーザーの追加または削除](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-user.md){target="_blank"}
