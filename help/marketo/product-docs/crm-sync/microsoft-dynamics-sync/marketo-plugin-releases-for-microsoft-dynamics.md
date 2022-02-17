---
unique-page-id: 10099389
description: Microsoft Dynamics のMarketo Plugin リリース — Marketoドキュメント — 製品ドキュメント
title: Microsoft Dynamics 向け Marketo プラグインリリース
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
source-git-commit: 1379fcbdc0a8673b1d6cb17a9d573d3625d5a1b8
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 12%

---

# Microsoft Dynamics 向け Marketo プラグインリリース {#marketo-plugin-releases-for-microsoft-dynamics}

最初にMicrosoft Dynamics と同期するときは、Marketo用のプラグインの最新バージョンをダウンロードします。 Marketoは定期的にこれらのプラグインを更新するので、同じ場所に戻って新しいバージョンをダウンロードできます。

[最新のプラグインをダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) Dynamics リリースに対応しています。

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## Dynamics ソリューションの更新 {#updating-your-dynamics-solution}

1. Dynamics CRM の既存のバージョンに対して、ソリューションの最新バージョンをインポートします ( 例：Dynamics CRM のバージョンが 1.4 で、最新バージョンが 1.5 の場合は、 _over_ バージョン 1.4)。

1. 次のポップアップが表示されます。 選択 **更新** および **カスタマイズの管理**&#x200B;を選択し、「 **インポート**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## 最新バージョン {#latest-versions}

>[!NOTE]
>
>これらのバージョンは、Dynamics のオンプレミスバージョンとオンラインバージョンの両方で機能します。

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">バージョン</th> 
   <th colspan="1">リリース日</th> 
   <th>注意</th> 
  </tr> 
  <tr> 
   <td colspan="1">5.0.1.1</td> 
   <td colspan="1">02/04/21</td> 
   <td colspan="1">複数選択オプションセットフィールド同期のサポート（この機能は V9.X 以降でのみ使用可能）。.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.2.0.0</td> 
   <td colspan="1">10/16/20</td> 
   <td colspan="1">MS Dynamics との Campaign 同期のサポートを追加しました。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.24</td> 
   <td colspan="1">8/22/18</td> 
   <td colspan="1">Microsoft Dynamics バージョン 9.x の連絡プロセスに対する、標準で認定されたリードのサポートが追加されました。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.23</td> 
   <td colspan="1">6/27/18</td> 
   <td colspan="1">バグ修正：Dynamics 2013 用Marketoソリューションのインストール中にビジネスプロセスエラーが発生しました。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.22</td> 
   <td colspan="1">9/29/17</td> 
   <td colspan="1">バグ修正：内部リビジョン。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><p>4.0.0.21</p></td> 
   <td colspan="1">11/9/16</td> 
   <td colspan="1">バグ修正：プラグインは、カスタムオブジェクトの状態変更をキャプチャするイベントをサブスクライブしませんでした。 この修正は、Dynamics CRM On Premise 2011 に固有です。 </td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.20</td> 
   <td colspan="1">7/22/16</td> 
   <td colspan="1">バグ修正：オポチュニティ連絡先の役割の更新が完全にキャプチャされていませんでした。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.19</td> 
   <td colspan="1">6/28/16</td> 
   <td colspan="1"><p>バグ修正：オポチュニティが作成された際に、marketo ログの customeropportunityrole で不要な更新トランザクションが記録されました。 </p><p>バグ修正：customeropportunityrole エンティティの削除時に、追加の削除トランザクションがログに記録されました。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.18</td> 
   <td colspan="1">5/31/16</td> 
   <td colspan="1">バグ修正：カスタムオブジェクトの更新と削除を非同期にしました。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.17</td> 
   <td colspan="1">4/8/16</td> 
   <td colspan="1">バグ修正：リードの同期フィルタが [ いいえ ] に設定され、商談と連絡先に同期フィルタが設定されていない場合、リードが選定された際に連絡先と商談に対してログの作成が生成されませんでした。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.16</td> 
   <td colspan="1">3/29/16</td> 
   <td>バグ修正：同期フィルターがオフになったときに、割り当てイベントがログに記録されました。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.15</td> 
   <td colspan="1">3/3/16</td> 
   <td colspan="1">バグ修正：ログインユーザーにはMarketo Config の権限がないので、顧客は CRM でリードを作成できませんでした。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.14</td> 
   <td colspan="1">1/18/16</td> 
   <td colspan="1">バグ修正：セキュリティ上の問題に対処するために、通常の Dynamics ユーザーのアクセス制限を作成しました。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.13</td> 
   <td colspan="1">12/30/15</td> 
   <td>バグ修正：Dynamics の更新が、ステップと画像のMarketoに同期されませんでした。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.12</td> 
   <td colspan="1">11/12/15</td> 
   <td colspan="1">バグ修正：同期フィルターが false に設定されている場合、リードレコードがMarketoに同期されていました。</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Marketo リード管理ソリューションのダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)
