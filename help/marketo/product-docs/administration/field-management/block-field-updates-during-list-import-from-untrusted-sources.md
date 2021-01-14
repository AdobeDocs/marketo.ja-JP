---
unique-page-id: 2360335
description: 信頼できないソースからのリストインポート中にフィールドの更新をブロックする — Marketto Docs — 製品ドキュメント
title: 信頼できないソースからのリストインポート中にフィールドの更新をブロックする
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---


# 信頼できないソースからのリストインポート中にフィールドの更新をブロックする{#block-field-updates-during-list-import-from-untrusted-sources}

一部のリストのデータを他のユーザーよりも信頼できます。 場合によっては、疑わしいデータが存在し、フィールドが空白の場合は取得し、既存の値がある場合は取得しないことがあります。 これを行うには、キーフィールドのフィールドの更新をブロックします。

>[!NOTE]
>
>**必要な管理者権限**

## 信頼できないソースからのフィールドの更新をブロックする{#blocking-field-updates-from-untrusted-sources}

1. **管理者**&#x200B;に移動し、**フィールド管理**&#x200B;をクリックします。

   ![](assets/image2014-9-19-9-3a38-3a38.png)

1. 目的のフィールドを探して選択し、「**フィールドアクション**」で「**フィールドの更新をブロック**」をクリックします。

   ![](assets/image2014-9-19-9-3a39-3a40.png)

1. 「**リストインポートの信頼できないソース**」をチェックし、「**適用**」をクリックします。

   ![](assets/blockupdates.png)

>[!TIP]
>
>**リスト信頼できるソースのインポート**&#x200B;をチェックすることで、信頼できる、信頼できないすべてのリストからフィールドを安全に保つことができます。

信頼できないリストに対して安全を確保する他のフィールドに対して、上記の手順を繰り返します。

## 信頼できないリストインポートの実行{#running-an-untrusted-list-import}

1. リストのインポートを実行する際、前の手順で設定したすべてのフィールドを安全にする場合は、「**信頼できない**」を必ず選択してください。

   ![](assets/importpersondetails.jpg)

リストをインポートする手順について詳しくは、[人のリストをインポート](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)を参照してください。

お疲れさま！ これで、重要なフィールドを信頼できないリストから守る方法が分かりました。
