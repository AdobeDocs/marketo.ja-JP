---
description: AWSへの移行 – Marketo Engage Docs – 製品ドキュメント
title: AWSへの移行
feature: Getting Started
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: 3b6dbef83c5ac1f764d573f96d88dd0dfb388acc
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 5%

---

# AWSへの移行 {#aws-migration}

今後数か月で、すべてのMarketo Engage サブスクリプションがプライベートデータセンターからAWS パブリッククラウドに移行され、信頼性、スケーラビリティ、スピードが向上します。

移行の約30日前に、メールとアプリ内通知が届きます。 このガイドを使用して準備を進めます。

## 推奨されるアクション {#actions}

移行期間中、すべてのMarketo Engage サービスは利用できなくなります。 ビジネスへの影響を軽減するには、次の手順に従うことをお勧めします。

* **リード/人物**&#x200B;を作成または更新するか、人物レコードを変更するプロセスを実行しないでください。

* **スケジュールされた施策が一時停止されるため、フォローオンプロセスをトリガーしません**。

* **Marketo Engageとの間でデータを送受信する統合機能**&#x200B;を一時的に無効にします。

* **データのインポートまたはエクスポート、または主要なリード/人物生成キャンペーンを実行しないでください。**

* **ログイン、API アクセス、電子メール送信、web トラッキング、および統合に関するIP許可リスト**&#x200B;のレビューと更新。

* **新しいIP アドレス**&#x200B;を追加し、現在のIP アドレスをそのまま維持します。 以下の[&#x200B; テーブルを介して追加するIP アドレスを参照してください](#ip-addresses)。

## 期待されるサービス効果 {#impacts}

以下の影響は、お客様の側で対処する必要はありません。

* **CRM統合とLaunchPoint サービス**&#x200B;は無効になりますが、後で自動的に再開する必要があります。
* **ランディングページ、フォーム、データ収集**&#x200B;は利用できなくなり、代わりにメンテナンスメッセージが表示されます。

>[!NOTE]
>
>[外部フォーム &#x200B;](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"}を使用しており、移行期間中にMarketo Engageが利用できない間に収集したフォーム送信データを失わないようにしたい場合は、事前に[Adobe サポート &#x200B;](https://experienceleague.adobe.com/ja/support){target="_blank"} **少なくとも2営業日**&#x200B;までにお問い合わせください。フォーム IDとサブスクリプションのMunchkin IDを入力してください。

## データセンター/ポッドの特定 {#identify}

以下の表を確認する前に、[&#x200B; サブスクリプションが配置されているデータセンターとポッド/サーバーを](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify)特定する方法を説明します。

## スケジュール {#schedule}

新しい日付とデータセンター/ポッド情報は定期的に追加または変更されるので、このスケジュールを監視して更新します。

+++7月スケジュール
<table>
 <tbody>
  <tr>
   <th style="width:25%">日付</th>
   <th style="width:25%">データセンター/ポッド</th>
   <th style="width:25%">時間</th>
   <th style="width:25%">ステータス</th>
  </tr>
  <tr>
   <td>2026年7月8日（PT）</td>
   <td>AB69<br>
   AB64</td>
   <td>午後5時（太平洋夏時間）<br>
   午後6時（太平洋夏時間）</td>
   <td>完了<br>
   完了日</td>
  </tr>
  <tr>
   <td>2026年7月9日（PT）</td>
   <td>AB70</td>
   <td>午後5時（太平洋夏時間）</td>
   <td>完了</td>
  </tr>
  <tr>
   <td>2026年7月11日（PT）</td>
   <td>AB46</td>
   <td>午前10時（太平洋夏時間）</td>
   <td>完了</td>
  </tr>
  <tr>
   <td>2026年7月13日（PT）</td>
   <td>NLD101</td>
   <td>午前10時（太平洋夏時間）</td>
   <td>完了</td>
  </tr>
  <tr>
   <td>2026年7月15日（PT）</td>
   <td>NLD102<br>
   NLD104</td>
   <td>午前10時（太平洋夏時間）<br>
   午前11時（太平洋夏時間）</td>
   <td>完了<br>
   完了日</td>
  </tr>
  <tr>
   <td>2026年7月17日（PT）</td>
   <td>NLD103<br>
   NLD105</td>
   <td>午前10時（太平洋夏時間）<br>
   午前11時（太平洋夏時間）</td>
   <td>完了<br>
   完了日</td>
  </tr>
  <tr>
   <td>2026年7月21日（PT）</td>
   <td>AB54</td>
   <td>午後5時（太平洋夏時間）</td>
   <td>完了</td>
  </tr>
  <tr>
   <td>2026年7月23日（PT）</td>
   <td>AB48</td>
   <td>午後5時（太平洋夏時間）</td>
   <td>完了</td>
  </tr>
  <tr>
   <td>2026年7月31日（PT）</td>
   <td>AB43</td>
   <td>午後3時（太平洋夏時間）</td>
   <td>完了</td>
  </tr>
  </body>
</table>

+++

<table>
 <tbody>
  <tr>
   <th style="width:25%">日付</th>
   <th style="width:25%">データセンター/ポッド</th>
   <th style="width:25%">時間</th>
   <th style="width:25%">ステータス</th>
  </tr>
  <tr>
   <td>2026年8月12日（PT）</td>
   <td>AB61<br>
   AB17</td>
   <td>午後3時（太平洋夏時間）<br>
   午後4時（太平洋夏時間）</td>
   <td>完了<br>
   完了日</td>
  </tr>
  <tr>
  <td>2026年8月13日（PT）</td>
   <td>AB68</td>
   <td>午後4時（太平洋夏時間）</td>
   <td>完了</td>
  </tr>
  <tr>
   <td>2026年8月20日（PT）</td>
   <td>AB42<br>
   <i>AB44</i></td>
   <td>午後5時（太平洋夏時間）<br>
   <i>PDT</i>午後6時</td>
   <td>予定通り<br>
   <i>延期（未定） </i></td>
  </tr>
  <tr>
   <td>2026年8月26日（PT）</td>
   <td>AB40<br>
   AB50</td>
   <td>午後5時（太平洋夏時間）<br>
   午後6時（太平洋夏時間）</td>
   <td>予定通り<br>
   予定通り</td>
  </tr>
  <tr>
   <td>2026年8月28日（PT）</td>
   <td>AB53<br>
   AB56</td>
   <td>午後3時（太平洋夏時間）<br>
   午後4時（太平洋夏時間）</td>
   <td>予定通り<br>
   予定通り</td>
  </tr>
  <tr>
   <td>2026年9月8日（PT）</td>
   <td>AB01<br>
   AB02</td>
   <td>午後5時（太平洋夏時間）<br>
   午後6時（太平洋夏時間）</td>
   <td>予定通り<br>
   予定通り</td>
  </tr>
  <tr>
   <td>2026年9月10日（PT）</td>
   <td>AB03<br>
   <i>AB04</i></td>
   <td>午後5時（太平洋夏時間）<br>
   <i>PDT</i>午後6時</td>
   <td>予定通り<br>
   <i>延期（未定） </i></td>
  </tr>
  <tr>
   <td>2026年9月15日（PT）</td>
   <td>AB05<br>
   AB06</td>
   <td>午後5時（太平洋夏時間）<br>
   午後6時（太平洋夏時間）</td>
   <td>予定通り<br>
   予定通り</td>
  </tr>
  <tr>
   <td>2026年9月17日（PT）</td>
   <td>AB07<br>
   AB08</td>
   <td>午後5時（太平洋夏時間）<br>
   午後6時（太平洋夏時間）</td>
   <td>予定通り<br>
   予定通り</td>
  </tr>
  </body>
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
</body>
</table>

## アップデートとサポート {#support}

最新の更新情報は、このページをブックマークしてください。 ご不明な点がある場合は、Admin Consoleのサポートポータルまたは[Experience League](https://experienceleague.adobe.com/ja/support){target="_blank"}からAdobe サポートにお問い合わせください。

## よくある質問 {#faq}

**データはどこに保存されていますか？**
Marketoのユーザーデータはすべて、Amazon Web Services（AWS）に保存されています。 Marketoは、インフラストラクチャを自社の物理データセンターからAWSのエンタープライズグレードのクラウドプラットフォームに移行しました。

**個人データは具体的にどこに保存されますか？**
個人データは、AWSのフルマネージドリレーショナルデータベースサービスであるAmazon Auroraに保存されます。 Auroraは、ハードウェアの障害、ストレージの低下、およびローカライズされたインフラストラクチャのイベントから個人データを保護するために、AWSリージョン内の3つの別々のアベイラビリティゾーンに6つの方法でデータを複製します。

**ストレージ環境は誰のものですか？**
ストレージインフラストラクチャは、Amazon Web Services（AWS）が所有および運用します。 Adobe（Marketo）は、AWSのお客様として、共通の責任モデルの下で運用されます。AWSは、基盤となるインフラストラクチャのセキュリティと可用性を担当し、Adobeは、その中で実行されるデータとアプリケーションのセキュリティを担当します。

**実稼動環境、バックアップ/DRの場所、およびストレージ テクノロジーの詳細を教えてください。**
Marketoでは、主要なデータベーステクノロジーとして、AWSによって完全に管理されるクラウドネイティブなリレーショナルデータベースエンジンであるAmazon Auroraを使用しています。 Auroraは計算とストレージを切り離し、実稼動領域内の3つのアベイラビリティゾーンにわたって6つの方法でデータを自動的にレプリケートし、書き込み操作を確認するには4つのコピーのクォーラムが必要です。

Auroraは、Amazon S3への継続的な自動バックアップもリアルタイムで実行し、設定された保持ウィンドウ内でPoint-in-Time Recovery （PITR）を任意の秒間に有効にします。

現時点では、MarketoのAurora デプロイメントは、クロスリージョンのレプリケーションなしで、1つのAWS リージョン内で動作します。 本番データは指定された地域インフラストラクチャ内に残り、災害復旧は、セカンダリ地域への地理的フェイルオーバーではなく、Auroraのマルチ AZ ストレージの冗長性と継続的なバックアップを通じて提供されます。 これは、MarketoのAWSインフラストラクチャが成熟するにつれて、さらに評価される可能性があります。
