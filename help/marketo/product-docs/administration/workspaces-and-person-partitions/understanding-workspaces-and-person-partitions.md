---
unique-page-id: 2360309
description: ワークスペースと人物パーティションについて - Marketo ドキュメント - 製品ドキュメント
title: ワークスペースと人物パーティションについて
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 100%

---

# ワークスペースと人物パーティションについて {#understanding-workspaces-and-person-partitions}

## ワークスペース {#workspaces}

>[!CAUTION]
>
>ワークスペースは、設定が複雑になる場合があります。ワークスペースが最適かどうか確認するには、[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。

ワークスペースは Marketo の別の領域で、プログラム、ランディングページ、電子メールなどのマーケティングアセットが格納されます。複数のユーザーが使用できます。各ユーザーは、1 つ以上のワークスペースにアクセスできます。

>[!NOTE]
>
>**例**
>
>ワークスペースを使用する理由をいくつか示します。
>
>* 地域：ヨーロッパ、アジア、北米のマーケティング部門にそれぞれワークスペースがあります
>* ビジネスユニット：Quicken、Quickbooks、TurboTax にそれぞれワークスペースがあります
>
>いずれの場合も、分離する理由は、マーケティングアセットが完全に異なるからです。マーケティングアセットを共有している場合、ワークスペースは適切なツールではないかもしれません。

>[!NOTE]
>
>[新規ワークスペースの作成](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md)方法をご確認ください。

## ワークスペース間での共有 {#sharing-across-workspaces}

ワークスペースをまたいでアセットを共有する方法を説明します。共有するものに対してどれも同じように機能します。この例は、セグメント化を示しています。

>[!NOTE]
>
>アセットを含む親フォルダーは、共有できる唯一のフォルダーで、子フォルダーは共有できません。

1. 新規フォルダーの作成。

   ![](assets/one.png)

1. 共有するフォルダーに名前を付けます。

   ![](assets/two.png)

1. 共有するアセットをフォルダーに移動します。

   ![](assets/three.png)

1. フォルダーを右クリックし、「**フォルダーを共有**」を選択します。

   ![](assets/four.png)

1. フォルダーを共有するワークスペースを選択して、「**保存**」をクリックします。フォルダーを共有ダイアログボックスには、表示権限を持つワークスペースのみが表示されます。

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >元のフォルダーに、小さな緑の矢印が表示され、共有されたことを示します。共有されたワークスペースには、読み取り専用を示す南京錠アイコンが表示されます。

これらの項目は、ワークスペースをまたいで共有できます。

* メールテンプレート
* ランディングページテンプレート
* モデル
* スマートキャンペーン
* [スマートリスト](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [セグメンテーション](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* スニペット

## ワークスペース間での複製 {#cloning-across-workspaces}

テンプレート以外のアセットの場合は、プログラム内でローカルアセットとして複製するのが最適です。適切なアクセスレベルで、次のアセットを別のワークスペースにドラッグ＆ドロップできます。

* プログラム
* メール
* ランディングページ
* フォーム

>[!NOTE]
>
>テンプレートを持つアセットの複製を作成する場合は、それらのテンプレートを宛先ワークスペースと共有する必要があります。

## アセットを他のワークスペースに移動 {#moving-assets-to-other-workspaces}

アセットを新しいワークスペースに移動するには、アセットをフォルダーに配置し、そのフォルダーを別のワークスペースにドラッグします。

>[!NOTE]
>
>メンバーを含むプログラムを別のワークスペースに移動することはできません。

## 人物パーティション {#person-partitions}

人物パーティションは、個別のデータベースのように動作します。各パーティションには、重複排除したり他のパーティションと混在したりしない、独自の人物が存在します。同じメールアドレスを持つ重複レコードの作成が必要なビジネスユースケースがあると思われる場合は、[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。

人物パーティションを[ワークスペース](create-a-new-workspace.md)に割り当てるには、次の設定に従います。

* 1 つのワークスペースと 1 つの人物パーティション（1：1）
* 1 つのワークスペースに対して多数の人物パーティション （1：x）
* 多数のワークスペースに対して 1 つの人物パーティション（x：1）

>[!NOTE]
>
>人物パーティションを使用する理由：
>
>* ワークスペースに異なるアセットがあるだけでなく、他のユーザーとも共有しません
>* その他のビジネス上の理由から重複が必要な場合


>[!CAUTION]
>
>人物パーティションは相互にやり取りしないので、設定する際は注意してください。

>[!NOTE]
>
>[人物パーティションの作成](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)方法をご確認ください。
