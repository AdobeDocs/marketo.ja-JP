---
unique-page-id: 14746188
description: Salesforce との登録解除の同期 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce との登録解除の同期
exl-id: 1694d7bf-d2f6-4950-8a3e-c7d89c37b276
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 100%

---

# Salesforce との登録解除の同期 {#syncing-unsubscribes-with-salesforce}

## Salesforce と登録解除を同期する際の要件 {#requirements-for-unsubscribes-to-sync-to-salesforce}

* 登録解除の同期を有効にする必要があります（夜間同期）
* Salesforce に「オプトアウト」フィールドがインストールされている
* Sales Connect のユーザーレコードに Salesforce ID がある

**登録解除をプッシュ**

Sales Connect で登録解除が収集された場合は、リアルタイムで Salesforce にプッシュし、同期対象として選択した「オプトアウト」フィールドのいずれかをアップデートします。Salesforce 同期を無効にしても、登録解除はメールオプトアウトに引き続きプッシュされます。

**登録解除を同期**

登録解除を同期を有効にする（以下の手順 3）と、夜間同期が有効になります。同期は 1 日に 1 回、午後 8:00（PST）頃に実行されます。Marketo Sales 内のすべての登録解除と Salesforce の「オプトアウト」フィールドが双方向に同期されます。

## Salesforce に登録解除の同期を設定 {#configure-unsubscribe-sync-to-salesforce}

ユーザーは、登録解除を Marketo も同期できる標準の「メールオプトアウト」フィールドに同期するか、「Marketo セールスオプトアウトフィールド」に同期してセールス登録解除とマーケティング登録解除を区別できるようにするかを指定できます。

1. [Web アプリケーション](https://toutapp.com/login)で、歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/one-1.png)

1. 管理設定で「**登録解除**」を選択します。

   ![](assets/two-2.png)

1. 「**Salesforce に同期**」をクリックし、夜間同期を有効にします。

   ![](assets/three-2.png)

1. 同期先のフィールドを選択します。

   ![](assets/4.png)

   | フィールド | 説明 |
   |---|---|
   | **Salesforce オプトアウトフィールドに同期** | デフォルトで選択され、Salesforce オプトアウトフィールドのみが更新されます。 |
   | **Marketo Sales オプトアウトフィールドに同期** | セールスとマーケティングの登録解除を分ける場合は、このオプションを選択して、追加の [Marketo Sales オプトアウトフィールド](#msoo)を更新します。 |

## ページレイアウトの「オプトアウト」フィールドのインストール {#installing-the-opt-out-field-in-the-page-layout}

**メールオプトアウト**

メールのオプトアウトは、Salesforce からインストールできる Salesforce の標準フィールドです。インストールするには、Salesforce 管理者である必要があります。

1. [Salesforce.com](https://salesforce.com) に移動し、ログインします。

   ![](assets/five-1.png)

1. ユーザー名をクリックし、「**設定**」を選択します。

   ![](assets/six-1.png)

1. クイック検索ボックスで、取引先責任者またはリードを検索します。このシナリオでは、取引先責任者ページレイアウトのフィールドをインストールしますが、両方の人物レコード用にインストールする場合もあります。

   ![](assets/seven-1.png)

1. 「**ページレイアウト**」を選択します。

   ![](assets/eight-1.png)

1. フィールドを追加するページレイアウトの横にある「**編集**」を選択します。

   ![](assets/nine.png)

1. 「**フィールド**」を選択します。

   ![](assets/ten.png)

1. メールオプトアウトをページレイアウトにドラッグ＆ドロップします。

   ![](assets/11.png)

1. 「**保存**」をクリックします。

   ![](assets/twelve.png)

## Marketo セールスオプトアウト {#marketo-sales-opt-out}

Marketo セールスオプトアウトフィールドは、Marketo Sales Connect のカスタマイズをインストールしたユーザーが使用できるカスタムフィールドです。

Marketo Sales Connect のカスタマイズを Salesforce に正常にインストールすると、Marketo セールスオプトアウトフィールドが表示されます。
