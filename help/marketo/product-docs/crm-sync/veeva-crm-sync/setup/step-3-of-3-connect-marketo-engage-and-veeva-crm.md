---
description: 最終的な設定手順で、Marketo Engageを Veeva CRM に接続する方法を説明します。 OAuth、認証情報を確認、同期の各フィールドを設定し、接続を完了します。
title: 手順 3／3 - Marketo Engage と  [!DNL Veeva]  CRM の接続
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
feature: Veeva CRM
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 92%

---

# 手順 3／3：Marketo Engage と [!DNL Veeva] CRM の接続 {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

この記事では、設定済みの [!DNL Veeva] CRM インスタンスと同期するように Marketo を設定します。[!DNL Veeva] CRM は [!DNL Salesforce] プラットフォーム上に構築されているので、**ポップアップに [!DNL Salesforce] が表示されます**。

>[!PREREQUISITES]
>
>* [手順 1／3：Marketo フィールドの  [!DNL Veeva]](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"} への追加
>* [手順 2／3：Marketo 用の  [!DNL Veeva]  ユーザの作成](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target="_blank"}

>[!IMPORTANT]
>
>一度に [!DNL Veeva] CRM インスタンスに接続できる Marketo インスタンスは 1 つだけです。

## OAuth を使用して [!DNL Veeva] CRM に接続 {#connect-to-veeva-crm-using-oauth}

1. Marketo で、「**[!UICONTROL 管理者]**」をクリックします。「**[!UICONTROL CRM]**」を選択し、「**[!UICONTROL Veeva と同期]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >同期ユーザから Marketo で[不要なフィールドをすべて非表示](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"}にした後で、「同期フィールド」をクリックするようにしてください。「同期フィールド」をクリックすると、ユーザが表示できるすべてのフィールドが Marketo に作成され、削除できなくなります。

1. 「**[!UICONTROL Veeva でログイン]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >Marketo サンドボックスを [!DNL Veeva] CRM サンドボックスに同期する場合は、「[!UICONTROL サンドボックス]」をオンにします。

1. 「**[!UICONTROL 資格情報を確認]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. [!DNL Salesforce] ログインページのポップアップが表示されます。「Marketo 同期ユーザ」資格情報を入力し、「**[!UICONTROL ログイン]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. メールで受け取った検証コード（[!DNL Salesforce] から送信）を入力し、「**[!UICONTROL 検証]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. 検証が成功すると、アクセスをリクエストするアクセスページが表示されいます。「**[!UICONTROL 許可]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. 数分後に、Marketo Engage にポップアップが表示されます。「**[!UICONTROL 資格情報を確認]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## [!DNL Veeva] 同期の開始 {#start-veeva-sync}

1. 「**[!UICONTROL Veeva 同期を開始]**」をクリックして、[!DNL Marketo-Veeva] CRM 間の永続的な同期を開始します。

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >Marketo は、[!DNL Veeva] CRM の同期や、リードを手動で入力した場合には、自動的に重複排除を行いません。

1. 「**[!UICONTROL 同期の開始]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>最初の同期が完了するまでの時間は、データベースのサイズと複雑さによって異なります。

## 同期の検証 {#verify-sync}

Marketo の「管理」領域に、[!DNL Veeva] CRM 同期に関するステータスメッセージが表示されます。次の手順に従うことで、同期が正しく機能していることを確認できます。

1. Marketo で、「**[!UICONTROL 管理]**」をクリックして、「**[!UICONTROL Veeva]**」をクリックします。

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. 同期ステータスは、右上隅に表示されます。最終同期、同期が進行しています、失敗のいずれかのメッセージが表示されます。

>[!MORELIKETHIS]
>
>[カスタムオブジェクトを設定](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}
