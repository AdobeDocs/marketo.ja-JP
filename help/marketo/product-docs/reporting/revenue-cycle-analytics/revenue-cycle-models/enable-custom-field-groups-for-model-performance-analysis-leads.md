---
unique-page-id: 3571890
description: モデル効果分析（リード）のカスタムフィールドグループの有効化 - Marketo ドキュメント - 製品ドキュメント
title: モデル効果分析（リード）のカスタムフィールドグループの有効化
exl-id: 417fd74f-d8f5-477b-b633-0fdfdd68b22b
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 66%

---

# モデル効果分析（リード）のカスタムフィールドグループの有効化 {#enable-custom-field-groups-for-model-performance-analysis-leads}

>[!PREREQUISITES]
>
>Marketo のフィールドオーガナイザーでレポート用に、標準フィールドまたはカスタムフィールドをグループに分類します。詳しくは、[フィールドオーガナイザーを使用したカスタムフィールドグループの作成](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/field-organizers/create-custom-field-groups-using-the-field-organizer.md)を参照してください。

<table>
 <tbody>
  <tr>
   <td colspan="3" rowspan="1"><p align="center"><strong>カスタムフィールドグループの有効化が収益サイクルエクスプローラーの複数の分析領域に与える影響</strong></p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>シナリオ</strong></p></td>
   <td colspan="1" rowspan="1"><p><strong><span class="uicontrol"> モデルパフォーマンス分析（リード） </span> 領域への影響</strong></p></td>
   <td colspan="1" rowspan="1"><p><strong>リード分析、キャンペーン分析、商談分析の各領域に与える影響</strong></p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>標準リードまたは会社フィールドに関連付けられたカスタムフィールドグループを有効にする</strong></p></td>
   <td colspan="1" rowspan="1"><p><span class="uicontrol"> モデルパフォーマンス分析（リード） </span> 領域のレポートに対して、カスタムフィールドグループが有効になっています</p></td>
   <td colspan="1" rowspan="1"><p>影響なし</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>ユーザー設定の個人または会社フィールドに関連付けられたカスタムフィールドグループを有効にする</strong></p></td>
   <td colspan="1" rowspan="1"><p><span class="uicontrol"> モデルパフォーマンス分析（リード） </span> 領域のレポートに対して、カスタムフィールドグループが有効になっています</p></td>
   <td colspan="1" rowspan="1"><p>カスタムフィールド自体が、リード分析、キャンペーン分析、商談分析エリアでのレポート作成に対して有効になる</p><p><strong>注意</strong>：これらの分析領域では、カスタムフィールドグループはサポートされていないので、グループの関連付けは収益サイクルエクスプローラーには表示されません。表示されるのはカスタムフィールド<em>のみ</em>です。</p></td>
  </tr>
 </tbody>
</table>

[!UICONTROL  モデルパフォーマンス分析（リード） ] 領域でレポート用のカスタムフィールドグループを有効にするには、次の手順に従います。

1. 「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/one-1.png)

1. 「**[!UICONTROL 収益サイクルアナリティクス]**」をクリックします。

   ![](assets/two-1.png)

1. 空のフィールドグループの横にある「**[!UICONTROL なし]**」をクリックします。既に 3 つのフィールドグループが有効になっていて、編集する場合は、変更するフィールドグループの名前をクリックします。

   ![](assets/three.png)

1. **[!UICONTROL フィールド]**&#x200B;ドロップダウンをクリックして、目的のものを選択します。

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >この例では、標準フィールド（状態）のカスタムフィールドグループを有効にしました。したがって、影響を受けるのは [!UICONTROL  モデル性能分析（リード） ] 領域のみでした。 ユーザーまたは会社のカスタムフィールドのカスタムフィールドグループが有効になっている場合、有効になっているグループは「同期の概要」タブの [!UICONTROL  モデル性能分析（リード） ] セクションに表示され、リード、キャンペーンおよび商談分析のカスタムフィールドの数が 1 増えます。

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/five-1.png)
