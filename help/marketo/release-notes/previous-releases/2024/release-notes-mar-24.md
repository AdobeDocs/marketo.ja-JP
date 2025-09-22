---
description: リリースノート - 2024年3月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2024年3月
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 65%

---

# リリースノート：2024年3月 {#release-notes-mar-24}

以下に、24 年 3 月リリースに含まれるすべての機能を示します。利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

>[!AVAILABILITY]
>
>星印（![星印](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

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
   <td><strong>API アクティビティメタデータ </strong>:
   User Agent、Platform、Device などのメタデータが web アクティビティやメールアクティビティに含まれるようになりました。これにより、Marketo REST API を使用してこれらのアクティビティに関して一貫したインサイトを提供できます。</td>
   <td>リリース済み</td>
   <td>該当なし</td>
  </tr>
 </tbody>
</table>
<br/>

## お知らせ {#announcements}

* **プログラムメンバー取得 API の修正**: [ プログラムメンバーを取得 ](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Program-Members/operation/getProgramMembersUsingGET){target="_blank"} エンドポイントの動作を修正する変更が最近加えられました。 以前は、 `updatedAt` フィルタータイプを使用して日付範囲を指定すると、その範囲内で更新されたプログラムメンバーシップレコードが応答に含まれない可能性がありました。 また、指定した日付範囲外で更新されたプログラムメンバーシップレコードが応答に正しく含まれない可能性がありました。 両方の問題が解決されました。

* **アカウント Insight ブラウザープラグインの廃止**:Adobeは、2024 年 4 月 8 日にChrome web ストアから Target アカウント管理 [ アカウント Insight ブラウザープラグイン ](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} を削除します。 既存のユーザー：Marketo Engage インスタンスをAdobe ID およびAdmin Consoleに移行するまで、プラグインを引き続き使用できます。 この変更は、Marketo Engage内の他の TAM 機能/データ **またはセールスInsightで動作するChromeおよび Outlook 電子メールプラグインに** 影響しません）。 [詳細情報](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}。
