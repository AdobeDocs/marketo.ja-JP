---
description: AWSへの移行 – Marketo Engage Docs – 製品ドキュメント
title: AWSへの移行
feature: Getting Started
hide: true
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: 8229c19a046bb9b8f82053475e8f00b5c27370c2
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 3%

---

# AWSへの移行 {#aws-migration}

今後数か月で、すべてのMarketo Engage サブスクリプションがプライベートデータセンターからAWS パブリッククラウドに移行され、信頼性、スケーラビリティ、スピードが向上します。

移行の約30日前に、メールとアプリ内通知が届きます。 このガイドを使用して準備を進めます。

## 推奨されるアクション

移行期間中、すべてのMarketo Engage サービスは利用できなくなります。 ビジネスへの影響を軽減するには、次の手順に従うことをお勧めします。

* **リード/人物**&#x200B;を作成または更新するか、人物レコードを変更するプロセスを実行しないでください。

* **スケジュールされた施策が一時停止されるため、フォローオンプロセスをトリガーしません**。

* **Marketo Engageとの間でデータを送受信する統合機能**&#x200B;を一時的に無効にします。

* **データのインポートまたはエクスポート、または主要なリード/人物生成キャンペーンを実行しないでください。**

* **ログイン、API アクセス、電子メール送信、web トラッキング、および統合に関するIP許可リスト**&#x200B;のレビューと更新。

* **新しいIP アドレス**&#x200B;を追加し、現在のIP アドレスをそのまま維持します。 以下の[&#x200B; テーブルを介して追加するIP アドレスを参照してください](#ip-addresses)。

## 期待されるサービス効果

以下の影響は、お客様の側で対処する必要はありません。

* **CRM統合とLaunchPoint サービス**&#x200B;は無効になりますが、後で自動的に再開する必要があります。
* **ランディングページ、フォーム、データ収集**&#x200B;は利用できなくなり、代わりにメンテナンスメッセージが表示されます。

## データセンター/ポッドの特定 {#identify}

以下の表を確認する前に、[&#x200B; サブスクリプションが配置されているデータセンターとポッド/サーバーを](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify)特定する方法を説明します。

## スケジュール {#schedule}

新しい日付やデータセンター/ポッド情報が定期的に追加されるので、詳細については、こちらで確認してください。

<table>
 <tbody>
  <tr>
   <th style="width:50%">日付</th>
   <th style="width:20%">データセンター/ポッド</th>
   <th style="width:30%">時間</th>
  </tr>
  <tr>
   <td>2026年6月19日（PT）</td>
   <td>AB46</td>
   <td>午後5時（太平洋標準時）</td>
  </tr>
  <tr>
   <td>2026年7月8日（PT）</td>
   <td>AB69<br>
   AB64</td>
   <td>午後5時（太平洋標準時）<br>
   午後6時（太平洋標準時）</td>
  </tr>
  <tr>
   <td>2026年7月9日（PT）</td>
   <td>AB70<br>
   AB43</td>
   <td>午後5時（太平洋標準時）<br>
   午後6時（太平洋標準時）</td>
  </tr>
  &lt;/body>
  </table>

## 追加するIP アドレス {#ip-addresses}

データセンターに基づいて、IT部門と協力して、それぞれのIP アドレスを追加します。

<table>
 <tbody>
  <tr>
   <th style="width:25%">データセンター</th>
   <th style="width:75%">IP アドレス</th>
  </tr>
  <tr>
   <td>AB</td>
   <td>54.160.246.246<br>
   54.237.141.197<br>
   52.20.211.99</td>
  </tr>
  <tr>
   <td>NLD</td>
   <td>34.247.24.245<br>
18.200.201.81<br>
54.220.138.65</td>
  </tr>
  &lt;/body>
  </table>

## アップデートとサポート

最新の更新情報は、このページをブックマークしてください。 ご不明な点がある場合は、Admin Consoleのサポートポータルまたは[Experience League](https://experienceleague.adobe.com/ja/support)からAdobe サポートにお問い合わせください。
