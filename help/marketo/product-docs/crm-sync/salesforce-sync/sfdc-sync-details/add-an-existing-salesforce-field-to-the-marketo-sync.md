---
unique-page-id: 4719308
description: 既存の Salesforce フィールドの Marketo  同期への追加 - Marketo ドキュメント - 製品ドキュメント
title: 既存の Salesforce フィールドの Marketo 同期への追加
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: ht
source-wordcount: '158'
ht-degree: 100%

---

# 既存の Salesforce フィールドの Marketo 同期への追加 {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**管理者権限が必要**

通常、Salesforce の新しいカスタムフィールドは Marketo に自動的に同期されます。そうでない場合、Marketo 同期ユーザーにはフィールドが表示されない場合があります。この問題の修正方法を次に示します。

1. 名前をクリックし、「**設定**」を選択します。

   ![](assets/image2015-6-30-14-3a20-3a6.png)

1. 左の検索バーで「**プロファイル**」と入力し、「**ユーザーを管理**」の下の「**プロファイル**」をクリックします。

   ![](assets/image2015-6-30-14-3a20-3a52.png)

1. 同期ユーザーのプロファイルをクリックします。

   ![](assets/image2015-6-30-14-3a23-3a41.png)

1. **フィールドレベルのセキュリティ**&#x200B;セクションで、フィールドを含むオブジェクトの横にある「**表示**」をクリックします。

   ![](assets/image2015-6-30-14-3a23-3a59.png)

1. 「**編集**」をクリックします。

   ![](assets/image2015-6-30-14-3a24-3a28.png)

1. 同期に追加するフィールドの「**表示**」のチェックをオンにし、「**保存**」をクリックします。

   ![](assets/image2015-6-30-14-3a24-3a49.png)

   できましたね。次の同期サイクルで、Marketo はフィールドを表示し、マジックを開めます。

   >[!NOTE]
   >
   > フィールドに既に Salesforce の値が含まれている場合、これらの値は次のレコードがアップデートされるまで Marketo に同期されません。
