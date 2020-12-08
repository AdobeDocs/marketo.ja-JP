---
unique-page-id: 3571816
description: 手順2/3 - Marketo用の同期ユーザーの設定（2013オンプレミス） - Marketto Docs — 製品ドキュメント
title: 手順2/3 - Marketto用の同期ユーザーの設定(2013 On-Premises)
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---


# 手順2/3:Marketor用の同期ユーザーの設定(2013 On-Premises) {#step-of-configure-sync-user-for-marketo-on-premises}

前の手順を完了した素晴らしい作業を続けます。

>[!NOTE]
>
>**前提条件**
>
>* [手順1/3:Dynamics(2013 On-Premises)にMarketo Solutionをインストールする](step-1-of-3-install.md)


## 同期ユーザーロールの割り当て {#assign-sync-user-role}

Marketor SyncユーザーロールをMarketor Syncユーザーにのみ割り当てます。 他のユーザーに割り当てる必要はありません。

>[!NOTE]
>
>これは、Marketoプラグインバージョン4.0.0.14以降に適用されます。 以前のバージョンでは、すべてのユーザーに同期ユーザーの役割が必要です。 Marketorをアップグレードするには、「Marketor Solution for Microsoft Dynamics [のアップグレード](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md)」を参照してください。

1. 「 **設定**」で、「 **管理**」をクリックします。

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. 「 **ユーザー**」を選択します。

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. ここでは、ユーザーのリストが表示されます。 専用のMarketor Syncユーザーを選択するか、 [Active Directoryフェデレーションサービス(AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx)[管理者に問い合わせて、Marketor専用の新しいユーザーを作成します。](http://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 同期ユーザーを選択します。 「ロール ![](assets/image2015-3-26-11-3a16-3a22.png)の **管理」をクリックして選択します**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. 「 **Marketto同期ユーザー** 」をオンにし、「 **OK**」をクリックします。

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >ロールが表示されない場合は、 [手順1/3に戻り、ソリューションをインポートし](step-1-of-3-install.md) ます。

   >[!NOTE]
   >
   >同期ユーザーがCRMで行った更新は、Marketorに同期され **ません** 。

## Marketing Solutionの設定 {#configure-marketo-solution}

もう少しで終わりだ！ 次の記事に移る前に、最後の設定をいくつか示します。

1. 「 **設定**」で、「 **マーケティング先設定**」をクリックします。

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >「 **Marketor Config** 」が見つからない場合は、ページを更新してみてください。 問題が解決しない場合は、Marketorソリューションを [再度公開するか](https://docs.marketo.com/pages/viewpage.action?pageId=3571813#Step1of3:InstalltheMarketoSolutioninDynamics(2013On-Premises)-PublishAllCustomizations) 、ログアウトしてから再度ログインしてみてください。

1. 「 **デフォルト**」をクリックします。

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. 「 **マーケティング先ユーザー** 」フィールドをクリックし、同期ユーザーを選択します。

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. 右下 ![](assets/image2015-3-13-15-3a10-3a11.png) のをクリックして、変更を保存します。

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. 「すべてのカスタマイズを **発行**」をクリックします。

   ![](assets/publish-all-customizations1.png)

## 手順3に進む前に {#before-proceeding-to-step}

* 同期するレコード数を制限する場合は、カスタム同期フィルタを [設定](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 。
* Microsoft Dynamics Sync [の](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) 検証プロセスを実行します。 初期設定が正しく行われたことを確認できます。
* Microsoft Dynamics CRMのMarketto Sync Userにログインします。

素晴らしい仕事！

>[!NOTE]
>
>**関連記事**
>
>* [手順3/3:MarketoとDynamicsの接続(2013 On-Premises)](step-3-of-3-connect.md)

