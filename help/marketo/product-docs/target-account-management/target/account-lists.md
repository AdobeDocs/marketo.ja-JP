---
unique-page-id: 11378814
description: アカウントリスト-Marketoドキュメント — 製品ドキュメント
title: 顧客リスト
exl-id: 31bb4341-d012-4239-8f40-10a07cd4c51c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 顧客リスト {#account-lists}

アカウントリストは、複数のアカウントをターゲットにすることができる、名前付きのアカウントの集まりです。 アカウントリストを使用すると、会社の業種、場所またはサイズに基づいてアカウント名をターゲットできます。

アカウントリストに加えて、パブリックCRMアカウント表示から生成される動的なアカウントリストを作成することもできます。 CRMアカウント表示は、アカウントを表示する際にフィルターとして機能する一連のルールです。 例えば、IndustryがHealthcare *で* Revenueが$100Mを超えるアカウントを検索する場合に使用できます。

![](assets/one.png)

>[!NOTE]
>
>Marketoターゲットのアカウント管理で作成されたアカウントリストは、[Webパーソナライゼーション](/help/marketo/product-docs/web-personalization/using-web-segments/web-segments.md)でスマートリストとWebキャンペーンを構築する際に、自動的に使用できます。

## 新しいアカウントリストの作成{#create-a-new-account-list}

1. 「**新規**」ドロップダウンをクリックし、「**新しいアカウントを作成**」を選択します。

   ![](assets/1a.png)

1. リストに名前を付け、「**作成**」をクリックします。

   ![](assets/three-0.png)

1. アカウントリストを作成したら、[](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)に名前付きのアカウントを追加し始めます。

   >[!NOTE]
   >
   >Marketoは、2,000人以下のアカウント名を持つアカウントリストのインサイトのみを表示します。

## 新しい動的アカウントリストの作成{#create-a-new-dynamic-account-list}

1. 「**新規**」ドロップダウンをクリックし、「**新しい動的リストを作成**」を選択します。

   ![](assets/1.png)

1. ダイアログで、ドロップダウンから&#x200B;**CRMアカウント表示**&#x200B;を選択するか、名前を入力して検索します。

   ![](assets/image2017-7-18-9-48-23.png)

1. 「**作成**」をクリックします。

   ![](assets/step4.jpg)

   >[!NOTE]
   >
   >Salesforceでは、同期ユーザーに対してリスト表示オブジェクトの権限を必ず指定してください。

## アカウントリストの名前を変更{#rename-an-account-list}

>[!NOTE]
>
>これらの手順は、アカウントリストにのみ適用されます。 _Dynamicaccount_ リストは、関連するCRMアカウント表示の名前を使用します。

1. 名前を変更するアカウントを選択し、「**アカウントリストの操作**」ドロップダウンをクリックして、「**アカウントリスト名の変更**」を選択します。

   ![](assets/three.png)

1. 新しい名前を入力し、**名前の変更**&#x200B;をクリックします。

   ![](assets/four.png)

   >[!NOTE]
   >
   >CRMアカウント表示は、8時間ごとに動的アカウントリストに同期します。 まだ同期されていない場合は、Marketoは次のサイクル中に同期します。

## アカウントリストの削除{#delete-an-account-list}

>[!NOTE]
>
>これらの手順は、アカウントリストと動的アカウントリストの両方で同じです。

1. 削除するアカウントを選択し、「**アカウントリストの操作**」ドロップダウンをクリックして、「**アカウントリストを削除**」を選択します。

   ![](assets/five.png)

1. 「**削除**」をクリックします。

   ![](assets/six.png)

>[!MORELIKETHIS]
>
>* [ア追加カウントリストに対する既存の名前付きアカウント](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)
>* [アカウントリストインサイト](/help/marketo/product-docs/target-account-management/measure/account-list-insights.md)

