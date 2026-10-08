---
description: 移行のタイミング、Admin Consoleのユーザー管理、システム管理者や製品管理者などのプロファイルレベルなど、Marketo Engage向けAdobe Identity Managementの概要。
title: Adobe Identity Management の概要
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
TQID: 'https://experienceleague.adobe.com/6af3WC1QOameThPvZTRmanxHl8nkFZaHquHJytngGmI'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b73410f7-454c-5670-baa7-a84eae014e94
    internal-label: Marketo with Adobe Identity
subfeature_v2:
  - id: efc9a24a-a6a4-449d-a3e6-44f6c74dfd46
    internal-label: Adobe Identity Management
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 59%
---
# Adobe Identity Management の概要 {#adobe-identity-management-overview}

すべての新しい Adobe Marketo Engage サブスクリプション（2023年7月31日（PT）以降）は、Adobe Identity Management システムと統合されます。

Adobe Identity にオンボードされたサブスクリプションの場合、Adobe Admin Console がユーザ管理に使用されます。 シングルサインオンなどのID関連の概念も、Admin Consoleで管理されます。

* 詳しくは、[Adobe Admin Console](https://helpx.adobe.com/jp/enterprise/using/admin-console.html){target="_blank"}を参照してください。
* Marketo サブスクリプションに関連する[Adobe組織の設定](https://helpx.adobe.com/jp/enterprise/using/set-up-identity.html){target="_blank"}の詳細をご覧ください。

>[!NOTE]
>
>シングルサインオンを導入する場合、サブスクリプションがAdobe組織でSSOを実装せずにAdobe Identityにオンボーディングされている場合は、[Marketo サポート ](https://nation.marketo.com/){target="_blank"}にチケットを送信し、トピックを「Marketo Admin Console版、SSOを実装」に指定します。

## プロファイルレベル {#profile-levels}

Adobe Identity Management システムにオンボーディングされたAdobe Marketo Engage サブスクリプションは、様々なプロファイルをサポートします。 この統合に関連するユーザープロファイルのタイプは以下のとおりです。

<table>
 <tr>
  <td><strong>Adobe Admin Console システム管理者</strong></td>
  <td>Adobe Admin Console で、アドビ組織および Marketo Engage 製品に対する ID 関連の概念を設定する役割を担います。 アドビ組織の設定で付与されたロールです。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console 製品管理者</strong></td>
  <td>Adobe Admin Console で、ユーザに Marketo Engage 製品の利用権限を付与する役割を担います。 Adobe Admin Console で付与されたロールです。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console 製品プロファイル管理者</strong></td>
  <td>製品プロファイル内のユーザーの管理を担当します。 特定のプロファイル以外のユーザーは管理できません。 製品プロファイル管理者は、製品プロファイルにユーザーとして追加されない限り、Marketo アプリケーションにアクセスできません。 役割は引き続き標準ユーザーになります（複数のワークスペースがある場合はデフォルトのワークスペース）。
</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage 管理者</strong></td>
  <td>管理者権限を持つ Marketo Engage へのアクセス権を付与されたユーザ。 Adobe Admin ConsoleではなくMarketo Engageで付与されたロール（<b> ユーザーを編集</b> モーダルの「管理者」としてのみ表示）。</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage ユーザー</strong></td>
  <td>Marketo Engage へのアクセス権を付与されたユーザー。 管理者権限はありません。</td>
 </tr>
</table>

>[!MORELIKETHIS]
>
>* [管理者設定](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [製品管理者の追加または削除](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-product-admin.md){target="_blank"}
>* [ユーザーの追加または削除](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-user.md){target="_blank"}
