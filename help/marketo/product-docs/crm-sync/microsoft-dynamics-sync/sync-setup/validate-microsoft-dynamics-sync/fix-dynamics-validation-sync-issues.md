---
unique-page-id: 10095429
description: Dynamics 検証同期に対する問題の修正 - Marketo ドキュメント - 製品ドキュメント
title: Dynamics 検証同期に対する問題の修正
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
source-git-commit: 48b8289994e000eafd72982ac1b4a0a809b10bab
workflow-type: ht
source-wordcount: '493'
ht-degree: 100%

---

# Dynamics 検証同期に対する問題の修正 {#fix-dynamics-validation-sync-issues}

## 同期ツールの結果を検証 {#validate-sync-tool-results}

Dynamics の同期検証を実行すると、レポートが生成されます。手順の横に ![x](assets/delete.png) がある場合、以下のオプションを参照して、問題を特定して修正します。次に、結果に緑のチェックマーク以外の内容が表示されなくなるまで同期検証手順を再実行します。

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL が有効です {#url-is-valid}

ここに ![x](assets/delete.png) がある場合、URL が有効であることを確認します。こちらのデベロッパー向けリソースで、組織サービスを参照してください。URL は、多くの理由で無効になっている可能性があります。

1. Dynamics にログインします。設定アイコンをクリックし、「**詳細設定**」を選択します。

   ![](assets/one.png)

1. 「設定」をクリックし、「**カスタマイズ**」を選択します。

   ![](assets/two.png)

1. 「**デベロッパーリソース**」をクリックします。

   ![](assets/three.png)

1. 組織サービスの URL は、「サービスエンドポイント」に表示されます。

   ![](assets/four.png)

## ユーザ名とパスワードが有効です {#username-and-password-are-valid}

ここに ![x](assets/delete.png) がある場合、Microsoft Dynamics の資格情報が有効であることを確認します。Web API S2S 認証の場合、Marketo のユーザ名は CRM のアプリケーションユーザの[電子メールアドレス](https://docs.microsoft.com/ja-jp/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user)と一致する必要があります。他のタイプの場合は、同期ユーザ名と一致する必要があります。

## 同期ユーザが Marketo 同期ユーザロールに割り当てられています {#sync-user-is-assigned-to-the-marketo-sync-user-role}

ここに ![x](assets/delete.png) がある場合、以下の 3 つの問題の 1 つである可能性があります。

**オプション 1 - Microsoft Dynamics で Marketo 同期ユーザのロールがオンになっていることを確認します**。

1. Dynamics で、設定アイコンをクリックし、「**詳細設定**」を選択します。

   ![](assets/one.png)

1. 「**設定**」をクリックし、「**セキュリティ**」を選択します。

   ![](assets/six.png)

1. 「**ユーザ**」をクリックします。

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. 同期ユーザのリンクをクリックします。

   ![](assets/seven.png)

1. 「**ロールを管理**」をクリックします。

   ![](assets/eight.png)

1. 「Marketo 同期ユーザ」のロールがオンになっていることを確認します。オンになっていない場合は、チェックをオンにして「**OK**」をクリックします。

   ![](assets/image2015-9-24-9-3a59-3a21.png)

**オプション 2 - 許可の同意を確認します**。

1. [クライアント ID とアプリ登録に対する同意の付与](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md)を確認して、アプリが API を呼び出す管理者の同意を得ていることを確認します。

**オプション 3 - 同期ユーザ**。

1. 同期ユーザが Marketo 設定に追加されていることを確認します。

## Marketo ソリューションが正常にインストールされました {#marketo-solution-is-properly-installed}

ここに ![x](assets/delete.png) がある場合、Microsoft Dynamics に移動して、Marketo のインストールが完了していることを確認します。Microsoft Dynamics 設定ドキュメントの手順 1 を参照してください。

1. Dynamics で、設定アイコンをクリックし、「**詳細設定**」を選択します。

   ![](assets/one.png)

1. 「**設定**」をクリックして、「**ソリューション**」を選択します。

   ![](assets/eleven.png)

1. 解決策が表示されることを確認します。

   ![](assets/twelve.png)

## ソリューションのすべての手順が有効です {#all-steps-in-the-solution-are-enabled}

ここに ![x](assets/delete.png) がある場合、デフォルトの手順が無効になっていないことを確認します。すべての手順はインストール時に自動的に有効になりますが、カスタマイズ時に無効にすることができます。

## 同期ユーザが Marketo ソリューションに割り当てられています {#sync-user-is-assigned-to-the-marketo-solution}

ここに ![x](assets/delete.png) がある場合、Microsoft Dynamics の Marketo デフォルトページで同期ユーザが割り当てられていることを確認します。

1. Dynamics で、設定アイコンをクリックし、「**詳細設定**」を選択します。

   ![](assets/one.png)

1. 「**設定**」をクリックし、「**Marketo 設定**」を選択します。

   ![](assets/thirteen.png)

1. 同期ユーザがデフォルトとして割り当てられていることを確認します。

   ![](assets/fourteen.png)

## 同期ユーザがユーザ名とパスワードに一致します {#sync-user-matches-username-and-password}

ここに ![x](assets/delete.png) がある場合、Microsoft Dynamics の「Marketo 設定のデフォルト設定」手順で、「Marketo ユーザ」フィールドに適切な同期ユーザを割り当ててください。

>[!MORELIKETHIS]
>
>[Microsoft Dynamics 同期の検証](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
