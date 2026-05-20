---
unique-page-id: 2360309
description: ワークスペースでマーケティングアセットを整理する方法と、個人のパーティションを個別のデータベースとして機能させる方法について説明します。
title: ワークスペースと人物パーティションについて
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
feature: Partitions, Workspaces
TQID: https://experienceleague.adobe.com/Ex-WBSNYTFvevcwryuO4CzUsg79nOmjkVx4WMUx9nqA
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 551
ht-degree: 78%

---

# ワークスペースと人物パーティションについて {#understanding-workspaces-and-person-partitions}

## ワークスペース {#workspaces}

>[!CAUTION]
>
>ワークスペースは、設定が複雑になる場合があります。 [Marketo サポート &#x200B;](https://nation.marketo.com/t5/Support/ct-p/Support)に連絡して、お客様に適しているかどうかを確認してください。

ワークスペースは Marketo の別の領域で、プログラム、ランディングページ、電子メールなどのマーケティングアセットが格納されます。 複数のユーザーが使用できます。 各ユーザーは、1 つ以上のワークスペースにアクセスできます。

>[!NOTE]
>
>**例**
>
>ワークスペースを使用する理由をいくつか示します。
>
>* 地域：ヨーロッパ、アジア、北米のマーケティング部門にそれぞれワークスペースがあります
>* ビジネスユニット：[!DNL Quicken]、[!DNL Quickbooks]、[!DNL TurboTax] にそれぞれワークスペースがあります
>
>いずれの場合も、分離する理由は、マーケティングアセットが完全に異なるからです。 マーケティングアセットを共有している場合、ワークスペースは適切なツールではないかもしれません。

>[!NOTE]
>
>[新しいワークスペースを作成する方法](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md)について説明します。

## ワークスペース間での共有 {#sharing-across-workspaces}

次の手順では、ワークスペース間でアセットを共有する方法を説明します。 共有するものに対してどれも同じように機能します。この例は、セグメント化を示しています。

>[!NOTE]
>
>アセットを含む親フォルダーは、共有できる唯一のフォルダーで、子フォルダーは共有できません。

1. 「**[!UICONTROL データベース]**」をクリックします。

   ![](assets/understanding-workspaces-and-person-partitions-1.png)

1. セグメント化フォルダーを右クリックし、「**[!UICONTROL 新規フォルダー]**」をクリックします。

   ![](assets/understanding-workspaces-and-person-partitions-2.png)

1. フォルダーに名前を付け、「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/understanding-workspaces-and-person-partitions-3.png)

1. 共有するアセットをフォルダーに移動します。

   ![](assets/understanding-workspaces-and-person-partitions-4.png)

1. フォルダーを右クリックし、「**[!UICONTROL フォルダーを共有]**」を選択します。

   ![](assets/understanding-workspaces-and-person-partitions-5.png)

1. フォルダーを共有するワークスペースを選択して、「**[!UICONTROL 保存]**」をクリックします。 フォルダーを共有ダイアログボックスには、表示権限を持つワークスペースのみが表示されます。

   ![](assets/understanding-workspaces-and-person-partitions-6.png)

   >[!NOTE]
   >
   >元のフォルダーには、共有されたことを示す小さな緑色の矢印が表示されます。 共有されたワークスペースには、読み取り専用を示す南京錠アイコンが表示されます。

これらの項目は、ワークスペースをまたいで共有できます。

* メールテンプレート
* ランディングページテンプレート
* モデル
* スマートキャンペーン
* [スマートリスト](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [セグメント化](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* スニペット

## ワークスペース間での複製 {#cloning-across-workspaces}

テンプレート以外のアセットの場合は、プログラム内のローカルアセットとして複製することをお勧めします。 適切なアクセスレベルで、以下のアセットを別のワークスペースにドラッグ＆ドロップできます。

* プログラム
* メール
* ランディングページ
* フォーム

>[!IMPORTANT]
>
>上記の項目はすべて Workspaces で複製できますが、メール、フォーム、ランディングページは、複製時に&#x200B;_プログラム内に存在する必要_&#x200B;があります。

>[!NOTE]
>
>テンプレートを持つアセットの複製を作成する場合は、それらのテンプレートを宛先ワークスペースと共有する必要があります。

## アセットを他のワークスペースに移動 {#moving-assets-to-other-workspaces}

アセットを新しいワークスペースに移動するには、アセットをフォルダーに配置し、そのフォルダーを別のワークスペースにドラッグします。

>[!NOTE]
>
>メンバーを含むプログラムをワークスペース間で移動することはできません。

## 人物パーティション {#person-partitions}

人物パーティションは、個別のデータベースのように動作します。 各パーティションには、重複排除したり他のパーティションと混在したりしない、独自の人物が存在します。 ビジネスの使用例で、同じ電子メールアドレスを持つ重複したレコードが必要な場合は、[Marketo サポート &#x200B;](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。

人物パーティションを[ワークスペース](create-a-new-workspace.md)に割り当てるには、以下の設定に従います。

* 1 つのワークスペースに対して 1 つの人物パーティション（1:1）
* 1 つのワークスペースに対して多数の人物パーティション （1:x）
* 多数のワークスペースに対して 1 つの人物パーティション（x:1）

>[!NOTE]
>
>人物パーティションを使用する理由：
>
>* ワークスペースには異なるアセットがあるだけでなく、誰も共有しません
>* その他のビジネス上の理由から重複が必要な場合

>[!CAUTION]
>
>人物パーティションは相互にやり取りしないので、設定する際は注意してください。

>[!NOTE]
>
>[人物パーティションの作成](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)方法をご確認ください。
