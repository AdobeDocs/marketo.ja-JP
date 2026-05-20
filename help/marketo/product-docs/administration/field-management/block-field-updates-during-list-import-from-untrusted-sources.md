---
unique-page-id: 2360335
description: 信頼できないソースからリストをインポートする際に、主要なフィールドが上書きされるのをブロックし、既存のデータを保護します。
title: 信頼できないソースからのリストインポート中に、フィールドの更新をブロック
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
feature: Field Management
TQID: https://experienceleague.adobe.com/cT1pOoWjR-UdHLqNJwhwgR9R12ciIa95q1xHPTf7rBY
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 205
ht-degree: 76%

---

# 信頼できないソースからのリストインポート中に、フィールドの更新をブロック {#block-field-updates-during-list-import-from-untrusted-sources}

一部のリストのデータは、他のリストよりも信頼できます。 疑わしいデータがあり、フィールドが空白の場合はデータを受け入れたいが、既存の値がある場合は受け入れない場合があります。 これは、キーフィールドのフィールド更新をブロックすることで実現できます。

>[!NOTE]
>
>**管理者権限が必要**

## 信頼できないソースからのフィールド更新をブロック {#blocking-field-updates-from-untrusted-sources}

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. 「**[!UICONTROL フィールド管理]**」をクリックします。

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. 目的のフィールドを探して選択し、「**[!UICONTROL フィールドアクション]**」で「**[!UICONTROL フィールドの更新をブロック]**」をクリックします。

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. 「**[!UICONTROL 信頼できないソースのリストをインポート]**」をチェックし、「**[!UICONTROL 適用]**」をクリックします。

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>また、「**[!UICONTROL 信頼できるソースのリストをインポート]**」もチェックすることで、信頼できるリスト、信頼できないリスト、すべてのリストからフィールドを安全に保つことができます。

信頼できないリストから安全に保つその他のフィールドに対して、上記の手順を繰り返します。

## 信頼できないリストのインポートの実行 {#running-an-untrusted-list-import}

1. リストのインポートを実行するにあたり、前の手順で設定したすべてのフィールドを安全にする場合は、必ず「**[!UICONTROL 信頼できない]**」を選択します。

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

リストのインポートの詳しい手順については、[人物のリストのインポート](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)を参照してください。

キーフィールドが信頼できないリストの読み込みから保護されるようになりました。
