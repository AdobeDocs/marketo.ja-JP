---
description: Adobe Identity Management の概要 - Marketo ドキュメント - 製品ドキュメント
title: Adobe Identity Management の概要
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: 1defe6e8c7b4e458203169150ec77df4f615e5d2
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 92%

---

# Adobe Identity Management の概要 {#adobe-identity-management-overview}

すべての新しい Adobe Marketo Engage サブスクリプション（2023年7月31日（PT）以降）は、Adobe Identity Management システムと統合されます。既存の Marketo Engage サブスクリプションは現在、更新、再契約イベント、追加などの販売イベントの際に Adobe Identity Management System に移行されています。現時点では、販売イベント以外の移行はサポートされていません。

>[!NOTE]
>
>Marketo サポートでは、Adobe IMS の移行に関する更新を提供できません。アドビのアカウントチームは、今後数か月以内に予定のタイムラインをお知らせします。詳しくは、[ この記事 ](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console.md){target="_blank"} および [ よくある質問 ](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"} を参照してください。

Adobe ID にオンボードされたサブスクリプションの場合、Adobe Admin Console がユーザ管理に使用されます。シングルサインオンなどの ID 関連の概念も、Admin Console で管理されます。

* 詳しくは、[Adobe Admin Console](https://helpx.adobe.com/jp/enterprise/using/admin-console.html){target="_blank"} を参照してください。
* 詳しくは、[Marketo サブスクリプションに関連するアドビ組織の設定](https://helpx.adobe.com/jp/enterprise/using/set-up-identity.html?lang=jp){target="_blank"}を参照してください。

>[!NOTE]
>
>シングルサインオンを実装し、アドビ組織に SSO を実装されていない状態でサブスクリプションが Adobe ID にオンボードされている場合は、[Marketo サポート](https://nation.marketo.com/){target="_blank"}にチケットを送信し、「Admin Console での Marketo、SSO の実装」というトピックを指定します。

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
  <td><strong>Marketo Engage管理者</strong></td>
  <td>管理者権限を持つ Marketo Engage へのアクセス権を付与されたユーザー。Adobe Admin Consoleではなく、Marketo Engageでのロールを付与されます（「ユーザーを編集 <b> モーダルでは単に「管理者」として表示さ </b> ます）。</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage ユーザー</strong></td>
  <td>Marketo Engage へのアクセス権を付与されたユーザー。管理者権限はありません。</td>
 </tr>
</table>

## よくある質問 {#faq}

よくある質問は[ここにあります](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}。

>[!MORELIKETHIS]
>
>* [管理者設定](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [製品管理者の追加または削除](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md){target="_blank"}
>* [ユーザーの追加または削除](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}
