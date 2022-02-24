---
unique-page-id: 10095429
description: Dynamics 検証同期の問題を修正 — Marketoドキュメント — 製品ドキュメント
title: Dynamics 検証同期に対する問題の修正
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
source-git-commit: 8d401eeba46dc1b21983ea03c8ecd823046a5479
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 10%

---

# Dynamics 検証同期に対する問題の修正 {#fix-dynamics-validation-sync-issues}

## 同期ツールの結果を検証 {#validate-sync-tool-results}

[Dynamics 同期の検証 ] を実行すると、レポートが生成されます。 この ![x](assets/delete.png) 手順の横にある以下のオプションを参照して、問題を特定して修正します。 次に、結果に緑のチェックマーク以外が表示されるまで同期検証手順を再実行します。

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL が有効です {#url-is-valid}

次の場合、 ![x](assets/delete.png) ここで、URL が有効であることを確認します。 開発者向けリソースのここにあり、組織サービスを参照してください。 この URL は、多くの理由で無効になっている可能性があります。

1. Dynamics にログインします。 設定アイコンをクリックし、「 **詳細設定**.

   ![](assets/one.png)

1. 設定をクリックし、 **カスタマイズ**.

   ![](assets/two.png)

1. クリック **開発者リソース**.

   ![](assets/three.png)

1. 組織サービスの URL は、「サービスエンドポイント」の下に表示されます。

   ![](assets/four.png)

## ユーザ名とパスワードが有効です {#username-and-password-are-valid}

次の場合、 ![x](assets/delete.png) ここで、Microsoft Dynamics のユーザー名とパスワードが有効であることを確認します。

## 同期ユーザーがMarketo同期ユーザーロールに割り当てられています {#sync-user-is-assigned-to-the-marketo-sync-user-role}

次の場合、 ![x](assets/delete.png) ここでは、以下の 3 つの問題の 1 つになる可能性があります。

**オプション 1 - Microsoft Dynamics でMarketo Sync ユーザーの役割がオンになっていることを確認します**:

1. Dynamics で、設定アイコンをクリックし、 **詳細設定**.

   ![](assets/one.png)

1. クリック **設定** を選択し、 **セキュリティ**.

   ![](assets/six.png)

1. クリック **ユーザー。**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. 同期ユーザーのリンクをクリックします。

   ![](assets/seven.png)

1. クリック **役割の管理**.

   ![](assets/eight.png)

1. 「 Marketo同期ユーザー」の役割がオンになっていることを確認します。 そうでない場合は、チェックし、 **はい。**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

**オプション 2 — 許可の同意を確認**:

1. 以下を確認します。 [クライアント ID とアプリ登録に対する同意の付与](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md) ：アプリが API を呼び出す管理者の同意を得ていることを確認します。

**オプション 3 — ユーザーの同期**:

1. 「同期ユーザー」がMarketo設定に追加されていることを確認します。

## Marketo ソリューションが正常にインストールされました {#marketo-solution-is-properly-installed}

次の場合、 ![x](assets/delete.png) ここで、Microsoft Dynamics に移動して、Marketoのインストールが完了していることを確認します。 Microsoft Dynamics セットアップドキュメントの手順 1 を参照してください。

1. Dynamics で、設定アイコンをクリックし、 **詳細設定**.

   ![](assets/one.png)

1. クリック **設定** を選択し、 **ソリューション**

   ![](assets/eleven.png)

1. 解決策が表示されることを確認します。

   ![](assets/twelve.png)

## ソリューションのすべてのステップが有効です {#all-steps-in-the-solution-are-enabled}

次の場合、 ![x](assets/delete.png) ここで、デフォルトの手順が無効になっていないことを確認します。 すべての手順はインストール時に自動的に有効になりますが、カスタマイズ時に無効にすることができます。

## 同期ユーザが Marketo ソリューションに割り当てられています {#sync-user-is-assigned-to-the-marketo-solution}

次の場合、 ![x](assets/delete.png) ここでは、Microsoft Dynamics のMarketoデフォルトページで同期ユーザーが割り当てられていることを確認します。

1. Dynamics で、設定アイコンをクリックし、 **詳細設定**.

   ![](assets/one.png)

1. クリック **設定** を選択し、 **Marketo Config**.

   ![](assets/thirteen.png)

1. 同期ユーザーがデフォルトとして割り当てられていることを確認します。

   ![](assets/fourteen.png)

## 同期ユーザがユーザ名とパスワードに一致します {#sync-user-matches-username-and-password}

次の場合、 ![x](assets/delete.png) ここでは、Microsoft Dynamics の「 Marketo設定のデフォルト設定」手順の「 Marketoユーザー」フィールドで、適切な同期ユーザーを割り当ててください。

>[!MORELIKETHIS]
>
>[Microsoft Dynamics 同期の検証](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
