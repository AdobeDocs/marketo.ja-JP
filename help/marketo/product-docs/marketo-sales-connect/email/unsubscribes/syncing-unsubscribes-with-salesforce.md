---
unique-page-id: 14746188
description: Salesforceとの登録解除の同期 — Marketto Docs — 製品ドキュメント
title: Salesforceとの登録解除の同期
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---


# Salesforceとの登録解除{#syncing-unsubscribes-with-salesforce}

## Salesforceとの同期を取り消すための要件{#requirements-for-unsubscribes-to-sync-to-salesforce}

* 「登録解除同期」を有効にする必要があります（夜間同期用）
* フィールドオプトアウトをSalesforceにインストールする必要があります
* Sales ConnectのユーザーレコードにはSalesforce IDが必要です

**プッシュ解除**

Sales Connectで登録解除が収集されると、Salesforceにリアルタイムでプッシュして、同期対象として選択したいずれかのオプトアウトフィールドを更新します。 Salesforceの同期を無効にしている場合は、登録解除を電子メールに引き続きプッシュオプトアウトします。

**登録解除同期**

登録解除同期を有効にした場合（下の手順3を参照）、夜間同期が有効になります。 同期は、午後8時(PST)頃に1日1回実行されます。 MSE/ToutApp内のすべての購読解除をSalesforceのフィールドと双方向オプトアウトに同期します。

## Salesforceへの登録解除同期の設定{#configure-unsubscribe-sync-to-salesforce}

ユーザーは、購読解除をMarketorと同期できる標準の電子メールオプトアウトフィールドと同期するか、またはマーケティング担当者のセールスフィールドと同期してSalesの購読解除とMarketingの購読解除を区別できるオプトアウトかを決定できます。

1. [Webアプリケーション](http://toutapp.com/login)に移動し、歯車アイコンをクリックして、**設定**&#x200B;を選択します。

   ![](assets/one-1.png)

1. 「管理設定」で、「**購読解除**」を選択します。

   ![](assets/two-2.png)

1. **Salesforce**&#x200B;と同期をクリックし、夜間同期を有効にします。

   ![](assets/three-2.png)

1. 同期先のフィールドを選択します。

   ![](assets/4.png)

   | **Salesforceフオプトアウトィールドと同期** | デフォルトで選択されている場合は、Salesforceフオプトアウトィールドのみが更新されます。 |
   |---|---|
   | **マーケティング担当者の販売オプトアウトフィールドと同期** | 販売とマーケティングの購読を分割する場合は、このオプションを選択して、追加の[販売のオプトアウトマーケティングフィールドを更新します。](#msoo) |

## ページレイアウトオプトアウトのフィールドのインストール{#installing-the-opt-out-field-in-the-page-layout}

**電子メオプトアウトール**

電子メールは、Salesforceからインストールできる、Salesforceの標準フィールドです。 インストールするには、Salesforce管理者である必要があります。

1. [Salesforce.com](http://Salesforce.com)に移動し、サインインします。

   ![](assets/five-1.png)

1. ユーザー名をクリックし、「**セットアップ**」を選択します。

   ![](assets/six-1.png)

1. [クイック検索]ボックスで、[連絡先]または[リード]を検索します。 このシナリオでは、[連絡先]ページのレイアウトにフィールドをインストールしますが、両方のユーザーレコードに対してインストールを行います。

   ![](assets/seven-1.png)

1. 「**ページレイアウト**」を選択します。

   ![](assets/eight-1.png)

1. フィールドを追加するページレイアウトの横にある「**編集**」を選択します。

   ![](assets/nine.png)

1. 「**フィールド**」を選択します。

   ![](assets/ten.png)

1. 電子メールをページレイアウトにドラッグ&amp;ドロップオプトアウトします。

   ![](assets/11.png)

1. 「**保存**」をクリックします。

   ![](assets/twelve.png)

## マーケティンオプトアウトグ担当者{#marketo-sales-opt-out}

「マーケティングオプトアウト先の販売」フィールドは、Marketo Sales Connectのカスタマイズをインストールしたユーザーが使用できるカスタムフィールドです。

「Marketo Sales Connect Customizations」のSalesforceへのインストールが完了すると、「Marketo Sales」フィールドが表示されオプトアウトます。
