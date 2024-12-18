---
unique-page-id: 10099389
description: Microsoft Dynamics 向け Marketo プラグインリリース - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 向け Marketo プラグインリリース
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
feature: Microsoft Dynamics
source-git-commit: f1fd9564abe4702c3a124442ee26027d4d22f23d
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 86%

---

# Microsoft Dynamics 向け Marketo プラグインリリース {#marketo-plugin-releases-for-microsoft-dynamics}

Microsoft Dynamics に初めて同期するときは、Marketo 用のプラグインの最新バージョンをダウンロードします。Marketo は定期的にこれらのプラグインを更新するので、同じ場所に戻って新しいバージョンをダウンロードできます。

お使いの Dynamics リリースに対応した、[最新のプラグインをダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}してください。

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## Dynamics ソリューションのアップデート {#updating-your-dynamics-solution}

1. Dynamics CRM の既存のバージョンに対して、ソリューションの最新バージョンをインポートします（例：Dynamics CRM のバージョンが 1.4 で、最新バージョンが 1.5 の場合は、バージョン 1.4 _以降_&#x200B;をインポートします）。

1. 次のポップアップが表示されます。「**アップデート**」および「**カスタマイズを維持**」を選択し、「**インポート**」をクリックします。

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## 最新バージョン {#latest-versions}

>[!NOTE]
>
>これらのバージョンは、Dynamics のオンプレミスバージョンとオンラインバージョンの両方で機能します。

<table> 
 <tbody> 
  <tr> 
   <th style="width:15%">バージョン</th> 
   <th style="width:20%">リリース日</th> 
   <th style="width:65%">注意</th> 
  </tr>
  <tr> 
   <td>5.0.2.1</td> 
   <td>1/19/24</td> 
   <td>バグ修正：カスタムエンティティ同期に関連するバグを修正しました。</td> 
  </tr> 
  <tr> 
   <td>5.0.2.0</td> 
   <td>2023/3/24</td> 
   <td>バグ修正：MS Dynamics で連絡先を結合できないバグを修正しました。</td> 
  </tr> 
  <tr> 
   <td>5.0.1.8</td> 
   <td>2023/3/27</td> 
   <td>バグ修正：プラグインが MS Dynamics の UI 要素の他のカスタマイズを上書きするのを防ぎます。
   <p>
   バグ修正：5.0.1.1 で欠落したナビゲーションタイルを復元しました。</td> 
  </tr> 
  <tr> 
   <td>5.0.1.1</td> 
   <td>2021/04/02</td> 
   <td>複数選択オプションセットフィールドの同期のサポート（この機能は V9.X 以降でのみ利用可能）。</td> 
  </tr> 
  <tr> 
   <td>4.2.0.0</td> 
   <td>2020/10/16</td> 
   <td>MS Dynamics との Campaign 同期のサポートを追加しました。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.24</td> 
   <td>2018/08/22</td> 
   <td>Microsoft Dynamics バージョン 9.x 標準の、認定リードの取引先責任者プロセスに対するサポートが追加されました。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.23</td> 
   <td>2018/06/27</td> 
   <td>バグ修正：Dynamics 2013 用 Marketo ソリューションのインストール中に発生するビジネスプロセスエラー。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.22</td> 
   <td>2017/09/29</td> 
   <td>バグ修正：内部リビジョン。</td> 
  </tr> 
  <tr> 
   <td><p>4.0.0.21</p></td> 
   <td>2016/11/9</td> 
   <td>バグ修正：プラグインは、カスタムオブジェクトのステート変更をキャプチャするイベントをサブスクライブしませんでした。この修正は、Dynamics CRM オンプレミス 2011 に固有です。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.20</td> 
   <td>2016/07/22</td> 
   <td>バグ修正：商談取引先責任者のロールの更新が完全にキャプチャされていませんでした。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.19</td> 
   <td>2016/06/28</td> 
   <td>バグ修正：商談が作成された際に、marketo ログの customeropportunityrole で不要な更新トランザクションが記録されました。<p>バグ修正：customeropportunityrole エンティティの削除時に、追加の削除トランザクションがログに記録されました。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.18</td> 
   <td>2016/05/31</td> 
   <td>バグ修正：カスタムオブジェクトの更新と削除を非同期にしました。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.17</td> 
   <td>2016/04/08</td> 
   <td>バグ修正：リードの同期フィルターが「いいえ」に設定され、商談と取引先責任者に同期フィルターが設定されていない場合、リードが条件を満たしたときに取引先責任者と商談に対してログの作成が生成されませんでした。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.16</td> 
   <td>2016/03/29</td> 
   <td>バグ修正：同期フィルターがオフになったときに、割り当てイベントがログに記録されました。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.15</td> 
   <td>2016/03/03</td> 
   <td>バグ修正：ログインユーザに Marketo 設定の権限がないので、顧客が CRM でリードを作成できませんでした。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.14</td> 
   <td>2016/01/18</td> 
   <td>バグ修正：セキュリティ上の問題に対処するために、通常の Dynamics ユーザのアクセス制限を作成しました。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.13</td> 
   <td>2015/12/30</td> 
   <td>バグ修正：Dynamics のアップデートが、Marketo のステップと画像に同期されませんでした。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.12</td> 
   <td>2015/11/12</td> 
   <td>バグ修正：同期フィルターが false に設定されている場合、リードレコードが Marketo に同期されていました。</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Marketo リード管理ソリューションのダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}
