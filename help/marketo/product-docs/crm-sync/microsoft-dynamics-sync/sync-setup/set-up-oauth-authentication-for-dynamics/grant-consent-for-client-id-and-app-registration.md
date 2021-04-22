---
description: クライアントIDとアプリ登録に関する同意の付与 —Marketoドキュメント — 製品ドキュメント
title: クライアントIDとアプリ登録に関する同意の付与
exl-id: d0c851d7-24a1-4b17-9daa-f0ceed39d040
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# クライアントIDとアプリ登録に関する同意の付与{#grant-consent-for-client-id-and-app-registration}

## 同期ユーザーに委任されたユーザーの権限を付与{#grant-delegated-user-permissions-for-the-sync-user}

1. クリーンテキストプログラム（Windowsの場合はメモ帳、Macの場合はテキスト編集）を使用して、認証用のUniform Resource Identifier(URI)を作成します。その際には、次のテキストを貼り付け、client_id、redirect_uri、およびstameの値を置き換えます。

   ```
   https://login.microsoftonline.com/common/oauth2/authorize?
   client_id='xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx'
   &response_type='code'
   &redirect_uri='https://www.<ourdomain>.com'
   &response_mode='query'
   &state='SOME_UNIQUE_UID'
   client_id value should be the client_id generated in App Registration process
   redirect_uri value should be same as value entered at the time of App registration-> Redirect URIs
   state value can be any ID (e.g.,12345)
   ```

   <table> 
    <colgroup> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>client_idの値</strong></td> 
      <td>は、アプリの登録プロセスで生成されるclient_idである必要があります</td> 
     </tr> 
     <tr> 
      <td><strong>redirect_uri値</strong></td> 
      <td>は、アプリの登録/リダイレクトURIの時点で入力された値と同じである必要があります</td> 
     </tr> 
     <tr> 
      <td><strong>状態値</strong></td> 
      <td>は任意のID（例：12345）です。</td> 
     </tr> 
    </tbody> 
   </table>

   最終的なURLは次のようになります。`https://login.microsoftonline.com/common/oauth2/authorize?client_id=xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx&response_type=code&redirect_uri=https://www.marketo.com&response_mode=query&state=12345`

1. 作成したURIを任意のブラウザーで開きます。

   ![](assets/grant-consent-for-client-id-app-registration-1.png)

1. 権限を付与する同期ユーザーとしてログインします。

   ![](assets/grant-consent-for-client-id-app-registration-2.png)

   >[!NOTE]
   >
   >別のタブで既に管理者としてAzureにログインしている場合は、別のブラウザーまたは匿名モードを使用して同期ユーザーとしてログインする必要があります。

1. 「**承諾**」をクリックします。

   ![](assets/grant-consent-for-client-id-app-registration-3.png)

## すべてのユーザーに同意を与える{#grant-consent-for-all-users}

管理者は、テナント内のすべてのユーザーに代わって、アプリケーションの委任された権限に同意することもできます。 管理者の同意により、テナント内のすべてのユーザーに対して同意ダイアログが表示されなくなり、管理者の役割を持つユーザーがAzureポータルで実行できます。 委任された権限に対して[同意できる管理者の役割](https://docs.microsoft.com/en-us/azure/active-directory/roles/permissions-reference)を示します。

1. Azureポータルで、アプリケーションのホームページに移動します。

1. 「管理」で、「**API権限**」をクリックします。

   ![](assets/grant-consent-for-client-id-app-registration-4.png)

1. 「**管理者の同意を許可**」ボタン（テナントの場合）をクリックします。

   ![](assets/grant-consent-for-client-id-app-registration-5.png)

1. 「**はい**」をクリックして確認します。

   ![](assets/grant-consent-for-client-id-app-registration-6.png)

>[!MORELIKETHIS]
>
>[オンプレミス用Microsoft Dynamics CRMアプリのセットアップ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/set-up-oauth-authentication-for-dynamics/set-up-microsoft-dynamics-crm-app-for-on-prem.md)
