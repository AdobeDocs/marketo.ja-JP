---
unique-page-id: 3571807
description: 手順2 / 3 - Dynamics (2011 On-Premises)のMarketo同期ユーザーを設定する — Marketto Docs — 製品ドキュメント
title: 手順2 / 3 - DynamicsでのMarketo Syncユーザーの設定(2011 On-Premises)
translation-type: tm+mt
source-git-commit: 309f299275bfe75e8af0150be0a5ffdf28a54cf8
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---


# 手順2/3:Dynamics (2011 On-Premises)のMarketo Syncユーザーを設定{#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

前の手順を完了した素晴らしい作業を続けます。

>[!PREREQUISITES]
>
>* [手順1/3:Marketo Solution(2011 On-Premises)のインストール](step-1-of-3-install.md)

>



## 同期ユーザーロールの割り当て{#assign-sync-user-role}

Marketor SyncユーザーロールをMarketor Syncユーザーにのみ割り当てます。 他のユーザーに割り当てる必要はありません。

>[!NOTE]
>
>これは、Marketoプラグインバージョン4.0.0.14以降に適用されます。 以前のバージョンでは、すべてのユーザーに同期ユーザーの役割が必要です。 Marketorをアップグレードするには、[Marketo Solution for Microsoft Dynamicsのアップグレード](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/upgrade-the-marketo-solution-for-microsoft-dynamics.md)を参照してください。

1. 左下のメニューで、「**設定**」を選択します。

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. ツリーで、「**管理**」を選択します。

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. 「**ユーザー**」を選択します。

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. ここでは、ユーザーのリストが表示されます。 ユーザーを同期する専用のマーケティング担当者を選択するか、[Active Directoryフェデレーションサービス(AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx)管理者に問い合わせて、Marketor専用の新しいユーザーを作成します。 「**ロールの管理**」をクリックします。

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. 「**ユーザーを同期するマーケティングツール**」を選択し、「**OK**」をクリックします。

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >ロールが表示されない場合は、[手順1/3](step-1-of-3-install.md)に戻り、ソリューションをインポートします。

   >[!NOTE]
   >
   >同期ユーザーがCRMで行った更新は、Marketoに&#x200B;**同期**&#x200B;されません。

## Marketto Solutionの設定{#configure-marketo-solution}

もう少しで終わりだ！ 次の記事に移る前に、最後の設定をいくつか示します。

1. **設定**&#x200B;を選択します。 次に、ツリーで「**Marketto Config **」を選択します。

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Marketor Configがない場合は、ページを更新してみてください。 問題が解決しない場合は、[Marketorソリューションを再度](step-1-of-3-install.md)発行するか、ログアウトしてから再度ログインします。

1. 「**デフォルト**」をクリックします。

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. ![](assets/image2015-4-2-14-3a29-3a1.png)をクリック

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. ポップアップで、同期ユーザーを選択します。 次に、「**OK**」をクリックします。

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. 「**保存**」をクリックして変更を保存します。

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. 「**すべてのカスタマイズを発行**」をクリックします。

   ![](assets/publish-all-customizations1.png)

## 手順3に進む前に{#before-proceeding-to-step}

    *同期するレコードの数を制限する場合は、[カスタム同期フィルタを設定](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)を今すぐ行ってください。
    * [Microsoft Dynamics Syncの検証](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)プロセスを実行します。初期設定が正しく行われたことを確認できます。
    * Microsoft Dynamics CRMのMarketto Sync Userにログインします。

素晴らしい仕事！

>[!NOTE]
>
>**関連記事**
>
>[手順3/3:Microsoft DynamicsとMarketoの接続（2011オンプレミス）](step-3-of-3-connect.md)

