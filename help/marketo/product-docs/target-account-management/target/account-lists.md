---
unique-page-id: 11378814
description: アカウントリストと、ターゲティング用に名前付きアカウントをグループ化する方法について説明します。 CRM アカウントビューから、静的リストまたは動的リストを作成します。
title: '[!UICONTROL アカウントリスト]'
exl-id: 31bb4341-d012-4239-8f40-10a07cd4c51c
feature: Target Account Management
TQID: 'https://experienceleague.adobe.com/fNIkaF84ELk9RJAxA9PK9rFlaEkNwia9sbgqsHOBOMI'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
    internal-label: Personalization
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
subfeature_v2:
  - id: fd4ca7b1-bd80-47f4-ad1a-846912e45cc5
    internal-label: Target Account Management
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 93%
---
# [!UICONTROL アカウントリスト] {#account-lists}

顧客リストは、一緒にターゲット設定できる重点顧客の集まりです。 アカウントリストを使用すると、重点アカウントを業種、所在地、または会社の規模別にターゲット設定できます。

アカウントリストに加えて、公開されている CRM アカウントビューから生成される動的アカウントリストも作成できます。 CRM アカウントビューは、アカウントを表示する際にフィルターとして機能する一連のルールです。 例えば、業界がヘルスケアで、*かつ*&#x200B;売上高が 1 億ドルを超えるアカウントを検索する場合に使用できます。

![](assets/one.png)

>[!NOTE]
>
>Marketo [!UICONTROL ターゲットアカウント管理]で作成されたアカウントリストは、[web パーソナライゼーション](/help/marketo/product-docs/web-personalization/using-web-segments/web-segments.md)でスマートリストと web キャンペーンを作成するときに自動的に使用できるようになります。

## 新規アカウントリストの作成&#x200B; {#create-a-new-account-list}

1. **[!UICONTROL 新規作成]**&#x200B;ドロップダウンをクリックして、「**[!UICONTROL 新規顧客リストを作成]**」を選択します。

   ![](assets/1a.png)

1. リストに名前を付け、「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/three-0.png)

1. 顧客リストを作成したら、[重点顧客を追加](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)し始めます。

   >[!NOTE]
   >
   >Marketo では、重点アカウントが 2,000 件以下のアカウントリストに関するインサイトのみが表示されます。

## 新規動的アカウントリストの作成 {#create-a-new-dynamic-account-list}

1. **[!UICONTROL 新規作成]**&#x200B;ドロップダウンをクリックして、「**[!UICONTROL 新規動的顧客リストを作成]**」を選択します。

   ![](assets/1.png)

1. ダイアログで、「**CRM 顧客ビュー**」をクリックするか、名前を入力して検索します。

   ![](assets/image2017-7-18-9-48-23.png)

1. 「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/step4.jpg)

   >[!NOTE]
   >
   >Salesforce では、同期ユーザーに対してリスト表示オブジェクトの権限を必ず指定してください。

## アカウントリストの名前変更 {#rename-an-account-list}

>[!NOTE]
>
>これらの手順は、アカウントリストにのみ適用されます。 *動的*&#x200B;顧客リストは、関連する CRM 顧客ビューの名前を使用します。

1. 名前を変更する顧客を選択し、**[!UICONTROL 顧客リストのアクション]**&#x200B;ドロップダウンをクリックして「**[!UICONTROL 顧客リストを名前変更]**」を選択します。

   ![](assets/three.png)

1. 新しい名前を入力し、「**[!UICONTROL 名前変更]**」をクリックします。

   ![](assets/four.png)

   >[!NOTE]
   >
   >CRM アカウントビューは、8 時間ごとに動的アカウントリストと同期します。 まだ同期されていない場合、Marketo は次のサイクルで同期します。

## アカウントリストの削除 {#delete-an-account-list}

>[!NOTE]
>
>これらの手順は、アカウントリストと動的アカウントリストの両方で同じです。

1. 削除する顧客を選択し、**[!UICONTROL 顧客リストのアクション]**&#x200B;ドロップダウンをクリックして「**[!UICONTROL 顧客リストを削除]**」を選択します。

   ![](assets/five.png)

1. 「**[!UICONTROL 削除]**」をクリックします。

   ![](assets/six.png)

>[!MORELIKETHIS]
>
>* [既存の[!UICONTROL 重点顧客]をアカウントリストに追加](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)
>* [アカウントリストインサイト](/help/marketo/product-docs/target-account-management/measure/account-list-insights.md)
