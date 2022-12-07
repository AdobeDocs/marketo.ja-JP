---
unique-page-id: 2360335
description: 信頼できないソースからのリストのインポート中にフィールドの更新をブロック - Marketo ドキュメント - 製品ドキュメント
title: 信頼できないソースからのリストインポート中に、フィールドの更新をブロック
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 100%

---

# 信頼できないソースからのリストインポート中に、フィールドの更新をブロック {#block-field-updates-during-list-import-from-untrusted-sources}

一部のリストのデータは、他のリストよりも信頼できます。疑わしいデータを、フィールドが空白の場合は取得し、既存の値が存在する場合は取得したくない場合があります。これは、キーフィールドのフィールド更新をブロックすることで実現できます。

>[!NOTE]
>
>**管理者権限が必要**

## 信頼できないソースからのフィールド更新をブロック {#blocking-field-updates-from-untrusted-sources}

1. 「**管理者**」領域に移動します。

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. 「**フィールド管理**」をクリックします。

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. 目的のフィールドを探して選択し、「**フィールドアクション**」で「**フィールドの更新をブロック**」をクリックします。

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. 「**信頼できないソースのリストをインポート**」をチェックし、「**適用**」をクリックします。

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>また、「**信頼できるソースのリストをインポート**」もチェックすることで、信頼できるリスト、信頼できないリスト、すべてのリストからフィールドを安全に保つことができます。

信頼できないリストから安全に保つその他のフィールドに対して、上記の手順を繰り返します。

## 信頼できないリストのインポートの実行 {#running-an-untrusted-list-import}

1. リストのインポートを実行するにあたり、前の手順で設定したすべてのフィールドを安全にする場合は、必ず「**信頼できない**」を選択します。

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

リストのインポートの詳しい手順については、[人物のリストのインポート](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)を参照してください。

お疲れさまでした。これで、キーフィールドを信頼できないリストから安全に保つ方法を理解できました。
