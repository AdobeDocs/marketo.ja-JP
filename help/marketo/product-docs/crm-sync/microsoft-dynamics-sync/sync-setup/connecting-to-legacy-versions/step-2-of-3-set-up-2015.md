---
unique-page-id: 7504739
description: Microsoft Dynamics 2015 オンプレミス向け Marketo インストール手順 2 / 3 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 2015 オンプレミス向け Marketo インストール手順 2 / 3
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 90%

---

# 手順 2 / 3 Dynamics（2015 オンプレミス）向け Marketo の設定{#step-of-set-up-for-marketo-on-premises-2015}

前の手順を完了させたら、先に進みましょう。

>[!PREREQUISITES]
>
>[Microsoft Dynamics 2015 オンプレミス向け Marketo インストール手順 1 / 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"}

## 同期ユーザのロールの割り当て {#assign-sync-user-role}

Marketo 同期ユーザロールを Marketo 同期ユーザにのみ割り当てます。他のユーザに割り当てる必要はありません。

>[!NOTE]
>
>これは、Marketo バージョン 4.0.0.14 以降に当てはまります。以前のバージョンでは、すべてのユーザに同期ユーザロールが必要です。お使いの Marketo をアップグレードするには、[Microsoft Dynamics 用 Marketo ソリューションのアップグレード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}を参照してください。

>[!IMPORTANT]
>
>同期ユーザーの言語設定 [ 英語に設定する必要があります ](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}。

1. 「**[!UICONTROL 設定]**」で、「**[!UICONTROL セキュリティ]**」をクリックします。

   ![](assets/assign1.png)

1. 「**[!UICONTROL ユーザ]**」をクリックします。

   ![](assets/assign2.png)

1. ユーザのリストが表示されます。専用のMarketo Sync ユーザーを選択するか、[Active Directory フェデレーション サービス ](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} （ADFS）の管理者に連絡してMarketo専用のユーザーを作成してください。

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 同期ユーザを選択します。「**[!UICONTROL ロールを管理]**」をクリックします。

   ![](assets/assign4.png)

1. 「Marketo 同期ユーザ」のチェックをオンにして、「**[!UICONTROL OK]**」をクリックします。

   ![](assets/assign5.png)

   >[!IMPORTANT]
   >
   >同期ユーザには、Marketo 設定に対する読み取り権限が必要です。

   >[!TIP]
   >
   >ロールが表示されない場合は、[手順 1 / 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"} に戻ってソリューションをインポートします。

   >[!NOTE]
   >
   >同期ユーザが CRM で行った更新は Marketo に同期&#x200B;_されません_。

## Marketo ソリューションの設定 {#configure-marketo-solution}

あと少しで完了です。次の記事に進む前に、最後の部分を設定しましょう。

1. 「**[!UICONTROL 設定]**」で、「**[!UICONTROL Marketo 設定]**」をクリックします。

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Marketo 設定が見つからない場合は、ページを更新してみてください。問題が解決しない場合は、、[Marketo ソリューションを公開](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"}するか、またはログアウトしてから再度ログインしてみてください。

1. 「**[!UICONTROL デフォルト]**」をクリックします。

   ![](assets/configure2.png)

1. 「**[!UICONTROL Marketo ユーザ]**」フィールドをクリックし、同期ユーザを選択します。

   ![](assets/configure3.png)

1. 右下隅の「保存」アイコンをクリックします。

   ![](assets/configure4.png)

1. 「**[!UICONTROL すべてのカスタマイズを公開]**」をクリックします。

   ![](assets/publish-all-customizations1.png)

   >[!NOTE]
   >
   >同期ユーザには、Marketo 設定に対する読み取り権限が必要です。

## 手順 3 に進む前に {#before-proceeding-to-step}

* 同期するレコード数を制限する場合は、[カスタム同期フィルターを設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"}します。
* [Microsoft Dynamics 同期を検証](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}プロセスを実行します。初期設定が正しく行われたことを確認します。
* Microsoft Dynamics CRM で、Marketo 同期ユーザにログインします。

>[!MORELIKETHIS]
>
>[Microsoft Dynamics 2015 オンプレミス向け Marketo インストール手順 3 / 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2015.md){target="_blank"}
