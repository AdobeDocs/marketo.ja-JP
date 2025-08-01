---
unique-page-id: 10099389
description: Marketo プラグインリリース  [!DNL Microsoft Dynamics] - Marketo ドキュメント – 製品ドキュメント
title: Marketo プラグインのリリース  [!DNL Microsoft Dynamics]
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
feature: Microsoft Dynamics
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 61%

---

# [!DNL Microsoft Dynamics] 用Marketo プラグインのリリース {#marketo-plugin-releases-for-microsoft-dynamics}

[!DNL Microsoft Dynamics] に初めて同期する際には、Marketo用のプラグインの最新バージョンをダウンロードします。 Marketo は定期的にこれらのプラグインを更新するので、同じ場所に戻って新しいバージョンをダウンロードできます。

[ リリースに対応する ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 最新のプラグインをダウンロード [!DNL Dynamics] します。

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## [!DNL Dynamics] ソリューションの更新 {#updating-your-dynamics-solution}

1. 既存のバージョンの [!DNL Dynamics] CRM に対して、ソリューションの最新バージョンをインポートします（例：[!DNL Dynamics] CRM のバージョンが 1.4 で、最新バージョンが 1.5 の場合は、_over_ バージョン 1.4 をインポートします）。

1. 次のポップアップが表示されます。「**アップデート**」および「**カスタマイズを維持**」を選択し、「**インポート**」をクリックします。

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## 最新バージョン {#latest-versions}

>[!NOTE]
>
>これらのバージョンは、[!DNL Dynamics] のオンプレミスバージョンとオンラインバージョンの両方で機能します。

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
   <td colspan="1">4.2.0.0</td>
   <td colspan="1">2020/10/16</td>
   <td colspan="1">MS [!DNL Dynamics] でのキャンペーン同期のサポートを追加しました。</td>
  </tr>
  <tr>
   <td colspan="1">4.0.0.24</td>
   <td colspan="1">2018/08/22</td>
   <td colspan="1">[!DNL Microsoft Dynamics] バージョン 9.x の標準のリード認定サポートを追加して、連絡先プロセスをサポートするようになりました。</td>
  </tr>
  <tr>
   <td colspan="1">4.0.0.23</td>
   <td colspan="1">2018/06/27</td>
   <td colspan="1">バグ修正：[!DNL Dynamics] 2013 のMarketo ソリューションのインストールを試みている際にビジネスプロセスエラーが発生しました。</td>
  </tr>
  <tr>
   <td>4.0.0.24</td>
   <td>2018/08/22</td>
   <td>Microsoft Dynamics バージョン 9.x 標準の、認定リードの取引先責任者プロセスに対するサポートが追加されました。</td>
  </tr>
  <tr>
   <td colspan="1"><p>4.0.0.21</p></td>
   <td colspan="1">2016/11/9</td>
   <td colspan="1">バグ修正：プラグインは、カスタムオブジェクトのステート変更をキャプチャするイベントをサブスクライブしませんでした。この修正は、[!DNL Dynamics] CRM オンプレミス 2011 に固有です。 </td>
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
   <td colspan="1">4.0.0.14</td>
   <td colspan="1">2016/01/18</td>
   <td colspan="1">バグ修正：セキュリティ上の問題に対処するために、通常の [!DNL Dynamics] ユーザーに対するアクセス制限を作成しました。</td>
  </tr>
  <tr>
   <td colspan="1">4.0.0.13</td>
   <td colspan="1">2015/12/30</td>
   <td>バグ修正：[!DNL Dynamics] のアップデートが、手順や画像についてMarketoと同期されていませんでした。</td>
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
