---
unique-page-id: 10098379
description: 新しいカスタムフィールドに対する Microsoft Dynamics とのクイック同期の使用 - Marketo ドキュメント - 製品ドキュメント
title: 新しいカスタムフィールドに対する Microsoft Dynamics とのクイック同期の使用
exl-id: c98f1443-c0dd-40e1-919b-f8110088b38a
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 94%

---

# 新しいカスタムフィールドに対する Microsoft Dynamics とのクイック同期の使用 {#use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field}

マーケティングまたはセールスが新しいフィールドを希望しています。または、最初のフィールド選択で 1 つ選択し忘れた場合もあります。または、ニーズが変更された場合も考えられます。どのような場合でも、クイック同期を使用して特定のフィールドを再同期できます。

通常は、クイック同期を使用して新しいフィールドを追加し、値を更新します。 ただし、既存のフィールドを同期する場合もあります。更新または作成した日付範囲に基づいて、フィールドの同期を制限できます。詳しくは、以下の[詳細同期オプション](#Advanced_Sync_Options)を参照してください。

クイック同期では、null 値を同期できます。例えば、A と B の値を使用し、Dynamics の B 値を null に変更すると、null 値が Marketo に同期されます。

## すべてのレコードのクイック同期 {#quick-sync-for-all-records}

ここでは、クイック同期を使用して新しいフィールドを再同期する方法を説明します。

1. Marketo Engage で、「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/image2016-8-19-11-3a14-3a5.png)

1. 「**[!UICONTROL Microsoft Dynamics]**」をクリックします。

   ![](assets/image2016-8-19-11-3a15-3a8.png)

1. 「フィールド同期の詳細」で、「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2016-8-19-11-3a16-3a22.png)

1. クイック同期するフィールドを選択し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2016-8-25-15-3a26-3a11.png)

   >[!NOTE]
   >
   >複数のエンティティからフィールドを選択できます。

1. 同期が完了すると、通知が届きます。

   ![](assets/field-sync-update-notification.png)

   >[!CAUTION]
   >
   >同期は他の同期と並行して実行され、データベースのサイズによっては、完了までに長い時間がかかる場合があります。同期待ちのキューに入っているフィールドの選択を解除することはできません。

## 詳細同期オプション {#advanced-sync-options}

既存のフィールドを限られたデータセットに対してのみ同期する場合は、どうすればいいですか？手順は以下のとおりです。

1. 既存のフィールドのチェックボックスをオフにします。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2016-8-25-16-3a16-3a32.png)

1. ポップアップを再度開き、フィールドを再選択します。

   ![](assets/select-field-reselect-hand.png)

1. 「**[!UICONTROL 詳細同期]**」をクリックします。

   ![](assets/image2016-8-25-15-3a52-3a9.png)

1. 「**[!UICONTROL 更新済み]**」を選択し、日付選択ツールを使用して日付範囲を選択します。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2016-8-25-16-3a0-3a3.png)

   フィールドのクイック同期は、2016/8/19～2016/9/16 の間に更新されたレコードにのみ実行されます。

## 非同期フィールドの修正 {#fixing-out-of-sync-fields}

まれに、Dynamics と Marketo のフィールドが同期していない場合は、素早く簡単に再同期できます。

1. フィールドの選択を解除し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2016-8-25-16-3a16-3a32-1.png)

1. フィールドを再選択し、「**[!UICONTROL 保存]** をクリックします。

   ![](assets/image2016-8-25-16-3a20-3a45.png)

   これで修正されます。
