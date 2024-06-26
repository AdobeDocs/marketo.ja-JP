---
description: 最新のリリースノート - Marketo ドキュメント - 製品ドキュメント
title: 最新のリリースノート
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: ea9bf2a002415936cdfb5bfb723ce80723003da5
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 61%

---

# リリースノート：2024年7月 {#release-notes-july-24}

2024年6月リリースに含まれるすべての機能を以下に示します。機能の可用性については、お使いの Adobe Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

>[!AVAILABILITY]
>
>星（![星](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに従っており、**2024年7月26日**（PT）からリリースが開始され、その次の週から残りの機能が段階的にロールアウトされます。リリースの機能と日付は変更される場合があります。各機能のステータスについては、各機能の隣で確認してください。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">機能</th> 
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
     <tr> 
   <td><strong>Marketo REST API の変更</strong>：に小規模な変更を導入しています <a href="https://developers.marketo.com/rest-api/user-management/">User Management API</a>. 両方 <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">ユーザーの参照</a> および <a href="https://developers.marketo.com/rest-api/user-management/#delete_user">ユーザーの削除</a> エンドポイントがサポートされるようになりました <a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">Target アカウント管理</a> ユーザー。</td> 
   <td><i>近日開始</i></td>
   <td><i>近日開始</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## お知らせ {#announcements}

* **新しい開発者向けドキュメントサイト**:Marketo Engageのユーザーエクスペリエンスを向上させるための継続的な取り組みの一環として、2024 年 7 月にすべての開発者向けドキュメントをAdobe Experience LeagueおよびAdobe Developer web サイトに移行する予定です。 [詳細情報](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **クエリパラメーターのアクセストークンの廃止**:Marketo EngageREST API 呼び出しのクエリパラメーターでアクセストークンを使用した認証のサポートは、将来のリリースで削除される予定です（具体的な日付は未定）。 既存の統合は、Authorization ヘッダーの使用に移行する必要があります [ここで説明します](https://developers.marketo.com/rest-api/authentication/){target="_blank"}. 新しい開発では、Marketo Engageによる認証に Authorization ヘッダーのみを使用する必要があります。

* **LinkedIn の再認証が必要です**：LinkedIn では、Marketo Engage LinkedIn 統合で使用されるマーケティング API をアップグレードしています。この変更により、サービスが中断されないよう、2024年7月26日（PT）から 12月15日（PT）までの間に、**管理**／**LaunchPoint** メニューですべての LinkedIn LaunchPoint サービスを再認証する必要があります。これを実行する方法については、[こちらからリード生成フォーム](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"}と[こちらから Matched Audiences](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"} を参照してください。リード生成フォームサービスには「LinkedIn リード生成」というタイプ、Matched Audience サービスには「LinkedIn Matched Audiences」というタイプがあります。詳しくは、[移行に関する FAQ](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"} を参照してください。
