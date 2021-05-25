---
unique-page-id: 3571807
description: 手順2 / 3 - DynamicsでのMarketo Syncユーザーのセットアップ（2011オンプレミス） - Marketoドキュメント — 製品ドキュメント
title: 手順2 / 3 - DynamicsでのMarketo Syncユーザーのセットアップ（2011オンプレミス）
exl-id: 807c8902-24a6-48b6-a5c9-96a72764fdef
source-git-commit: 5473e1a78769ba23e9c3a5926407cf42ef9685a0
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# 手順2 / 3:Dynamics (2011 On-Premises)でのMarketo Syncユーザーのセットアップ{#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

前述の手順を完了した素晴らしい仕事は、この作業を続けます。

>[!PREREQUISITES]
[手順1/3:Marketo Solution（2011年オンプレミス版）のインストール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)>
>

## 同期ユーザーロール{#assign-sync-user-role}の割り当て

Marketo同期ユーザーの役割をMarketo同期ユーザーにのみ割り当てます。 他のユーザーに割り当てる必要はありません。

>[!NOTE]
これは、Marketoプラグインバージョン4.0.0.14以降に適用されます。 以前のバージョンでは、すべてのユーザーに同期ユーザーの役割が必要です。 Marketoをアップグレードするには、「[Microsoft Dynamics用Marketoソリューションのアップグレード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)」を参照してください。

>[!IMPORTANT]
Sync User [の言語設定は、英語](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us)に設定する必要があります。

1. 左下のメニューで、「**設定**」を選択します。

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. ツリーで、「**管理**」を選択します。

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. 「**ユーザー**」を選択します。

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. ここにユーザーのリストが表示されます。 専用のMarketo同期ユーザーを選択するか、[Active Directoryフェデレーションサービス(AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx)管理者に問い合わせて、Marketo専用の新しいユーザーを作成してもらいます。 「**役割の管理**」をクリックします。

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. 「**Marketo同期ユーザー**」をオンにし、「**OK**」をクリックします。

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   役割が表示されない場合は、[手順1/3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)に戻り、ソリューションをインポートします。

   >[!NOTE]
   同期ユーザーがCRMでおこなった更新は、Marketoに&#x200B;**同期されません**。

## Marketoソリューションの設定{#configure-marketo-solution}

もう少しで終わりだ！ 次の記事に進む前に、設定の最後の部分がいくつかあります。

1. **設定**&#x200B;を選択します。 次に、ツリーで&#x200B;**Marketo Config**&#x200B;を選択します。

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   Marketo Configが見つからない場合は、ページを更新してみてください。 問題が解決しない場合は、[Marketoソリューションを再度公開するか、ログアウトしてから再度ログインします。](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)

1. 「**デフォルト**」をクリックします。

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. ![](assets/image2015-4-2-14-3a29-3a1.png)をクリックします。

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. ポップアップで、同期ユーザーを選択します。 次に、「**OK**」をクリックします。

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. 「**保存**」をクリックして変更を保存します。

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. 「**すべてのカスタマイズを公開**」をクリックします。

   ![](assets/publish-all-customizations1.png)

## 手順3に進む前に{#before-proceeding-to-step}

    *同期するレコードの数を制限する場合は、[カスタム同期フィルターを設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)を今すぐお使いください。
    * [Microsoft Dynamics Syncの検証](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)プロセスを実行します。初期設定が正しく行われたことを確認します。
    * Microsoft Dynamics CRMでMarketo同期ユーザーにログインします。

OK！

>[!MORELIKETHIS]
[手順3/3:Microsoft DynamicsとMarketo（2011オンプレミス）の接続](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-3-of-3-connect.md)
