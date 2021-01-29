---
unique-page-id: 3571816
description: 手順2/3 - Marketo用の同期ユーザーの設定（2013オンプレミス） - Marketto Docs — 製品ドキュメント
title: 手順2/3 - Marketto用の同期ユーザーの設定(2013 On-Premises)
translation-type: tm+mt
source-git-commit: 309f299275bfe75e8af0150be0a5ffdf28a54cf8
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---


# 手順2/3:Marketor (2013 On-Premises)用の同期ユーザーの構成{#step-of-configure-sync-user-for-marketo-on-premises}

前の手順を完了した素晴らしい作業を続けます。

>[!PREREQUISITES]
>
>* [手順1/3:Dynamics(2013 On-Premises)にMarketo Solutionをインストールする](step-1-of-3-install.md)


## 同期ユーザーロールの割り当て{#assign-sync-user-role}

Marketor SyncユーザーロールをMarketor Syncユーザーにのみ割り当てます。 他のユーザーに割り当てる必要はありません。

>[!NOTE]
>
>これは、Marketoプラグインバージョン4.0.0.14以降に適用されます。 以前のバージョンでは、すべてのユーザーに同期ユーザーの役割が必要です。 Marketorをアップグレードするには、[Marketo Solution for Microsoft Dynamicsのアップグレード](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/upgrade-the-marketo-solution-for-microsoft-dynamics.md)を参照してください。

1. 「**設定**」で、「**管理**」をクリックします。

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. 「**ユーザー**」を選択します。

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. ここでは、ユーザーのリストが表示されます。 専用のMarketo Syncユーザーを選択するか、[Active Directoryフェデレーションサービス(AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [管理者に問い合わせて、Marketor専用の新しいユーザーを作成します。](http://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 同期ユーザーを選択します。 ![](assets/image2015-3-26-11-3a16-3a22.png)をクリックし、「**ロールの管理**」を選択します

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. 「**ユーザーを同期するマーケティングツール**」を選択し、「**OK**」をクリックします。

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >ロールが表示されない場合は、[手順1/3](step-1-of-3-install.md)に戻り、ソリューションをインポートします。

   >[!NOTE]
   >
   >同期ユーザーがCRMで行った更新は、Marketoに&#x200B;**同期**&#x200B;されません。

## Marketto Solutionの設定{#configure-marketo-solution}

もう少しで終わりだ！ 次の記事に移る前に、最後の設定をいくつか示します。

1. 「**設定**」で、「**マーケティング先設定**」をクリックします。

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >**Marketto Config**&#x200B;がない場合は、ページを更新してみてください。 問題が解決しない場合は、[Marketoソリューション](https://docs.marketo.com/pages/viewpage.action?pageId=3571813#Step1of3:InstalltheMarketoSolutioninDynamics(2013On-Premises)-PublishAllCustomizations)を再度公開するか、ログアウトしてから再度ログインしてみてください。

1. 「**デフォルト**」をクリックします。

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. 「**Marketto User**」フィールドをクリックし、同期ユーザーを選択します。

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. 右下の![](assets/image2015-3-13-15-3a10-3a11.png)をクリックして、変更を保存します。

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. 「**すべてのカスタマイズを発行**」をクリックします。

   ![](assets/publish-all-customizations1.png)

## 手順3に進む前に{#before-proceeding-to-step}

* 同期するレコード数を制限する場合は、[カスタムの同期フィルタ](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)を設定します。
* [Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)の検証プロセスを実行します。 初期設定が正しく行われたことを確認できます。
* Microsoft Dynamics CRMのMarketto Sync Userにログインします。

素晴らしい仕事！

>[!NOTE]
>
>**関連記事**
>
>* [手順3/3:MarketoとDynamicsの接続(2013 On-Premises)](step-3-of-3-connect.md)

