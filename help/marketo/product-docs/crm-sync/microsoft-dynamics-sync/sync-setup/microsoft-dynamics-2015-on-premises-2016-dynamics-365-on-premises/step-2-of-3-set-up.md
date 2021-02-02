---
unique-page-id: 7504739
description: Marketo for Dynamics 2015オンプレムおよび2016 365オンプレムステップ2 / 3 - Marketto Docs — 製品ドキュメントのインストール
title: Marketo for Dynamics 2015オンプレムおよび2016 365オンプレムのインストール手順2/3
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---


# 手順2 / 3 Dynamics用のMarketoの設定（2015オンプレムおよび2016 365オンプレム）{#step-of-set-up-for-marketo-on-premises-and-365}

優れたジョブが前の手順を完了しています。 これからも続けていこう。

>[!PREREQUISITES]
>
>[Marketo for Dynamics 2015オンプレムおよび2016 365オンプレムのインストール手順1/3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## 同期ユーザーロールの割り当て{#assign-sync-user-role}

Marketor SyncユーザーロールをMarketor Syncユーザーにのみ割り当てます。 他のユーザーに割り当てる必要はありません。

>[!NOTE]
>
>これは、Marketoバージョン4.0.0.14以降に適用されます。 以前のバージョンでは、すべてのユーザーに同期ユーザーの役割が必要です。 Marketorをアップグレードするには、[Marketo Solution for Microsoft Dynamicsのアップグレード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/upgrade-the-marketo-solution-for-microsoft-dynamics.md)を参照してください。

1. 「**設定**」で、「**セキュリティ**」をクリックします。

   ![](assets/assign1.png)

1. 「**ユーザー**」をクリックします。

   ![](assets/assign2.png)

1. ここでは、ユーザーのリストが表示されます。 専用のMarketo Syncユーザーを選択するか、[Active Directoryフェデレーションサービス](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS)管理者に連絡して、Marketo用の専用ユーザーを作成してください。

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 同期ユーザーを選択します。 「**ロールの管理**」をクリックします。

   ![](assets/assign4.png)

   「ユーザーを同期するマーケティングツール」を選択し、「OK」をクリックします。

   ![](assets/assign5.png)

   >[!TIP]
   >
   >ロールが表示されない場合は、[手順1/3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)に戻り、ソリューションをインポートします。

   >[!NOTE]
   >
   >同期ユーザーがCRMで行った更新は、Marketoに&#x200B;**同期**&#x200B;されません。

## Marketto Solutionの設定{#configure-marketo-solution}

もう少しで終わりだ！ 次の記事に移る前に、最後の設定をいくつか示します。

1. 「**設定**」で、「**マーケティング先設定**」をクリックします。

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Marketor Configがない場合は、ページを更新してみてください。 問題が解決しない場合は、[Marketor Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)を公開するか、ログアウトしてから再度ログインしてみてください。

1. 「**デフォルト**」をクリックします。

   ![](assets/configure2.png)

1. 「**Marketto User**」フィールドをクリックし、同期ユーザーを選択します。

   ![](assets/configure3.png)

1. 右下隅の保存アイコンをクリックします。

   ![](assets/configure4.png)

1. 「**すべてのカスタマイズを発行**」をクリックします。

   ![](assets/publish-all-customizations1.png)

## 手順3に進む前に{#before-proceeding-to-step}

* 同期するレコード数を制限する場合は、[カスタムの同期フィルタ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)を設定します。
* [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)の検証プロセスを実行します。 初期設定が正しく行われたことを確認できます。
* Microsoft Dynamics CRMのMarketo Sync Userにログインします。

>[!MORELIKETHIS]
>
>[Marketo for Dynamics 2015オンプレムおよび2016 365オンプレムのインストール手順3/3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
