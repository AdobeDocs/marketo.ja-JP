---
description: 最新のリリースノート - Marketo ドキュメント - 製品ドキュメント
title: 最新のリリースノート
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: cfbf9206bcb0e54abdbd962e52844bba11b07197
workflow-type: ht
source-wordcount: '295'
ht-degree: 100%

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

* **プログラムメンバー API 修正の取得**：の動作を修正するために最近変更がおこなわれました [プログラムメンバーの取得](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Program_Members/getProgramMembersUsingGET){target="_blank"} endpoint. 以前は、 `updatedAt` フィルタータイプを使用して日付範囲を指定すると、その範囲内で更新されたプログラムメンバーシップレコードが応答に含まれない可能性がありました。 また、指定した日付範囲外で更新されたプログラムメンバーシップレコードが応答に正しく含まれない可能性がありました。 両方の問題が解決されました。

* **アカウントインサイトブラウザープラグインの廃止**:Adobeが Target アカウント管理を削除しています [アカウントインサイトブラウザープラグイン](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} from the Chrome Web Store on March 18, 2024. Existing users: you can continue to use the plug-in until you migrate your Marketo Engage instance to Adobe Identity and Admin Console. This change **will not impact** any other TAM features/data within Marketo Engage or the Chrome and Outlook email plug-ins that work with Sales Insight. [Learn more](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.
