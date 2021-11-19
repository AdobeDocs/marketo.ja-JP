---
description: 購読解除の概要 — Marketoドキュメント — 製品ドキュメント
title: 配信停止の概要
hide: true
hidefromtoc: true
source-git-commit: a4a92f2d557581d6685342f45c11c260cf9cad3b
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 5%

---

# 配信停止の概要 {#unsubscribe-overview}

組織が E メールのプライバシーに関する法律に準拠することがますます重要になってきています。 これを支援するために、配信停止エクスペリエンスをいくつか強化しました。

* 配信停止リンクは、Marketo Sales および Salesforce から送信されるすべてのメールに配置されます（Outlook または Gmail から送信されるカスタムメールには適用されません）
* 管理者は、チーム全体の配信停止メッセージを編集できます
* 配信停止情報は PDV に保存されます
* 配信停止は手動でおこなうことができます。リンク、Salesforce 同期、バウンスをクリック済み
* 新しい配信停止リンクランディングページ

## リンクの配信停止ランディングページ {#unsubscribe-link-landing-page}

ユーザーが購読解除リンクをクリックすると、購読解除ランディングページが表示され、購読解除元とその理由を選択できます。

![](assets/unsubscribe-overview-1.png)

この情報は、後で表示するために担当者詳細ビューに保存されます。

## グループの配信停止 {#unsubscribe-group}

配信停止済みの担当者をすべて 1 か所で表示および管理します。

![](assets/unsubscribe-overview-2.png)

購読解除済みの担当者を検索するには、検索バーを使用します。

![](assets/unsubscribe-overview-3.png)

管理者の場合は、配信停止グループに移動して、「アカウント配信停止」でフィルタリングし、ユーザーデータベースで収集された配信停止をすべて表示できます。

![](assets/unsubscribe-overview-4.png)

## 配信停止履歴カード {#unsubscribe-history-card}

配信停止履歴カードを使用すると、管理者やユーザーは、連絡先の配信停止履歴に関するコンテキスト情報を取得できます。 「人」タブに移動し、人を選択して移動します。 担当者の詳細ビューの [ バージョン情報 ] タブの下部に表示されます。

>[!NOTE]
>
>配信停止履歴カードは、配信停止履歴カードが _再購読_ ある時点で

![](assets/unsubscribe-overview-5.png)

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>日</strong></td> 
   <td><p>購読解除/再購読がおこなわれた日付を表示します。</p></td> 
  </tr> 
  <tr> 
   <td><strong>詳細</strong></td> 
   <td><p>再購読：セールスコネクト管理者が、連絡先レコードから配信停止を手動で削除しました。 また、連絡先の購読解除理由に関する詳細も表示されます。</p><p>配信停止：連絡先が購読解除されました。</p></td> 
  </tr> 
  <tr> 
   <td><strong>ソース</strong></td> 
   <td><p>Salesforce 同期：配信停止が Salesforce の同期によってキャプチャされました。</p><p>手動：ユーザーが購読解除ボタンをクリックしてオプトアウトした。</p><p>クリックされたリンク：E メールの受信者が購読解除リンクをクリックしました。</p><p>"管理名":管理者の名前は、アクションが連絡先の再登録をおこなう日時を示します。 これにより、誰が配信停止を削除したかをユーザーに知らせます。</p></td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[配信停止リンクメッセージのカスタマイズ](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
