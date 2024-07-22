---
unique-page-id: 3571807
description: 手順 2 / 3 - Dynamics（2011 オンプレミス）での Marketo 同期ユーザーのセットアップ - Marketo ドキュメント - 製品ドキュメント
title: 手順 2 / 3 - Dynamics（2011 オンプレミス）での Marketo 同期ユーザーのセットアップ
exl-id: 807c8902-24a6-48b6-a5c9-96a72764fdef
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 90%

---

# 手順 2 / 3：Dynamics（2011 オンプレミス）での Marketo 同期ユーザーのセットアップ {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

前の手順を完了させたら、先に進みましょう。

>[!PREREQUISITES]
>
>[手順 1 / 3：Marketo ソリューション（2011 オンプレミス版）のインストール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"}

## 同期ユーザー役割を割り当てる {#assign-sync-user-role}

Marketo 同期ユーザロールを Marketo 同期ユーザにのみ割り当てます。他のユーザーに割り当てる必要はありません。

>[!NOTE]
>
>これは、Marketo プラグインバージョン 4.0.0.14 以降に当てはまります。以前のバージョンでは、すべてのユーザーに同期ユーザー役割が必要です。Marketo をアップグレードするには、[Microsoft Dynamics 用 Marketo ソリューションのアップグレード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}を参照してください。

>[!IMPORTANT]
>
>同期ユーザーの言語設定 [ 英語に設定する必要があります ](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}。

1. 左下のメニューで、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. ツリーで、「**[!UICONTROL 管理者]**」を選択します。

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. 「**[!UICONTROL ユーザー]**」を選択します。

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. ユーザーのリストが表示されます。専用のMarketo同期ユーザーを選択するか、[Active Directory フェデレーション サービス （AFDS） ](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} の管理者に連絡してMarketo専用の新しいユーザーを作成してください。 「**[!UICONTROL ロールを管理]**」をクリックします。

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. 「**[!UICONTROL Marketo 同期ユーザー]**」をクリックし、「**[!UICONTROL OK]**」をクリックします。

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >役割が表示されない場合は、[手順 1 / 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"} に戻ってソリューションをインポートします。

   >[!NOTE]
   >
   >同期ユーザが CRM で行った更新は Marketo に同期&#x200B;_されません_。

## Marketo ソリューションの設定 {#configure-marketo-solution}

あと少しで完了です。次の記事に進む前に、最後の部分を設定しましょう。

1. 「**[!UICONTROL 設定]**」を選択します。次に、ツリーで「**[!UICONTROL Marketo 設定]**」を選択します。

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Marketo 設定が見つからない場合は、ページを更新してみてください。問題が解決しない場合は、[Marketo ソリューションをもう一度公開](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"}するか、ログアウトしてから再度ログインします。

1. 「**[!UICONTROL デフォルト]**」をクリックします。

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. ![](assets/image2015-4-2-14-3a29-3a1.png) をクリックします。

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. ポップアップで、同期ユーザーを選択します。次に、「**[!UICONTROL OK]**」をクリックします。

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. 「**[!UICONTROL 保存]**」をクリックして、変更を保存します。

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. 「**[!UICONTROL すべてのカスタマイズを公開]**」をクリックします。

   ![](assets/publish-all-customizations1.png)

## 手順 3 に進む前に {#before-proceeding-to-step}

* 同期するレコード数を制限する場合は、[カスタム同期フィルターを設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"}します。
* [Microsoft Dynamics 同期を検証](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}プロセスを実行します。初期設定が正しく行われたことを確認します。
* Microsoft Dynamics CRM で Marketo 同期ユーザーにログインします。

  これで完了です。

>[!MORELIKETHIS]
>
>[手順 3 / 3：Microsoft Dynamics と Marketo（2011 オンプレミス）の接続](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2011.md){target="_blank"}
