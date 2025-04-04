---
description: 最新のリリースノート - Marketo ドキュメント - 製品ドキュメント
title: 最新のリリースノート
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: cf4df30b575061bde18cf38e355604b970b7c51e
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 100%

---

# リリースノート：2025年3月 {#release-notes-mar-25}

以下に、25年3月リリースに含まれるすべての機能を示します。利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

>[!AVAILABILITY]
>
>星（![星](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに該当し、リリースは **2025年3月28日**（PT）から開始し、その次の週から残りの機能が段階的にロールアウトされます。リリースの機能と日付は変更される場合があります。各機能のステータスについては、各機能の隣で確認してください。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">機能</th> 
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
    <tr> 
   <td><strong>すべてのプログラムで使用可能なメールデザイナー</strong>：新しいメールデザイナーのメールは、エンゲージメントプログラム、デフォルトプログラム、イベントプログラムをまたいでアクセスできるようになりました（唯一の例外はインタラクティブウェビナープログラムです）。以前は、メールプログラムでのみ使用できました。この更新により、クローン作成も使用できるようになります。</td>
   <td>出荷済み</td>
   <td>該当なし</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>インタラクティブウェビナーの生成 AI 機能</strong>：オンデマンドウェビナーのチャプターと概要を生成できるようになりました。データの HTML ファイルを編集して書き出します。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>グローバルおよびワークスペースのマイトークン</strong>：ワークスペースとグローバルレベルの両方でマイトークンを設定して、Marketo Engage ワークスペースをまたいで、さらにはインスタンス全体でのブランドとマーケティングの販促物に対する生産性の向上と制御を可能にします。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>任意のトリガー属性のトークン</strong>：<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments" target="_blank">このドキュメント</a>のリストのみから使用可能なトリガートークンのリストを展開して、キャンペーンフローフィールドの任意のトリガーアクティビティ属性のデータの使用をサポートします。アクティビティ属性から注目のアクションにデータを印刷するか、カスタムアクティビティからリードの最新トランザクション ID をリードフィールドに設定します。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## お知らせ {#announcements}

* **ソーシャル機能の廃止**：2024年7月31日水曜日（PT）に、Marketo Engage では製品内の次のソーシャル機能の廃止を開始しました。

   * 投票
   * ソーシャルボタン
   * 紹介オファー
   * 動画の共有
   * 懸賞

この時点では、ユーザは Marketo Engage でこれらのソーシャル機能を作成、複製、埋め込むことができなくなりました。既存のソーシャルアセットは、2025年1月31日（PT）まで引き続き機能します。2025年2月1日（PT）をもって、ソーシャルアセットは機能しなくなりました。ランディングページに埋め込まれた任意のソーシャル機能を削除する必要があります。[詳細情報](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Rest API「access_token」パラメーターの廃止**：Marketo REST API 呼び出しの認証に使用される `access_token` クエリパラメーターは非推奨（廃止予定）となり、2025年6月30日（PT）以降は使用できなくなります。すべての新規および既存の統合は、「Authorization」ヘッダーを使用して REST API 呼び出しを認証する必要があります。[詳しくは、こちらを参照してください](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API の廃止**：Marketo SOAP API のサポートは、2025年10月31日（PT）に終了する予定です。SOAP API 機能を使用するサービスは、[REST API](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} に移行する必要があります。

