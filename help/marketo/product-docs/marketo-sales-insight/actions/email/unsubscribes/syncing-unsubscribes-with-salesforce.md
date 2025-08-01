---
description: Salesforce との登録解除の同期 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce との登録解除の同期
exl-id: b5b0f625-e38c-4a03-81e7-010082001636
feature: Sales Insight Actions
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 58%

---

# 購読解除と [!DNL Salesforce] の同期 {#syncing-unsubscribes-with-salesforce}

登録解除を Salesforce の「オプトアウト」フィールドと同期する場合、Salesforce 登録解除の同期を使用できます。

## Salesforce と登録解除を同期する際の要件 {#requirements-for-unsubscribes-to-sync-to-salesforce}

* 登録解除の同期を有効にする必要があります（夜間同期）
* オプトアウトフィールドを [!DNL Salesforce] にインストールする必要があります
* [!DNL Marketo Sales] の人物レコードには [!DNL Salesforce] ID が必要です

**登録解除のプッシュ**

登録解除が [!DNL Marketo Sales] で収集されると、リアルタイムで [!DNL Salesforce] にプッシュし、同期するように選択したオプトアウトフィールドのいずれかを更新します。 [!DNL Salesforce] 同期を無効にした場合でも、購読解除をメールオプトアウトにプッシュします。

**登録解除の同期**

登録解除を同期を有効にする（以下の手順 3）と、夜間同期が有効になります。同期は 1 日 1 回、午後 8:00 （PST）頃に行われます。 Marketo Sales 内のすべての登録解除と Salesforce の「オプトアウト」フィールドが双方向に同期されます。

>[!NOTE]
>
>Salesforce との登録解除の同期は、登録解除を同期しますが、再登録は同期しません。Marketo Sales および Salesforce から登録解除を削除する場合、Salesforce で登録解除のチェックをオフにして、Marketo Sales で登録解除を削除します。

## [!DNL Salesforce] への購読解除同期の設定 {#configure-unsubscribe-sync-to-salesforce}

ユーザーは、登録解除をMarketoと同期できる標準のメールオプトアウトフィールドと同期するか、[!DNL Marketo Sales] ールオプトアウトフィールドと同期して、営業の登録解除とマーケティングの登録解除を区別できるようにすることができます。

1. 歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/syncing-unsubscribes-with-salesforce-1.png)

1. [!UICONTROL  管理者設定 ] で **[!UICONTROL 購読解除]** を選択します。

   ![](assets/syncing-unsubscribes-with-salesforce-2.png)

1. 「**[!UICONTROL 統合]**」タブをクリックします。[!UICONTROL Salesforceに同期 ] で、夜間同期を有効にします。

   ![](assets/syncing-unsubscribes-with-salesforce-3.png)

1. 同期先のフィールドを選択します。

   ![](assets/syncing-unsubscribes-with-salesforce-4.png)

   | フィールド | 説明 |
   |---|---|
   | **「オプトアウト [!DNL Salesforce] 同期」フィールド** | デフォルトで選択されている場合は、「オプトアウト」フィールド [!DNL Salesforce] のみ更新されます。 |
   | **「オプトアウト [!DNL Marketo Sales] 同期」フィールド** | 営業とマーケティングの購読解除を分離する場合、このオプションを選択して追加の [[!DNL Marketo Sales]  オプトアウトフィールド ](#msoo) を更新します。 |

## ページレイアウトの「オプトアウト」フィールドのインストール {#installing-the-opt-out-field-in-the-page-layout}

**メールオプトアウト**

「メールオプトアウト」は、[!DNL Salesforce] からインストールできる [!DNL Salesforce] の標準フィールドです。 インストールするには [!DNL Salesforce] 管理者である必要があります。

1. [Salesforce.com](https://salesforce.com) に移動し、ログインします。

   ![](assets/syncing-unsubscribes-with-salesforce-5.png)

1. ユーザー名をクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/syncing-unsubscribes-with-salesforce-6.png)

1. クイック検索ボックスで、取引先責任者またはリードを検索します。このシナリオでは、取引先責任者ページレイアウトのフィールドをインストールしますが、両方の人物レコード用にインストールする場合もあります。

   ![](assets/syncing-unsubscribes-with-salesforce-7.png)

1. 「**[!UICONTROL ページレイアウト]**」を選択します。

   ![](assets/syncing-unsubscribes-with-salesforce-8.png)

1. フィールドを追加するページレイアウトの横にある「**[!UICONTROL 編集]**」を選択します。

   ![](assets/syncing-unsubscribes-with-salesforce-9.png)

1. 「**[!UICONTROL フィールド]**」を選択します。

   ![](assets/syncing-unsubscribes-with-salesforce-10.png)

1. [!UICONTROL  メールオプトアウト ] をページレイアウトにドラッグ&amp;ドロップします。

   ![](assets/syncing-unsubscribes-with-salesforce-11.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/syncing-unsubscribes-with-salesforce-12.png)

## Marketo Sales オプトアウト {#marketo-sales-opt-out}

Marketo Sales オプトアウトフィールドは、[AppExchange から](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"} Marketo Sales Insight パッケージをインストールしたユーザーが使用できるカスタムフィールドです。

Marketo Sales Insight パッケージを AppExchange から Salesforce に正常にインストールすると、「Marketo Sales オプトアウト」フィールドが表示されます。
