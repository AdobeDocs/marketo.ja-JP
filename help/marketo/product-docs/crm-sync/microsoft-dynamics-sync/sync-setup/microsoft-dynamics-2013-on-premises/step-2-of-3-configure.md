---
unique-page-id: 3571816
description: 手順2/3 -Marketo用の同期ユーザーの設定（2013オンプレミス） -Marketoドキュメント — 製品ドキュメント
title: 手順2/3 -Marketoの同期ユーザーを構成(2013 On-Premises)
exl-id: 27c4407e-0623-4ae0-8aa1-0b28c6c5c4f8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# 手順2/3:Marketo(2013 On-Premises)の同期ユーザーの構成{#step-of-configure-sync-user-for-marketo-on-premises}

前の手順を完了した素晴らしい作業を続けます。

>[!PREREQUISITES]
>
>[手順1/3:DynamicsでのMarketoソリューションのインストール（2013オンプレミス）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)

## 同期ユーザーロールの割り当て{#assign-sync-user-role}

Marketo同期ユーザーロールをMarketo同期ユーザーにのみ割り当てます。 他のユーザーに割り当てる必要はありません。

>[!NOTE]
>
>これは、Marketoプラグインバージョン4.0.0.14以降に適用されます。 以前のバージョンでは、すべてのユーザーに同期ユーザーの役割が必要です。 Marketoをアップグレードするには、[Microsoft Dynamics用Marketoソリューションのアップグレード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)を参照してください。

1. 「**設定**」で、「**管理**」をクリックします。

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. 「**ユーザー**」を選択します。

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. ここでは、ユーザーのリストが表示されます。 専用のMarketo同期ユーザーを選択するか、[Active Directoryフェデレーションサービス(AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [管理者に問い合わせて、Marketo専用の新しいユーザーを作成してください。](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 同期ユーザーを選択します。 ![](assets/image2015-3-26-11-3a16-3a22.png)をクリックし、**ロールの管理**&#x200B;を選択します

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. 「**Marketo同期ユーザー**」をチェックし、「**OK**」をクリックします。

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >ロールが表示されない場合は、[手順1/3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)に戻り、ソリューションをインポートします。

   >[!NOTE]
   >
   >同期ユーザーがCRMで行った更新は、**** Marketoには同期されません。

## Marketoソリューションの構成{#configure-marketo-solution}

もう少しで終わりだ！ 次の記事に移る前に、最後の設定をいくつか示します。

1. 「**設定**」で、「**Marketo設定**」をクリックします。

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >**Marketo設定**&#x200B;が見つからない場合は、ページを更新してみてください。 問題が解決しない場合は、[Marketoソリューション](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)を再度発行するか、ログアウトしてから再度ログインしてみてください。

1. 「**デフォルト**」をクリックします。

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. 「**Marketoユーザー**」フィールドをクリックし、同期ユーザーを選択します。

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. 右下の![](assets/image2015-3-13-15-3a10-3a11.png)をクリックして、変更を保存します。

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. 「**すべてのカスタマイズを発行**」をクリックします。

   ![](assets/publish-all-customizations1.png)

## 手順3に進む前に{#before-proceeding-to-step}

* 同期するレコード数を制限する場合は、[カスタムの同期フィルタ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)を設定します。
* [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)の検証プロセスを実行します。 初期設定が正しく行われたことを確認できます。
* Microsoft Dynamics CRMのMarketo同期ユーザーにログインします。

OK！

>[!MORELIKETHIS]
>
>[手順3/3:Marketoとダイナミクスの接続（2013オンプレミス）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-3-of-3-connect.md)
