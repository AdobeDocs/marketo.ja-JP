---
description: 最新のリリースノート - Marketo ドキュメント - 製品ドキュメント
title: 最新のリリースノート
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: a65ff2cb24b264cd2d3a1c9c7e0109bcf69ac996
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 86%

---

# リリースノート：2024年10月 {#release-notes-oct-24}

以下に、2024年10月リリースに含まれるすべての機能を示します。利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

>[!AVAILABILITY]
>
>星（![星](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに該当し、リリースは **2024年10月4日**（PT）から開始し、その次の週から残りの機能が段階的にロールアウトされます。リリースの機能と日付は変更される場合があります。各機能のステータスについては、各機能の隣で確認してください。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">機能</th> 
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
    <tr> 
   <td><strong>インタラクティブなウェビナー向けのエンゲージメントダッシュボードで登録データを強化</strong>：参加者数が最も多かった企業を確認し、エンゲージメントダッシュボードで利用できるレポートで企業、役職、業界をリードレベルで更新できるようになりました。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
    <tr> 
   <td><strong>インタラクティブウェビナーのトークン化</strong>：ウェビナーの詳細を手動で追加しなくても、トークンを使用してメールやランディングページでインタラクティブウェビナーを促進できるようになりました。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr> 
   <td><strong>スマートリストの「影響に設定」カウント</strong>：スマートキャンペーンの選定ルールを編集した際に影響を受けるユーザの数を確認します。</td> 
   <td>出荷済み</td>
   <td>該当なし</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr> 
   <td><strong>ナビゲーションパネルの「マイアカウント」ボタン</strong>：Adobe Identity Management システムに移行したユーザは、左側のナビゲーションパネルの新しい「マイアカウント」ボタンを使用して、タイムゾーンの設定とサブスクリプションの詳細にアクセスできます。</td> 
   <td>出荷済み</td>
   <td>該当なし</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   <tr> 
   <td><strong>メールパフォーマンスレポートの機能強化</strong>：メールレポートの指標とアクティビティトラッキングに関する複数の改善が行われ、追加のインサイトが提供され、精度が向上しました。
   <ul>
   <li>削除および結合された人物をメールパフォーマンス指標からフィルタリングします。</li>
   <li>応答アクティビティを 3 日間待機した後、メールは<i>中止</i>として分類されるようになりました。</li>
   <li>メール開封数は、スマートキャンペーンごとに個別に開かれたユニーク数としてカウントされます</li>
   <li>トラッキングピクセルの場所の絞り込みにより、メールアクティビティのトラッキングが改善されました。</li>
   </td> 
   <td>出荷済み</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md" target="_blank">メールパフォーマンスレポート</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   <tr> 
   <td><strong>Salesforce同期バックログの指標 </strong>：最適な同期エクスペリエンスを得るために CRM の更新を計画およびスケジュールするために、同期のスループットとバックログの傾向を監視します。
   </td> 
   <td>出荷済み</td>
   <td><a href="/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-backlog-metrics.md" target="_blank">Salesforce 同期バックログ指標</a></td>
  </tr>
 </tbody> 
</table>
<br/>

## お知らせ {#announcements}

* **Rest API access_token パラメーターの廃止**:Marketo REST API 呼び出しの認証に使用される「access_token」クエリパラメーターは非推奨となり、2025 年 6 月 30 日（PT）以降は使用できなくなります。 すべての新規および既存の統合は、「Authorization」ヘッダーを使用して REST API 呼び出しを認証する必要があります [ 詳しくは、こちらを参照 ](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication#using-an-access-token)。


* **QR コードの廃止**：2024年10月4日（PT）に、プッシュ通知およびアプリ内メッセージアセットで使用する QR コード機能が廃止される予定です。これには、新しいテストデバイス用の QR コードの使用や、QR コードを使用した新しいアセットの作成が含まれます。使用頻度の低い機能を廃止することで、そのリソースを Marketo Engage の全体的なメンテナンスに再割り当てできます。

* **Munchkin の変更**

   * **新しいバージョン**：2024年9月17日（PT）に、[Munchkin](/help/marketo/product-docs/administration/setup-administration/munchkin.md){target="_blank"} v.164 では、**管理**／**宝箱**&#x200B;で「Munchkin ベータ版」設定が有効化された Marketo Engage インスタンスへのロールアウトを開始します。他のすべてのインスタンスへのロールアウトは、10月29日（PT）に開始される予定です。このバージョンでは、Munchkin の Cookie の作成が更新されます。機能に変更はありません。

   * **URL から文字を削除**：Munchkin JS によって作成された「Web ページを訪問」および「リンクをクリック」アクティビティでは、すべての URL フィールドから URL エンコードされていない制御文字が削除されるようになりました。この変更は、サポートされていないシステムでこれらのタイプの文字が生成され、Marketo Engage 内で有効に使用されないことに関連するエラーを防ぐために設計されています。
