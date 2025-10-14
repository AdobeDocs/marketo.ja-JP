---
description: 手順 3/3 - Marketo Engageと CRM の接続  [!DNL Veeva] Marketo ドキュメント – 製品ドキュメント
title: 手順 3/3 - Marketo Engageと CRM [!DNL Veeva]  接続
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 42%

---

# 手順 3/3:Marketo Engageと [!DNL Veeva] CRM の接続 {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

この記事では、設定済みの [!DNL Veeva] CRM インスタンスと同期するようにMarketo Engageを設定します。 **CRM は [!DNL Salesforce] プラットフォーム上に構築されているので** 一部のポップアップ [!DNL Veeva] は [!DNL Salesforce] が表示されます。

>[!PREREQUISITES]
>
>* [&#x200B; 手順 1/3：へのMarketo フィールドの追加  [!DNL Veeva]](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}
>* [&#x200B; 手順 2/3:Marketoのユ  [!DNL Veeva]  ザーを作成する &#x200B;](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target="_blank"}

>[!IMPORTANT]
>
>[!DNL Veeva] CRM インスタンスに接続できるMarketo インスタンスは一度に 1 つだけです。

## OAuth を使用 [!DNL Veeva] た CRM への接続 {#connect-to-veeva-crm-using-oauth}

1. Marketo で、「**[!UICONTROL 管理者]**」をクリックします。「**[!UICONTROL CRM]**」を選択し、「**[!UICONTROL Veeva と同期]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >「フィールドを同期」をクリックする前に、Marketoで同期ユーザーから必ず [&#x200B; 必要のないすべてのフィールドを非表示 &#x200B;](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} にしてください。 「同期フィールド」をクリックすると、ユーザが表示できるすべてのフィールドが Marketo に作成され、削除できなくなります。

1. 「**[!UICONTROL Veeva でログイン]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >Marketo サンドボックスを [!UICONTROL &#x200B; CRM サンドボックスと同期する場合は &#x200B;] サンドボックス [!DNL Veeva] にチェックを入れます。

1. 「**[!UICONTROL 資格情報を確認]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. [!DNL Salesforce] ログインページを含むポップアップが表示されます。 「Marketo 同期ユーザ」資格情報を入力し、「**[!UICONTROL ログイン]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. 電子メールで受信した確認コード（[!DNL Salesforce] から送信）を入力し、「**[!UICONTROL 確認]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. 検証が成功すると、アクセスをリクエストするアクセスページが表示されいます。「**[!UICONTROL 許可]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. 数分後に、Marketo Engage にポップアップが表示されます。「**[!UICONTROL 資格情報を確認]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## 同期 [!DNL Veeva] 開始 {#start-veeva-sync}

1. **[!UICONTROL Veeva 同期を開始]** をクリックして、永続的な [!DNL Marketo-Veeva] CRM 同期を開始します。

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >Marketoは、[!DNL Veeva] CRM との同期やリードを手動で入力した場合に、自動的に重複排除を行いません。

1. 「**[!UICONTROL 同期の開始]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>最初の同期が完了するまでの時間は、データベースのサイズと複雑さによって異なります。

## 同期の検証 {#verify-sync}

Marketoの管理領域に、[!DNL Veeva] CRM 同期用のステータスメッセージが表示されます。 次の手順に従うことで、同期が正しく機能していることを確認できます。

1. Marketo で、「**[!UICONTROL 管理]**」をクリックして、「**[!UICONTROL Veeva]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. 同期ステータスは、右上隅に表示されます。最終同期、同期が進行しています、失敗のいずれかのメッセージが表示されます。

>[!MORELIKETHIS]
>
>[&#x200B; カスタムオブジェクトの設定 &#x200B;](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}
