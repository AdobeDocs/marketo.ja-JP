---
unique-page-id: 2360327
description: 割り当てルールを使用した人物パーティションの割り当て - Marketo ドキュメント - 製品ドキュメント
title: 割り当てルールを使用した人物パーティションの割り当て
exl-id: 6b54dcb7-8da9-466b-b153-099ebcb96424
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '167'
ht-degree: 100%

---

# 割り当てルールを使用した人物パーティションの割り当て {#assigning-person-partitions-with-assignment-rules}

>[!NOTE]
>
>**管理者権限が必要**

>[!PREREQUISITES]
>
>[人物パーティションの作成](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)

人物パーティションを使用する場合、CRM から作成された人物をそれぞれのパーティションにルーティングする割り当てルールを設定します。

>[!NOTE]
>
>CRM から Marketo で作成され、SOAP API を介して作成された人物のみに割り当てルールが適用されます。

1. 「管理者」で「ワークスペースとパーティション」をクリックします。

   ![](assets/image2014-9-17-10-3a32-3a55.png)

1. 「**人物パーティション**」タブで、「**割り当てルール**」をクリックします。

   ![](assets/two-6.png)

1. 「**選択肢を追加**」をクリックして、人物パーティションに人物をルーティングする条件を追加します。

   ![](assets/three-6.png)

1. 条件を作成するフィールドを選択します。

   ![](assets/four-5.png)

1. 選択肢の演算子を選択して、値を入力します。

   ![](assets/five-1.png)

1. 条件を満たす人物を対象にする人物パーティションを選択します。

   ![](assets/six-1.png)

   >[!NOTE]
   >
   >選択肢は好きなだけ追加できます。

1. 「**保存**」をクリックします。

   ![](assets/seven.png)

これで手順は完了です。人物パーティションを人物で満たすためのルールを割り当てました。

>[!NOTE]
>
>以前の条件が満たされない場合、デフォルトの選択肢が適用されます。
