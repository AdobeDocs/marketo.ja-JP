---
unique-page-id: 3571827
description: 手順 2／3 - サーバー間接続を使用した Marketo ソリューションの設定 - Marketo ドキュメント - 製品ドキュメント
title: 手順 2／3 - サーバー間接続を使用した Marketo ソリューションの設定
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 100%

---

# 手順 2／3：サーバー間接続を使用した Marketo ソリューションの設定 {#step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s}

>[!PREREQUISITES]
>
>[手順 1／3 - サーバー間接続を使用した Marketo ソリューションのインストール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"}

## [!DNL Azure AD] でのクライアントアプリケーションの作成 {#create-client-application-in-azure-ad}

1. [この Microsoft 記事](https://docs.microsoft.com/ja-jp/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}にアクセスします。

1. すべての手順に従います。手順 3 で、関連するアプリケーション名（例：「[!DNL Marketo Integration]」）を入力します。「サポートされたアカウントタイプ」で、「**この組織ディレクトリのアカウントのみ**」を選択します。

1. アプリケーション ID（ClientId）とテナント ID を書き留めます。後で Marketo に入力する必要があります。

1. [この記事](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"}の手順に従って、管理者の同意を与えます。

1. 「**[!UICONTROL Certificates &amp; secrets]**」をクリックして、管理センターでクライアントシークレットを生成します。

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-1.png)

1. 「**[!UICONTROL 新規クライアントシークレット]**」ボタンをクリックします。

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-2.png)

1. クライアントシークレットの説明を追加して、「**[!UICONTROL 追加]**」をクリックします。

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-3.png)

>[!CAUTION]
>
>後で必要になるので、クライアントシークレットの値（以下のスクリーンショットを参照）を必ずメモしておきます。これは 1 回だけ表示され、再度取得することはできません。

![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-4.png)

## Microsoft でのアプリケーションユーザの作成 {#create-application-user-in-microsoft}

1. 次のリンクから、[Microsoft でのアプリケーションユーザの設定](https://docs.microsoft.com/ja-jp/powerapps/developer/common-data-service/use-single-tenant-server-server-authentication#application-user-creation){target="_blank"}手順に従います。

   >[!IMPORTANT]
   >
   >* アプリケーションユーザに権限を付与する際に、「Marketo 同期ユーザロール」に割り当てるようにします。
   >* Power Platform 上の[詳細を表示オプション](https://docs.microsoft.com/ja-jp/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user)で、アプリケーションユーザのメールアドレスをメモします。このメールアドレスは、Marketo 内で MS [!DNL Dynamics] への接続を設定する際のユーザ名として使用されます。

## [!DNL Azure AD] と [!DNL AD FS On-prem] の連携 {#azure-ad-federated-with-ad-fs-on-prem}

[!DNL Azure AD] から [!DNL ADFS Onprem] への連携では、特定のアプリケーション用に Home Realm Discovery ポリシーを作成する必要があります。このポリシーを使用すると、[!DNL Azure AD] は認証リクエストをフェデレーションサービスにリダイレクトします。このためには、[!DNL AD Connect] でパスワードハッシュの同期を有効にする必要があります。詳しくは、 [!DNL ROPC] による [[!DNL OAuth] ](https://docs.microsoft.com/ja-jp/azure/active-directory/develop/v2-oauth-ropc) および[アプリケーション用の HRD ポリシーの設定](https://docs.microsoft.com/ja-jp/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application)を参照してください。

その他のリファレンスについて詳しくは、[こちら](https://docs.microsoft.com/ja-jp/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=%E5%AF%BE%E8%A9%B1%E5%9E%8B%E3%83%A6%E3%83%BC%E3%82%B6%E3%83%BC%20%E3%82%B5%E3%82%A4%E3%83%B3%E3%82%A4%E3%83%B3%E3%81%AF%E3%80%81%E3%83%A6%E3%83%BC%E3%82%B6%E3%83%BC%E3%81%8C%20Azure%20AD%20%E3%81%AB%E8%AA%8D%E8%A8%BC%E8%A6%81%E7%B4%A0%E3%82%92%E6%8F%90%E4%BE%9B%E3%81%99%E3%82%8B%E3%81%8B%E3%80%81Azure%20AD%20%E3%81%BE%E3%81%9F%E3%81%AF%E3%83%98%E3%83%AB%E3%83%91%E3%83%BC%20%E3%82%A2%E3%83%97%E3%83%AA%20%28Microsoft%20Authenticator%20%E3%82%A2%E3%83%97%E3%83%AA%E3%81%AA%E3%81%A9%29%20%E3%81%A8%E7%9B%B4%E6%8E%A5%E3%82%84%E3%82%8A%E5%8F%96%E3%82%8A%E3%81%99%E3%82%8B%E3%82%B5%E3%82%A4%E3%83%B3%E3%82%A4%E3%83%B3%E3%81%A7%E3%81%99%E3%80%82&text=%E3%81%93%E3%81%AE%E3%83%AD%E3%82%B0%E3%81%AB%E3%81%AF%E3%80%81Azure%20AD%20%E3%81%A8%E9%80%A3%E6%90%BA%E3%81%97%E3%81%A6%E3%81%84%E3%82%8B%20ID%20%E3%83%97%E3%83%AD%E3%83%90%E3%82%A4%E3%83%80%E3%83%BC%E3%81%AB%E3%82%88%E3%82%8B%E3%83%95%E3%82%A7%E3%83%87%E3%83%AC%E3%83%BC%E3%82%B7%E3%83%A7%E3%83%B3%20%E3%82%B5%E3%82%A4%E3%83%B3%E3%82%A4%E3%83%B3%E3%82%82%E5%90%AB%E3%81%BE%E3%82%8C%E3%81%BE%E3%81%99%E3%80%82){target="_blank"}を参照してください。

## Marketo ソリューションの設定 {#configure-marketo-solution}

もう少しです。あとは、作成した新しいユーザーについて Marketo ソルーションに知らせるだけです。

1. 「[!UICONTROL 詳細設定]」セクションに戻り、「[!UICONTROL 設定]」の横にある ![](assets/image2015-5-13-15-3a49-3a19.png) アイコンをクリックし、「**[!UICONTROL Marketo 設定]**」を選択します。

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >設定メニューで「Marketo 設定」が表示されていない場合、ページを更新します。うまくいかない場合は、再度 [Marketo Solution を公開](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"}するか、ログアウトしてから再度ログインしてください。

1. 「**[!UICONTROL デフォルト]**」をクリックします。

   ![](assets/fifteen.png)

1. **[!UICONTROL Marketo ユーザー]**&#x200B;フィールドの検索ボタンをクリックして、作成した同期ユーザーを選択します。

   ![](assets/sixteen.png)

1. 右下隅にある![](assets/image2015-3-13-15-3a10-3a11.png)アイコンをクリックして、変更を保存します。

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. 右上にある「**X**」をクリックして画面を閉じます。

   ![](assets/seventeen.png)

1. 「[!UICONTROL 設定]」の横にある ![](assets/image2015-5-13-15-3a49-3a19-1.png) アイコンをクリックし、「**[!UICONTROL ソリューション]**」を選択します。

   ![](assets/eighteen.png)

1. 「**[!UICONTROL すべてのカスタマイズを公開]**」ボタンをクリックします。

   ![](assets/nineteen.png)

   >[!NOTE]
   >
   >基本認証から [!DNL OAuth] にアップグレードする場合は、[この記事](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md)を参照して認証を再設定します。

## 手順 3 に進む前に {#before-proceeding-to-step}

* 同期するレコード数を制限する場合は、[カスタム同期フィルターを設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)します。
* [ [!DNL Microsoft Dynamics]  同期を検証](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)プロセスを実行します。初期設定が正しく行われたことを確認します。
* [!DNL Microsoft Dynamics] CRM で、Marketo 同期ユーザにログインします。

>[!MORELIKETHIS]
>
>* [手順 3／3：サーバー間接続を使用した Marketo ソリューションの接続](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-3-of-3-connect.md)
>* [ [!DNL Dynamics]  認証方法の再設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md)
