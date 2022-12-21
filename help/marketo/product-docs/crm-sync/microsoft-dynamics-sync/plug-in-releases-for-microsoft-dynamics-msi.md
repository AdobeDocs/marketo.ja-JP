---
unique-page-id: 10099102
description: Microsoft Dynamics MSI 向けプラグインリリース - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics MSI 向けプラグインリリース
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
source-git-commit: ff076d66a193664aa6ec05cf940143cebdd2d942
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 81%

---

# Microsoft Dynamics MSI 向けプラグインリリース {#plug-in-releases-for-microsoft-dynamics-msi}

Microsoft Dynamics に初めて同期するときは、Marketo Sales Insight（MSI）用の最新バージョンのプラグインをダウンロードしてインストールします。Marketo は定期的にこれらのプラグインを更新するので、同じ場所に戻って新しいバージョンをダウンロードできます。

Marketoのネイティブ CRM 同期ソリューションを Dynamics に使用している場合は、 [最新のプラグインのダウンロード](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md){target=&quot;_blank&quot;} は、Dynamics リリースに対応しています。 カスタム同期を実行し、Marketo Sales Insight を購入済みの場合は、[パッケージはここにあります](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target=&quot;_blank&quot;}。

>[!NOTE]
>
>これらのバージョンは、Dynamics のオンプレミスバージョンとオンラインバージョンの両方で機能します。

## MSI ソリューションのアップグレード {#upgrading-your-msi-solution}

1. Dynamics の「_インポート_」ボタンを押して、Dynamics CRM の&#x200B;**既存のバージョンに**&#x200B;最新バージョンのソリューションをインポートします。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>例：Dynamics CRM のバージョンが 2.0.0.20 で、最新バージョンが 2.0.0.21 の場合は、2.0.0.20 _以降_&#x200B;のバージョンをインポートします。

1. 「**次へ**」をクリックします。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. 「**アップグレードのステージ**」および「**カスタマイズを維持**」を選択し、「**インポート**」をクリックします。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. 「**次へ**」をクリックします。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. インポートが正常に完了すると、MarketoSalesInsight と MarketoSalesInsight_Upgrade の 2 つの MSI ソリューションが表示されます。古いソリューションを選択し、「ソリューションアップグレードを適用」をクリックします。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

これで完了です。アップグレード後は、1 つの MSI ソリューションのみが表示されます。

## バージョンの更新 {#version-updates}

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
   <th colspan="1">注意</th> 
  </tr> 
  <tr> 
   <td colspan="1">02/03/22</td> 
   <td colspan="1">2.0.0.27</td> 
   <td colspan="1">インサイト用のアカウントレイアウト：注目のアクション、スコアの変更、Web アクティビティ、E メールアクティビティ</td> 
  </tr>
  <tr> 
   <td colspan="1">01/05/22</td> 
   <td colspan="1">2.0.0.26</td> 
   <td colspan="1">送信メール用のプログラム採用スコア</td> 
  </tr>
  <tr> 
   <td colspan="1">10/28/21</td> 
   <td colspan="1">2.0.0.25</td> 
   <td colspan="1">製品採用スコア指標、新しいグローバルダッシュボード（Web アクティビティ、E メール、最適）</td> 
  </tr>
  <tr> 
   <td colspan="1">02/10/21</td> 
   <td colspan="1">2.0.0.22</td> 
   <td colspan="1">自動監査を削除し、MSI ソリューションのドキュメントの変更を削除します</td> 
  </tr>
  <tr> 
   <td colspan="1">10/01/20</td> 
   <td colspan="1">2.0.0.21</td> 
   <td colspan="1">バグ修正：Sales Insight の役割を持つユーザーの MSI API 設定フィールドへのアクセスの割り当て</td> 
  </tr> 
  <tr> 
   <td colspan="1">2020/07/20</td> 
   <td colspan="1">2.0.0.20</td> 
   <td colspan="1">バグ修正：非同期レコードの検証メッセージを追加</td> 
  </tr> 
  <tr> 
   <td colspan="1">2020/06/12</td> 
   <td colspan="1">2.0.0.19</td> 
   <td colspan="1">バグ修正：MSD API 設定で MSI シークレットパスワードを非表示に</td> 
  </tr> 
  <tr> 
   <td colspan="1">2020/05/26</td> 
   <td colspan="1">2.0.0.18</td> 
   <td colspan="1">バグ修正：「MSI」ボタンを表示するために MSI 役割 ID の検証を変更</td> 
  </tr> 
  <tr> 
   <td colspan="1">2020/05/21</td> 
   <td colspan="1">2.0.0.17</td> 
   <td colspan="1">バグ修正：所有者フィールドを再表示し、フィールドを必須にしないように設定</td> 
  </tr> 
  <tr> 
   <td colspan="1">2020/04/28</td> 
   <td colspan="1">2.0.0.16</td> 
   <td colspan="1">バグ修正：MSD CRM サイトマップ設定のリンク依存関係を削除</td> 
  </tr> 
 </tbody> 
</table>
