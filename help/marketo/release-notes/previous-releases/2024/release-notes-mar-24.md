---
description: リリースノート - 2024年3月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2024年3月
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 79%

---

# リリースノート：2024年3月 {#release-notes-mar-24}

以下に、24 年 3 月リリースに含まれるすべての機能を示します。機能の可用性についてはお使いの Marketo Engage のエディションをご確認ください。

>[!AVAILABILITY]
>
>星（![星](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに該当し、リリースは **2024年3月8日**（PT）から開始し、その次の週から残りの機能が段階的にロールアウトされます。リリースの機能と日付は変更される場合があります。各機能のステータスについては、各機能の隣で確認してください。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">機能</th> 
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
  <tr> 
   <td><strong>高度な対話型フローロジック</strong>：対話型フローのフォローアップ用に、単一の選択で評価用のフィールドを追加します。</td> 
   <td>リリース済み</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Marketo EngageFormsの対話型フロー設定</a></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong>対話型フローロジックの並べ替え</strong>:Marketo EngageFormsでは、対話型フローの選択肢を、削除して元に戻す代わりに並べ替えることができるようになりました。</td> 
   <td>リリース済み</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Marketo EngageFormsの対話型フロー設定</a></td>
   </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>API アクティビティメタデータ</strong>：ユーザーエージェント、プラットフォーム、デバイスなどのメタデータが Web アクティビティと電子メールアクティビティに含まれるようになり、Marketo REST API を介してこれらのアクティビティに対する一貫したインサイトを提供できます。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## お知らせ {#announcements}

* **プログラムメンバー API 修正の取得**：の動作を修正するために最近変更がおこなわれました [プログラムメンバーの取得](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Program-Members/operation/getProgramMembersUsingGET){target="_blank"} endpoint. 以前は、 `updatedAt` フィルタータイプを使用して日付範囲を指定すると、その範囲内で更新されたプログラムメンバーシップレコードが応答に含まれない可能性がありました。 また、指定した日付範囲外で更新されたプログラムメンバーシップレコードが応答に正しく含まれない可能性がありました。 両方の問題が解決されました。

* **アカウント Insight ブラウザープラグインの廃止**:Adobeが Target Account Management を削除しています [アカウント Insight ブラウザープラグイン](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} 2024 年 4 月 8 日（PT）の Chrome ウェブストアから。 既存のユーザー：Marketo EngageインスタンスをAdobe ID およびAdmin Consoleに移行するまで、プラグインを引き続き使用できます。 この変更 **影響なし** Marketo Engage内のその他の TAM 機能/データ、または Sales Insight で動作する Chrome および Outlook メールプラグイン。 [詳細情報](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}。
