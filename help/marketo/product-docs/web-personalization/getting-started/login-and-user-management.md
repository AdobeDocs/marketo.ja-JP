---
unique-page-id: 7513771
description: login and user management login-and-user-managementを使用して、Marketo Engageでログインとユーザー管理を行う方法について説明します。 このガイドを使用して、次のステップを完了してください。
title: ログインとユーザー管理
exl-id: 3cf5a50a-1926-4fb6-a1fe-39ba5eb2560f
feature: Web Personalization
TQID: 'https://experienceleague.adobe.com/YDr1WsoffJR07q6pyCNZt2zU1dtgYUueaIae-aW2qj4'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
    internal-label: Personalization
  - id: 664d862c-1673-5ed4-a3d6-386ac83225e4
    internal-label: Web Personalization
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 85%
---
# ログインとユーザー管理 {#login-and-user-management}

## [!UICONTROL Web パーソナライゼーション]ユーザーロールの作成 {#create-a-web-personalization-user-role}

1. **[!UICONTROL 管理者]**&#x200B;セクションに移動して、「**[!UICONTROL ユーザーと役割]**」をクリックします。

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. 「**[!UICONTROL 役割]**」をクリックします。

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >Web Personalization（WP）のユーザーロールが既に存在する場合は、手順4に示すように設定されていることを確認します。

1. 「**[!UICONTROL 新しいロール]**」をクリックします。

   ![](assets/three-1.png)

1. [!UICONTROL ロール名]を入力し、「[!UICONTROL 権限]」を選択します。 「**[!UICONTROL 作成]**」をクリックします（この役割は[すべてのワークスペースに適用](/help/marketo/product-docs/administration/users-and-roles/edit-user-workspaces.md)されます）。

   ![](assets/four.png)

   >[!TIP]
   >
   >ターゲティングとパーソナライズ機能のすべての項目に対するアクセス権をユーザーに与えるには、必ず&#x200B;_すべて_&#x200B;のチェックボックスを選択します。

## [!UICONTROL Web パーソナライゼーション]および予測コンテンツのユーザー権限 {#web-personalization-and-predictive-content-user-permissions}

**[!UICONTROL ターゲティングとパーソナライゼーション]**：この権限のみが選択されている場合、ユーザーは表示のみの権限を持ちます。

**[!UICONTROL Web パーソナライゼーションと予測の管理]**：ユーザーは、web パーソナライゼーションおよび予測コンテンツアプリのアカウント設定とコンテンツ設定にのみアクセスできます。 ユーザーはアプリ内のページを表示できますが、作成、編集、削除、起動の権限はありません。

**[!UICONTROL 予測コンテンツエディター]**：ユーザーは予測コンテンツアプリにエディターアクセスできます。 権限を使用して、コンテンツを作成、編集、削除できます。 Web やメールでの予測用にコンテンツを有効にすることはできません。

**[!UICONTROL 予測コンテンツランチャー]**：ユーザーは、アカウントとコンテンツの設定を除く、すべての予測コンテンツ機能にアクセスできます。 この権限を使用して、コンテンツの作成、編集、削除、有効化をおこなうことができます。

**[!UICONTROL Web キャンペーンエディター]**：ユーザーは、すべての web パーソナライゼーションに対してエディターアクセス権を持ち、web キャンペーンの作成、編集および削除は行うことができますが、web キャンペーンを起動することはできません。

**[!UICONTROL Web キャンペーンランチャー]**：ユーザーは、アカウントとコンテンツの設定を除く、すべての web パーソナライゼーションアプリ機能にアクセスできます。 この権限を使用して、web キャンペーンの作成、編集、削除、およびローンチを行うことができます。

## WP ロールをユーザーに割り当てる {#assign-wp-role-to-user}

1. **[!UICONTROL ユーザー]**&#x200B;に移動します。

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. WP アクセスを許可するユーザーを選択し、「**[!UICONTROL ユーザーを編集]**」をクリックします。

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. すべてのワークスペースの WP ユーザーロールを選択します。

   ![](assets/seven.png)

1. 新しく有効にしたユーザが次回ログインすると、My Marketo に **[!UICONTROL Web パーソナライゼーション]**&#x200B;タイルが表示されます。

   ![](assets/eight.png)
