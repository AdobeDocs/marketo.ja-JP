---
description: クライアント ID とアプリの登録に対する同意の付与 — Marketoドキュメント — 製品ドキュメント
title: クライアント ID とアプリ登録に対する同意の付与
exl-id: d0c851d7-24a1-4b17-9daa-f0ceed39d040
source-git-commit: e8ba27c09165aa844ae6df175464d989b1931bad
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 6%

---

# クライアント ID とアプリ登録に対する同意の付与 {#grant-consent-for-client-id-and-app-registration}

## 同期ユーザーに委任されたユーザー権限を付与する {#grant-delegated-user-permissions-for-the-sync-user}

1. クリーンテキストプログラム (Windows の場合はメモ帳、Macの場合はテキスト編集 ) を使用して、下のテキストを貼り付け、client_id、redirect_uri、および state の値を置き換えて、認証用の Uniform Resource Identifier(URI) を作成します。

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
      <td><strong>client_id の値</strong></td> 
      <td>は、アプリ登録プロセスで生成される client_id である必要があります</td> 
     </tr> 
     <tr> 
      <td><strong>redirect_uri 値</strong></td> 
      <td>は、アプリの登録/リダイレクト URI の時点で入力された値と同じである必要があります</td> 
     </tr> 
     <tr> 
      <td><strong>状態値</strong></td> 
      <td>任意の ID を指定できます ( 例：12345)</td> 
     </tr> 
    </tbody> 
   </table>

   最終的な URL は次のようになります。 `https://login.microsoftonline.com/common/oauth2/authorize?client_id=xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx&response_type=code&redirect_uri=https://www.marketo.com&response_mode=query&state=12345`

1. 作成した URI を任意のブラウザーで開きます。

   ![](assets/grant-consent-for-client-id-app-registration-1.png)

1. 権限を付与する Sync User としてログインします。

   ![](assets/grant-consent-for-client-id-app-registration-2.png)

   >[!NOTE]
   >
   >別のタブで既に Azure に管理者としてログインしている場合は、別のブラウザまたは匿名モードを使用して、同期ユーザーとしてログインする必要があります。

1. クリック **確定**.

   ![](assets/grant-consent-for-client-id-app-registration-3.png)

## すべてのユーザーに同意する {#grant-consent-for-all-users}

管理者は、テナント内のすべてのユーザーに代わって、アプリケーションの委任された権限に同意することもできます。 管理者の同意を得ると、テナント内のすべてのユーザーに対して同意ダイアログが表示されなくなり、管理者の役割を持つユーザーが Azure ポータルで同意ダイアログを実行できます。 管理者の役割で実行できる役割を説明します [委任された権限に対する同意](https://docs.microsoft.com/en-us/azure/active-directory/roles/permissions-reference).

1. Azure ポータルで、アプリケーションのホームページに移動します。

1. 管理で、 **API 権限**.

   ![](assets/grant-consent-for-client-id-app-registration-4.png)

1. 次をクリック： **管理者の同意を得る** （テナントの場合）ボタン。

   ![](assets/grant-consent-for-client-id-app-registration-5.png)

1. クリック **はい** をクリックして確定します。

   ![](assets/grant-consent-for-client-id-app-registration-6.png)

