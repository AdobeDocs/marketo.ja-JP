---
description: リリースノート - 2024年3月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2024年3月
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
TQID: 'https://experienceleague.adobe.com/uyu2IwlX7zpRMqlc5N5VMZgq5ndkPKp7lvGsnpSLgrc'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
    internal-label: Resources
subfeature_v2:
  - id: af97ce94-35fa-4fa9-b85a-46b752ac4028
    internal-label: Release information
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 66%
---
# リリースノート：2024年3月 {#release-notes-mar-24}

以下に、24 年 3 月リリースに含まれるすべての機能を示します。 利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

>[!AVAILABILITY]
>
>星印（![星印](assets/yellow-star.png)）で示す機能は有償オプションです。 詳しくは、Marketo Engage 担当営業にお問い合わせください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに該当し、リリースは **2024年3月8日**（PT）から開始し、その次の週から残りの機能が段階的にロールアウトされます。 リリースの機能と日付は変更される場合があります。 各機能のステータスは、その機能の横に表示されている情報を確認してください。

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">機能</th>
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
  <tr>
   <td><strong>高度な対話型フローロジック</strong>：対話型フローのフォローアップ用に、単一の選択で評価用のフィールドを追加します。</td>
   <td>リリース</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Marketo Engage フォームの対話型フロー設定</a></td>
  </tr>
   <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr>
   <td><strong>対話型フローロジックの並べ替え</strong>:Marketo EngageFormsでは、対話型フローの選択肢を、削除して元に戻す代わりに並べ替えることができるようになりました。</td>
   <td>リリース</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Marketo Engage フォームの対話型フロー設定</a></td>
   </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>API アクティビティ メタデータ </strong>:
   Webや電子メールのアクティビティにUser Agent、Platform、Deviceなどのメタデータが含まれるようになり、Marketo REST APIを使用して、これらのアクティビティに関する一貫したインサイトを提供できるようになりました。</td>
   <td>リリース</td>
   <td>該当なし</td>
  </tr>
 </tbody>
</table>
<br/>

## お知らせ {#announcements}

* **プログラムメンバーの取得API修正**: [&#x200B; プログラムメンバーの取得](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Program-Members/operation/getProgramMembersUsingGET){target="_blank"} エンドポイントの動作を修正するために、最近変更が行われました。 以前は、 `updatedAt` フィルタータイプを使用して日付範囲を指定すると、その範囲内で更新されたプログラムメンバーシップレコードが応答に含まれない可能性がありました。 また、指定した日付範囲外で更新されたプログラムメンバーシップレコードが、誤って応答に含まれてしまう可能性がありました。 両方の問題が解決されました。

* **Account Insight Browser Plug-in Deprecation**: Adobeは、2024年4月8日にTarget Account Management [Account Insight ブラウザープラグイン &#x200B;](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"}をChrome Web Storeから削除します。 既存のユーザー：Marketo Engage インスタンスをAdobe IDおよびAdmin Consoleに移行するまで、プラグインを引き続き使用できます。 この変更&#x200B;**は、Marketo Engage内の他のTAM機能/データ、またはSales Insightと連携するChromeおよびOutlook メールプラグインには影響しません**。 [詳細情報](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}。
