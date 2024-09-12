---
description: リリースノート - 2024 年 7 月 – Marketo ドキュメント – 製品ドキュメント
title: リリースノート - 2024年7月
feature: Release Information
source-git-commit: 3a722d0f4ec3e48b031c641d3b73e1e5539ebf80
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 97%

---

# リリースノート：2024年7月 {#release-notes-july-24}

2024年7月リリースに含まれるすべての機能を以下に示します。利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

>[!AVAILABILITY]
>
>星（![星](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

次の機能は標準リリースサイクルに従っており、**2024年7月26日（PT）**&#x200B;からリリースが開始され、その次の週から残りの機能が段階的にロールアウトされます。リリースの機能と日付は変更される場合があります。各機能のステータスについては、各機能の隣で確認してください。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">機能</th> 
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
     <tr> 
   <td><strong>インタラクティブウェビナーのエンゲージメントダッシュボード</strong>：ウェビナーのパフォーマンスの集計ビューとウェビナー中の各出席者のエンゲージメントの包括的なビューを取得し、Marketo Engage オーケストレーションツールを使用してターゲットとするリードを決定できます。</td> 
    <td>出荷済み</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/engagement-dashboard.md" target="_blank">エンゲージメントダッシュボード</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>インタラクティブウェビナーのルーム管理</strong>：作成された個々のルームにアクセスし（必要に応じて変更）、コンテンツと録画にアクセスします（必要に応じてクリアしてストレージを最適化します）。</td> 
    <td>出荷済み</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/room-management.md" target="_blank">ルーム管理</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>インタラクティブウェビナーのウェビナーカスタマイズ</strong>：ウェビナー戦略をブランド戦略とより簡単に一致させるために、共通のルームインターフェイス、中間画面（出席者のエントリ画面の背景など）、カスタムビデオ背景を使用することで、組織が承認した統一されたブランドエクスペリエンスを提供します。</td> 
    <td>出荷済み</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/customization.md" target="_blank">インタラクティブウェビナーのカスタマイズ</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Marketo REST API の変更</strong>：<a href="https://developers.marketo.com/rest-api/user-management/">User Management API</a> に小規模な変更を行っています。<a href="https://developers.marketo.com/rest-api/user-management/#browse_users">ユーザを参照</a>エンドポイントと<a href="https://developers.marketo.com/rest-api/user-management/#delete_user">ユーザを削除</a>エンドポイントの両方が、<a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">ターゲットアカウント管理</a>ユーザをサポートするようになりました。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## お知らせ {#announcements}

* **新しい開発者向けドキュメントサイト**：Marketo Engage のユーザエクスペリエンスを向上させるための継続的な取り組みの一環として、2024年7月にすべての開発者向けドキュメントを Adobe Experience League と Adobe Developer web サイトに移行する予定です。[詳細情報](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **ソーシャル機能の廃止**：2024年7月31日水曜日（PT）に、Marketo Engage では製品内の次のソーシャル機能の廃止を開始します。

   * 投票
   * ソーシャルボタン
   * 紹介オファー
   * 動画の共有
   * 懸賞

ユーザは、Marketo Engage でこれらのソーシャル機能を作成、複製、埋め込むことができなくなります。既存のソーシャルアセットは、2025年1月31日（PT）まで引き続き機能します。[詳細情報](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **クエリパラメーターのアクセストークンの廃止**：Marketo Engage REST API 呼び出しのクエリパラメーターでのアクセストークンを使用した認証のサポートは、将来のリリースで削除される予定です（具体的な日付は未定）。既存の統合は、[こちらで説明する](https://developers.marketo.com/rest-api/authentication/){target="_blank"} Authorization ヘッダーの使用に移行する必要があります。新規開発では、Marketo Engage での認証に Authorization ヘッダーのみを使用する必要があります。

* **LinkedIn の再認証が必要です**：LinkedIn では、Marketo Engage LinkedIn 統合で使用されるマーケティング API をアップグレードしています。この変更により、サービスが中断されないよう、2024年7月26日（PT）から 12月15日（PT）までの間に、**管理**／**LaunchPoint** メニューですべての LinkedIn LaunchPoint サービスを再認証する必要があります。これを実行する方法については、[こちらからリード生成フォーム](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"}と[こちらから Matched Audiences](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"} を参照してください。リード生成フォームサービスには「LinkedIn リード生成」というタイプ、Matched Audience サービスには「LinkedIn Matched Audiences」というタイプがあります。詳しくは、[ 移行に関する FAQ](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"} を参照してください。
