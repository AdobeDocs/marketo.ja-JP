---
description: 配信停止の概要 - Marketo ドキュメント - 製品ドキュメント
title: 配信停止の概要
exl-id: 7598efa9-9686-4dd0-840b-f8b6de4ab2be
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: ht
source-wordcount: '348'
ht-degree: 100%

---

# 配信停止の概要 {#unsubscribe-overview}

組織がメールのプライバシーに関する法律に準拠する重要性が高まっています。これを支援するために、アドビは配信停止エクスペリエンスをいくつか強化しました。

* 配信停止リンクは、Marketo Sales および Salesforce から送信されるすべてのメールに配置されます（Outlook または Gmail から送信されるカスタムメールには適用されません）
* 管理者は、チーム全体の配信停止メッセージを編集できます
* 配信停止情報は PDV に保存されます
* 配信停止は、リンクをクリック、Salesforce 同期、バウンスすることによって、手動で行うことができます。
* 新しい配信停止リンクランディングページ

## 配信停止リンクランディングページ {#unsubscribe-link-landing-page}

ユーザが配信停止リンクをクリックすると、配信停止ランディングページが表示され、配信停止元とその理由を選択できます。

![](assets/unsubscribe-overview-1.png)

この情報は、後で表示するために人物の詳細表示に保存されます。

## グループの配信停止 {#unsubscribe-group}

配信停止済みの人物をすべて 1 か所で表示および管理します。

![](assets/unsubscribe-overview-2.png)

配信停止済みの人物を検索するには、検索バーを使用します。

![](assets/unsubscribe-overview-3.png)

管理者の場合は、配信停止グループに移動して、「アカウント配信停止」でフィルタリングし、ユーザデータベースで収集された配信停止をすべて表示できます。

![](assets/unsubscribe-overview-4.png)

## 配信停止履歴カード {#unsubscribe-history-card}

配信停止履歴カードを使用すると、管理者やユーザは、取引先責任者の配信停止履歴に関するコンテキスト情報を取得できます。「人物」タブに移動し、人物を選択して移動します。人物の詳細表示の「情報」タブの下部に表示されます。

>[!NOTE]
>
>その人物がある時点で&#x200B;_再購読_&#x200B;した場合、配信停止履歴カードのみ表示されます。

![](assets/unsubscribe-overview-5.png)

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>日付</strong></td> 
   <td><p>配信停止／再購読が行われた日付を表示します。</p></td> 
  </tr> 
  <tr> 
   <td><strong>詳細</strong></td> 
   <td><p>再購読：Sales Connect 管理者が、取引先責任者レコードから配信停止を手動で削除した。また、取引先責任者の配信停止理由に関する詳細も表示されます。</p><p>配信停止：取引先責任者が配信停止された。</p></td> 
  </tr> 
  <tr> 
   <td><strong>ソース</strong></td> 
   <td><p>Salesforce 同期：配信停止が Salesforce の同期によって取得された。</p><p>手動：ユーザが「配信停止」ボタンをクリックしてオプトアウトした。</p><p>リンクをクリック：メールの受信者が配信停止リンクをクリックした。</p><p>「管理者名」：管理者の名前は、アクションが取引先責任者の再購読の場合に表示されます。これにより、配信停止を削除した人をユーザに知らせます。</p></td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[配信停止リンクメッセージのカスタマイズ](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
