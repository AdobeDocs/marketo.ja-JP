---
unique-page-id: 7504739
description: Marketo for Dynamics 2015オンプレミスおよび2016 365オンプレミステップ2 / 3 - Marketoドキュメント — 製品ドキュメント
title: Marketo for Dynamics 2015オンプレミスおよび2016 365オンプレミスステップ2 / 3をインストール
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
source-git-commit: 5473e1a78769ba23e9c3a5926407cf42ef9685a0
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# 手順2 / 3 Dynamics用のMarketoのセットアップ（2015オンプレミスおよび2016 365オンプレミス）{#step-of-set-up-for-marketo-on-premises-and-365}

前の手順を完了しているすばらしいジョブ。 これからも続けよう。

>[!PREREQUISITES]
[Marketo for Dynamics 2015オンプレミスおよび2016 365オンプレミスステップ1 / 3をインストール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)>
>

## 同期ユーザーロール{#assign-sync-user-role}の割り当て

Marketo同期ユーザーの役割をMarketo同期ユーザーにのみ割り当てます。 他のユーザーに割り当てる必要はありません。

>[!NOTE]
これは、Marketoバージョン4.0.0.14以降に適用されます。 以前のバージョンでは、すべてのユーザーに同期ユーザーの役割が必要です。 Marketoをアップグレードするには、[Microsoft Dynamics用Marketoソリューションのアップグレード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)を参照してください。

>[!IMPORTANT]
Sync User [の言語設定は、英語](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us)に設定する必要があります。

1. 「**設定**」で、「**セキュリティ**」をクリックします。

   ![](assets/assign1.png)

1. 「**ユーザー**」をクリックします。

   ![](assets/assign2.png)

1. ここにユーザーのリストが表示されます。 専用のMarketo Syncユーザーを選択するか、[Active Directoryフェデレーションサービス](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS)管理者に問い合わせて、Marketo用の専用ユーザーを作成してください。

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 同期ユーザーを選択します。 「**役割の管理**」をクリックします。

   ![](assets/assign4.png)

   「 Marketo Sync User 」をオンにし、「 OK 」をクリックします。

   ![](assets/assign5.png)

   >[!TIP]
   役割が表示されない場合は、[手順1/3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)に戻り、ソリューションをインポートします。

   >[!NOTE]
   同期ユーザーがCRMでおこなった更新は、Marketoに&#x200B;**同期されません**。

## Marketoソリューションの設定{#configure-marketo-solution}

もう少しで終わりだ！ 次の記事に進む前に、設定の最後の部分がいくつかあります。

1. 「**設定**」で、「**Marketo Config**」をクリックします。

   ![](assets/configure1.png)

   >[!NOTE]
   Marketo Configが見つからない場合は、ページを更新してみてください。 問題が解決しない場合は、[Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)を公開するか、ログアウトしてから再度ログインしてみます。

1. 「**デフォルト**」をクリックします。

   ![](assets/configure2.png)

1. 「**Marketoユーザー**」フィールドをクリックし、同期ユーザーを選択します。

   ![](assets/configure3.png)

1. 右下隅の保存アイコンをクリックします。

   ![](assets/configure4.png)

1. 「**すべてのカスタマイズを公開**」をクリックします。

   ![](assets/publish-all-customizations1.png)

## 手順3に進む前に{#before-proceeding-to-step}

* 同期するレコードの数を制限する場合は、[カスタム同期フィルター](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)を今すぐ設定します。
* [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)の検証プロセスを実行します。 初期設定が正しく行われたことを確認します。
* Microsoft Dynamics CRMでMarketo同期ユーザーにログインします。

>[!MORELIKETHIS]
[Marketo for Dynamics 2015オンプレミスおよび2016 365オンプレミスステップ3 / 3をインストール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
