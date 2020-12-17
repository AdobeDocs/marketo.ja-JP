---
unique-page-id: 10095429
description: Dynamics検証の同期の問題を修正 — Marketto Docs — 製品ドキュメント
title: Dynamics検証の同期の問題を修正
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---


# Dynamics検証の同期の問題を修正{#fix-dynamics-validation-sync-issues}

## 同期ツールの結果の検証{#validate-sync-tool-results}

Dynamics Validate Syncを実行すると、このレポートが生成されます。 手順の横に![delete](assets/delete.png)がある場合は、以下を参照して問題を特定し、修正してください。 次に、結果にチェックマーク以外の内容が表示されるまで、同期検証手順を再実行します。

![](assets/image2015-9-22-15-3a58-3a12.png)

## URLは有効{#url-is-valid}です

ここに![delete](assets/delete.png)がある場合は、URLが有効であることを確認します。 開発者向けリソースで見つけて、組織サービスを参照してください。 URLが無効になる理由はいくつかあります。

1. Dynamicsにログインします。 設定アイコンをクリックし、「**詳細設定**」を選択します。

   ![](assets/one.png)

1. 「設定」をクリックし、「**カスタマイズ**」を選択します。

   ![](assets/two.png)

1. **開発者向けリソース**&#x200B;をクリックします。

   ![](assets/three.png)

1. 組織サービスのURLは、「サービスエンドポイント」の下にあります。

   ![](assets/four.png)

## ユーザー名とパスワードは有効です{#username-and-password-are-valid}

![—](assets/delete.png)をお持ちの場合は、Microsoft Dynamicsのユーザー名とパスワードが有効であることを確認してください。

## 同期ユーザーがMarketto Syncユーザーロール{#sync-user-is-assigned-to-the-marketo-sync-user-role}に割り当てられています

ここに![—](assets/delete.png)がある場合は、Microsoft DynamicsでMarketto Syncユーザーロールがチェック済みであることを確認する必要があります。 Microsoft Dynamicsのインストールドキュメントの手順2を参照してください。

1. Dynamicsで、設定アイコンをクリックし、**詳細設定**&#x200B;を選択します。

   ![](assets/one.png)

1. 「**設定**」をクリックし、「**セキュリティ**」を選択します。

   ![](assets/six.png)

1. 「**ユーザー」をクリックします。**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. 同期ユーザーのリンクをクリックします。

   ![](assets/seven.png)

1. 「**ロールの管理**」をクリックします。

   ![](assets/eight.png)

1. Marketor Syncユーザーロールがチェック済みであることを確認します。 見つからない場合は、チェックして&#x200B;**OKをクリックします。**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

## Marketo Solutionは適切にインストールされています{#marketo-solution-is-properly-installed}

![—](assets/delete.png)をお持ちの場合は、Microsoft Dynamicsにアクセスして、Marketoのインストールが存在することを確認してください。 MIcrosoft Dynamicsセットアップドキュメントの手順1を参照してください。

1. Dynamicsで、設定アイコンをクリックし、**詳細設定**&#x200B;を選択します。

   ![](assets/one.png)

1. 「**設定**」をクリックし、「**ソリューション」を選択します。**

   ![](assets/eleven.png)

1. ソリューションが一覧に表示されることを確認します。

   ![](assets/twelve.png)

## ソリューション内のすべてのステップが有効{#all-steps-in-the-solution-are-enabled}

ここに![—](assets/delete.png)がある場合は、デフォルトの手順がいずれも非アクティブ化されていないことを確認してください。 すべての手順は、インストール時に自動的に有効になりますが、カスタマイズ時に無効にすることができます。

## 同期ユーザーがMarketoソリューション{#sync-user-is-assigned-to-the-marketo-solution}に割り当てられている

ここに![—](assets/delete.png)がある場合は、Microsoft DynamicsのMarketo Defaultページで同期ユーザーが割り当てられていることを確認してください。

1. Dynamicsで、設定アイコンをクリックし、**詳細設定**&#x200B;を選択します。

   ![](assets/one.png)

1. 「**設定**」をクリックし、「**Marketto Config**」を選択します。

   ![](assets/thirteen.png)

1. 同期ユーザーがデフォルトとして割り当てられていることを確認します。

   ![](assets/fourteen.png)

## 同期ユーザーがユーザー名とパスワード{#sync-user-matches-username-and-password}と一致

ここに![—](assets/delete.png)がある場合は、Microsoft DynamicsのMarketo Configのデフォルト設定手順の「Marketoユーザー」フィールドに適切な同期ユーザーを割り当ててください。

>[!MORELIKETHIS]
>
>[Microsoft Dynamics同期の検証](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)

