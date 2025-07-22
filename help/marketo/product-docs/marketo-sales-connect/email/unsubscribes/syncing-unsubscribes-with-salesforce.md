---
unique-page-id: 14746188
description: Salesforce との登録解除の同期 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce との登録解除の同期
exl-id: 1694d7bf-d2f6-4950-8a3e-c7d89c37b276
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 59%

---

# 購読解除と [!DNL Salesforce] の同期 {#syncing-unsubscribes-with-salesforce}

## 購読解除が [!DNL Salesforce] と同期するための要件 {#requirements-for-unsubscribes-to-sync-to-salesforce}

* 登録解除の同期を有効にする必要があります（夜間同期）
* オプトアウトフィールドを [!DNL Salesforce] にインストールする必要があります
* [!DNL Sales Connect] の人物レコードには [!DNL Salesforce] ID が必要です

**登録解除のプッシュ**

登録解除が [!DNL Sales Connect] で収集されると、リアルタイムで [!DNL Salesforce] にプッシュし、同期するように選択したオプトアウトフィールドのいずれかを更新します。 [!DNL Salesforce] 同期を無効にした場合でも、購読解除をメールオプトアウトにプッシュします。

**登録解除を同期**

登録解除を同期を有効にする（以下の手順 3）と、夜間同期が有効になります。同期は 1 日 1 回、午後 8:00 （PST）頃に行われます。 Marketo Sales 内のすべての登録解除と Salesforce の「オプトアウト」フィールドが双方向に同期されます。

## [!DNL Salesforce] への購読解除同期の設定 {#configure-unsubscribe-sync-to-salesforce}

ユーザーは、登録解除を Marketo も同期できる標準の「メールオプトアウト」フィールドに同期するか、「Marketo セールスオプトアウトフィールド」に同期してセールス登録解除とマーケティング登録解除を区別できるようにするかを指定できます。

1. [Web アプリケーション](https://toutapp.com/login)で、歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/one-1.png)

1. [!UICONTROL  管理者設定 ] で **[!UICONTROL 購読解除]** を選択します。

   ![](assets/two-2.png)

1. 「**[!UICONTROL Salesforce に同期]**」をクリックし、夜間同期を有効にします。

   ![](assets/three-2.png)

1. 同期先のフィールドを選択します。

   ![](assets/4.png)

   | フィールド | 説明 |
   |---|---|
   | **[!UICONTROL Salesforce オプトアウトフィールドに同期]** | デフォルトで選択されている場合は、「オプトアウト」フィールド [!DNL Salesforce] のみ更新されます。 |
   | **[!UICONTROL Marketo Sales オプトアウトフィールドに同期]** | セールスとマーケティングの登録解除を分ける場合は、このオプションを選択して、追加の [Marketo Sales オプトアウトフィールド](#msoo)を更新します。 |

## ページレイアウトの「オプトアウト」フィールドのインストール {#installing-the-opt-out-field-in-the-page-layout}

**メールオプトアウト**

「メールオプトアウト」は、[!DNL Salesforce] からインストールできる [!DNL Salesforce] の標準フィールドです。 インストールするには [!DNL Salesforce] 管理者である必要があります。

1. [Salesforce.com](https://salesforce.com) に移動し、ログインします。

   ![](assets/five-1.png)

1. ユーザー名をクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/six-1.png)

1. クイック検索ボックスで、取引先責任者またはリードを検索します。このシナリオでは、取引先責任者ページレイアウトのフィールドをインストールしますが、両方の人物レコード用にインストールする場合もあります。

   ![](assets/seven-1.png)

1. 「**[!UICONTROL ページレイアウト]**」を選択します。

   ![](assets/eight-1.png)

1. フィールドを追加するページレイアウトの横にある「**[!UICONTROL 編集]**」を選択します。

   ![](assets/nine.png)

1. 「**[!UICONTROL フィールド]**」を選択します。

   ![](assets/ten.png)

1. [!UICONTROL  メールオプトアウト ] をページレイアウトにドラッグ&amp;ドロップします。

   ![](assets/11.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/twelve.png)

## Marketo Sales オプトアウト {#marketo-sales-opt-out}

「Marketoの販売オプトアウト」フィールドは、Marketo [!DNL Sales Connect] Customizations をインストールしたユーザーが使用できるカスタムフィールドです。

Marketo [!DNL Sales Connect] Customizations をに正常にインストールす [!DNL Salesforce] と、Marketoの「Sales Opt Out」フィールドが表示されます。
