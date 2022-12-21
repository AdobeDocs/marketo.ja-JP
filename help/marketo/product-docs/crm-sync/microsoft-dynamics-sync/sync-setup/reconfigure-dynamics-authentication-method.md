---
description: Dynamics 認証方法の再設定 - Marketo ドキュメント - 製品ドキュメント
title: Dynamics 認証方法の再設定
exl-id: 2bd6a992-3dfd-4e91-bec5-9fb3f7bbb840
source-git-commit: ab20d9683aa5987778970fd32793dc0f3056c84b
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 100%

---

# Dynamics 認証方法の再設定 {#reconfigure-dynamics-authentication-method}

次の手順に従って、Dynamics 認証方法を更新します。

>[!PREREQUISITES]
>
>次の記事のいずれかで、目的の認証方法を使用して、Microsoft Dynamics および Active Directory（Azure AD/ADFS）でアプリケーションを設定します。
>
>* [手順 2 / 3：サーバー間接続を使用した Marketo ソリューションの設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md)
>* [手順 2 / 4：リソース所有者のパスワード制御接続を使用した Marketo ソリューションの設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)


1. Marketo で「**管理者**」をクリックします。

   ![](assets/reconfigure-dynamics-authentication-method-1.png)

1. 「**Microsoft Dynamics**」をクリックし、「**同期を無効にする**」をクリックします。

   ![](assets/reconfigure-dynamics-authentication-method-2.png)

   >[!NOTE]
   >
   >認証方法を更新するには、グローバル同期を一時的に無効にする必要があります。

1. 「**新しい認証方法の再設定**」タブをクリックします。

   ![](assets/reconfigure-dynamics-authentication-method-3.png)

1. 目的の新しい認証方法を選択します（この例では Web API を選択しています）。

   ![](assets/reconfigure-dynamics-authentication-method-4.png)

1. 新しい認証方法に必要な資格情報を入力し、「**検証**」をクリックします。

   ![](assets/reconfigure-dynamics-authentication-method-5.png)

   >[!NOTE]
   >
   >* 具体的なフィールドは選択した認証方法によって異なり、以前の認証方法に応じてフォームが自動的に更新されます。
   >* 以前にも同期したことがある場合、上記のフォームデータが事前入力されている場合があります。すべての資格情報を再入力し、正しい値が設定されていることを確認してください。


1. すべて問題ない場合、同期の検証ですべて緑のチェックマーク ![](assets/green-check.png) が生成されます。メッセージを確認し、「**切替**」をクリックして認証方法を更新します。

   ![](assets/reconfigure-dynamics-authentication-method-6.png)

   >[!NOTE]
   >
   >![](assets/red-x.png) が表示された場合は、その手順に問題があります。問題を特定して修正するには、[Dynamics 検証同期に対する問題の修正](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)を参照してください。次に、上記の画像のような結果になるまで同期検証手順を再実行します。

1. 「**確認**」をクリックして続行します。

   ![](assets/reconfigure-dynamics-authentication-method-7.png)

1. 再度「**確認**」をクリックします。

   ![](assets/reconfigure-dynamics-authentication-method-8.png)

1. 「**OK**」をクリックします。

   >[!IMPORTANT]
   >
   >新しい認証モードを受け入れるまでに 15 分かかります。切り替えてから 15 分待ってから、同期を再度有効にしてください。
