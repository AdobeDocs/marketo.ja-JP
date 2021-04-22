---
description: オンプレム用Microsoft Dynamics CRMアプリのセットアップ —Marketoドキュメント — 製品ドキュメント
title: オンプレミス用Microsoft Dynamics CRMアプリのセットアップ
exl-id: 50d41d0a-0c3b-43b8-8117-d91903e74699
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# オンプレム用Microsoft Dynamics CRMアプリのセットアップ{#set-up-microsoft-dynamics-crm-app-for-on-prem}

MarketoのクライアントID/クライアントシークレットベースのセットアップは、AD FSを使用したオンプレムで実行できます(ver. 2016以降)。 古いバージョンのOn-premについては、[Marketoサポート](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせの上、ユーザーIDとパスワードのみに基づいて認証方法が変更されたことをご確認ください。

## Microsoft Dynamics CRMアプリ{#set-up-microsoft-dynamics-crm-app}のセットアップ

[このMicrosoft記事](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later)の手順に従います。

完了したら、次の手順は&#x200B;**Dynamics CRMで生成されたクライアントIDとシークレットをMarketo**&#x200B;に入力します。

## Dynamics CRMで生成されたクライアントIDとシークレットをMarketoに入力{#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}

次の手順は、オンラインバージョンとオンプレムバージョンに適用されます。

1. Marketoで、**管理者**&#x200B;をクリックします。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-1.png)

1. **Microsoft Dynamics**&#x200B;をクリックします。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-2.png)

1. 「**同期を無効にする**」をクリックします。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-3.png)

1. 「資格情報」の横の「**編集**」をクリックします。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-4.png)

1. 以前に取得した&#x200B;**クライアントID**&#x200B;と&#x200B;**クライアントシークレット**&#x200B;を入力し、**保存**&#x200B;を押します。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-5.png)

1. 「**同期設定を検証**」をクリックします。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-6.png)

1. 「**次へ**」をクリックします。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-7.png)

1. すべての緑のチェックマークが表示されます。 「**閉じる**」をクリックします。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-8.png)

   >[!NOTE]
   >
   >緑のチェックマークの中に赤いX印が表示される場合は、[この記事](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)で修正オプションを参照してください。

1. 「**同期を有効にする**」をクリックします。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-9.png)

それだ！
