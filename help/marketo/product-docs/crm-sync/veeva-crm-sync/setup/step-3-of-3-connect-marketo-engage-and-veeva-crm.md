---
description: 手順 3 / 3 - Marketo Engage と Veeva CRM の接続 - Marketo ドキュメント - 製品ドキュメント
title: 手順 3/3 - Marketo Engage と Veeva CRM の接続
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
feature: Veeva CRM
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 85%

---

# 手順 3/3：Marketo Engage と Veeva CRM の接続 {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

この記事では、設定済みの Veeva CRM インスタンスと同期するように Marketo を設定します。Veeva CRM は Salesforce プラットフォーム上に構築されているので、**ポップアップに Salesforce が表示されます**。

>[!PREREQUISITES]
>
>* [ 手順 1/3:Veeva へのMarketo フィールドの追加 ](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}
>* [ 手順 2/3:Veeva Marketo ユーザーを作成する ](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target="_blank"}

>[!IMPORTANT]
>
>一度に Veeva CRM インスタンスに接続できる Marketo インスタンスは 1 つだけです。

## OAuth を使用して Veeva CRM に接続 {#connect-to-veeva-crm-using-oauth}

1. Marketo で、「**[!UICONTROL 管理者]**」をクリックします。「**[!UICONTROL CRM]**」を選択し、「**[!UICONTROL Veeva と同期]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >「フィールドを同期」をクリックする前に、Marketoで同期ユーザーから必ず [ 必要のないすべてのフィールドを非表示 ](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} にしてください。 「同期フィールド」をクリックすると、ユーザが表示できるすべてのフィールドが Marketo に作成され、削除できなくなります。

1. 「**[!UICONTROL Veeva でログイン]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >Marketo サンドボックスを Veeva CRM サンドボックスに同期する場合は、「サンドボックス」をオンにします。

1. 「**[!UICONTROL 資格情報を確認]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. Salesforce ログインページのポップアップが表示されます。「Marketo Sync User」の認証情報を入力し、「**[!UICONTROL ログイン]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. メールで受け取った検証コード（Salesforce から送信）を入力し、**[!UICONTROL 検証]**&#x200B;をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. 検証が成功すると、アクセスをリクエストするアクセスページが表示されいます。「**[!UICONTROL 許可]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. 数分後に、Marketo Engage にポップアップが表示されます。「**[!UICONTROL 資格情報を確認]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## Veeva 同期を開始 {#start-veeva-sync}

1. 「**[!UICONTROL Veeva 同期を開始]**」をクリックして、Marketo と Veeva CRM 間の永続的な同期を開始します。

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >Marketo は、Veeva CRM の同期や、リードを手動で入力した場合には、自動的に重複排除を行いません。

1. 「**[!UICONTROL 同期の開始]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>最初の同期が完了するまでの時間は、データベースのサイズと複雑さによって異なります。

## 同期の検証 {#verify-sync}

Marketo の「管理」領域に、Veeva CRM 同期に関するステータスメッセージが表示されます。次の手順に従うことで、同期が正しく機能していることを確認できます。

1. Marketo で、「**[!UICONTROL 管理]**」をクリックして、「**[!UICONTROL Veeva]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. 同期ステータスは、右上隅に表示されます。最終同期、同期が進行しています、失敗のいずれかのメッセージが表示されます。

>[!MORELIKETHIS]
>
>[ カスタムオブジェクトの設定 ](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}
