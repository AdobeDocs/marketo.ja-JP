---
unique-page-id: 10099389
description: Microsoft Dynamics用Marketoプラグインリリース —Marketoドキュメント — 製品ドキュメント
title: Microsoft Dynamics用Marketoプラグインリリース
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 7%

---

# Microsoft Dynamics用Marketoプラグインリリース{#marketo-plugin-releases-for-microsoft-dynamics}

Microsoft Dynamicsとの初回同期時に、Marketo用プラグインの最新バージョンをダウンロードします。 定期的に、Marketoがこれらのプラグインを更新するので、同じ場所に戻って新しいバージョンをダウンロードできます。

[ご使用のDynamicsリリースに対応する最新の](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) プラグインをダウンロードします。

![](assets/lead-management-solution.png)

## Dynamics Solutionを更新しています{#updating-your-dynamics-solution}

1. Dynamics CRMの既存のバージョンを使用して、ソリューションの最新バージョンをインポートします(例：Dynamics CRMにバージョン1.4があり、最新バージョンが1.5の場合は、_over_&#x200B;バージョン1.4)をインポートします。

1. 次のポップアップが表示されます。 「**更新**」および「**カスタマイズを維持**」を選択し、「**読み込み**」をクリックします。

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## 最新バージョン{#latest-versions}

>[!NOTE]
>
>これらのバージョンは、オンプレミスとオンラインの両方のDynamicsで機能します。

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">バージョン</th> 
   <th colspan="1">リリース日</th> 
   <th>注意</th> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.0</td> 
   <td colspan="1">10/16/20</td> 
   <td colspan="1">MS Dynamicsとのキャンペーン同期のサポートが追加されました。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.24</td> 
   <td colspan="1">8/22/18</td> 
   <td colspan="1">Microsoft Dynamics Version 9.xの問い合わせプロセスに、すぐに利用できる条件を満たすリードのサポートが追加されました。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.23</td> 
   <td colspan="1">6/27/18</td> 
   <td colspan="1">バグ修正：Dynamics 2013用Marketoソリューションのインストール中にビジネスプロセスエラーが発生しました。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.22</td> 
   <td colspan="1">9/29/17</td> 
   <td colspan="1">バグ修正：内部リビジョン。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><p>4.0.0.21</p></td> 
   <td colspan="1">11/9/16</td> 
   <td colspan="1">バグ修正：プラグインは、カスタムオブジェクトの状態変更をキャプチャするイベントをサブスクライブしませんでした。 この修正は、Dynamics CRM On Premise 2011に固有のものです。 </td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.20</td> 
   <td colspan="1">7/22/16</td> 
   <td colspan="1">バグ修正：オポチュニティ連絡先の役割の更新が完全にキャプチャされませんでした。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.19</td> 
   <td colspan="1">6/28/16</td> 
   <td colspan="1"><p>バグ修正：オポチュニティが作成された時点で、マーケティングログのcustomeropportunityroleに不要な更新トランザクションが記録されていました。 </p><p>バグ修正：customeropportunityroleエンティティの削除時に、余分な削除トランザクションがログに記録されていました。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.18</td> 
   <td colspan="1">5/31/16</td> 
   <td colspan="1">バグ修正： カスタムオブジェクトの更新と削除を非同期にしました。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.17</td> 
   <td colspan="1">2016年4月8日</td> 
   <td colspan="1">バグ修正：リードの同期フィルタが「NO」に設定され、オポチュニティと連絡先に同期フィルタがない場合、リードが条件を満たしたときに、連絡先とオポチュニティに対して「ログを作成」が生成されませんでした。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.16</td> 
   <td colspan="1">3/29/16</td> 
   <td>バグ修正：同期フィルタがオフになった場合に割り当てイベントがログに記録されました。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.15</td> 
   <td colspan="1">3/3/16</td> 
   <td colspan="1">バグ修正：ログインユーザーがMarketo設定の権限を持っていないため、顧客はCRMでリードを作成できませんでした。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.14</td> 
   <td colspan="1">1/18/16</td> 
   <td colspan="1">バグ修正：セキュリティ上の問題に対処するために、通常のDynamicsユーザーのアクセス制限を作成しました。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.13</td> 
   <td colspan="1">12/30/15</td> 
   <td>バグ修正：Dynamicsの更新が、ステップと画像のためにMarketoに同期されませんでした。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.12</td> 
   <td colspan="1">11/12/15</td> 
   <td colspan="1">バグ修正：同期フィルターがfalseに設定されているときに、リードレコードがMarketoに同期されていました。</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Marketoリード管理ソリューションのダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)
