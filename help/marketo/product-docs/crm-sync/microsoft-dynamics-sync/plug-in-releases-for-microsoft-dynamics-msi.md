---
unique-page-id: 10099102
description: Microsoft Dynamics MSI用プラグインリリース — Marketto Docs — 製品ドキュメント
title: Microsoft Dynamics MSIのプラグインリリース
translation-type: tm+mt
source-git-commit: d1d74e24c07578b1b0c2696c08fe5a5be543cce8
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 4%

---


# Microsoft Dynamics MSI {#plug-in-releases-for-microsoft-dynamics-msi}のプラグインリリース

Microsoft Dynamicsとの最初の同期時には、Marketo Sales Insight(MSI)用の最新バージョンのプラグインをダウンロードしてインストールします。 定期的にMarketing Suiteでこれらのプラグインが更新されるので、同じ場所に戻って新しいバージョンをダウンロードできます。

[お使いのDynamicsリリースに対応する最新のプラグイン](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md)をダウンロードしてください。

>[!NOTE]
>
>これらのバージョンは、オンプレミスとオンラインの両方のDynamicsで機能します。

## MSIソリューションをアップグレード{#upgrading-your-msi-solution}

1. Dynamicsの&#x200B;**「**&#x200B;インポート」ボタンを押して、Dynamics CRMの既存のバージョン&#x200B;_に対してソリューション_&#x200B;の最新バージョンをインポートします。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>例：Dynamics CRMにバージョン2.0.0.20が搭載され、最新バージョンが2.0.0.21の場合は、_over_&#x200B;バージョン2.0.0.20をインポートします。

1. 「**次へ**」をクリックします。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. 「**アップグレードのステージ**」と「**カスタマイズを維持**」を選択し、「**読み込み**」をクリックします。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. 「**次へ**」をクリックします。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. インポートが正常に完了すると、次の2つのMSIソリューションが表示されます。MarketoSalesInsightとMarketoSalesInsight_Upgrade 古いソリューションを選択し、「Apply Solution Upgrade」をクリックします。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

それだ！ アップグレード後は、1つのMSIソリューションしか表示されません。

## バージョンの更新{#version-updates}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th colspan="1">リリース日</th> 
   <th colspan="1">バージョン</th> 
   <th colspan="1">メモ</th> 
  </tr> 
  <tr> 
   <td colspan="1">10/1/20</td> 
   <td colspan="1">2.0.0.21</td> 
   <td colspan="1">バグ修正：Sales Insightロールを持つユーザー用のMSI API設定フィールドへのアクセス権の割り当て</td> 
  </tr> 
  <tr> 
   <td colspan="1">07/20/20</td> 
   <td colspan="1">2.0.0.20</td> 
   <td colspan="1">バグ修正：非同期レコード追加の検証メッセージ</td> 
  </tr> 
  <tr> 
   <td colspan="1">06/12/20</td> 
   <td colspan="1">2.0.0.19</td> 
   <td colspan="1">バグ修正：MSD API設定でMSIシークレットパスワードを非表示にするには</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/26/20</td> 
   <td colspan="1">2.0.0.18</td> 
   <td colspan="1">バグ修正：MSIボタンを表示するためのMSIロールID検証を変更するには</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/21/20</td> 
   <td colspan="1">2.0.0.17</td> 
   <td colspan="1">バグ修正：所有者フィールドの再表示と必須フィールド以外のフィールドへの変更</td> 
  </tr> 
  <tr> 
   <td colspan="1">04/28/20</td> 
   <td colspan="1">2.0.0.16</td> 
   <td colspan="1">バグ修正：MSD CRMサイトマップ設定のリンクの依存関係を削除しています</td> 
  </tr> 
 </tbody> 
</table>
