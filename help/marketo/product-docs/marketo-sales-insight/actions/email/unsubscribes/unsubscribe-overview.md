---
description: Sales Insight アクションでの購読解除の処理について説明します。 購読解除の仕組みとMarketoおよびSalesforceとの同期について説明します。
title: 配信停止の概要
exl-id: 7598efa9-9686-4dd0-840b-f8b6de4ab2be
feature: Sales Insight Actions
TQID: https://experienceleague.adobe.com/cY3Vm4hAQvzV4ABOqhjFELHzaGyf0Rt7UKg-5JF-PvQ
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
topic_v2:
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 357
ht-degree: 82%

---

# 登録解除の概要 {#unsubscribe-overview}

組織によるメールのプライバシーに関する法律への準拠はますます重要になっています。 これを支援するために、アドビは配信停止エクスペリエンスをいくつか強化しました。

* 登録解除リンクは、[!DNL Marketo Sales] および [!DNL Salesforce] から送信されるすべてのメールに配置されます（[!DNL Outlook] または Gmail から送信されるカスタムメールには適用されません）
* 管理者は、チーム全体の配信停止メッセージを編集できます
* 配信停止情報は PDV に保存されます
* 登録解除は手動で行うことができます。クリック済みリンク、[!DNL Salesforce] 同期、バウンスです。
* 新しい登録解除リンクランディングページ

## リンクの登録解除ランディングページ {#unsubscribe-link-landing-page}

ユーザが配信停止リンクをクリックすると、配信停止ランディングページが表示され、配信停止元とその理由を選択できます。

![](assets/unsubscribe-overview-1.png)

この情報は、後で表示するために人物の詳細表示に保存されます。

## 登録解除グループ {#unsubscribe-group}

配信停止済みの人物をすべて 1 か所で表示および管理します。

![](assets/unsubscribe-overview-2.png)

配信停止済みの人物を検索するには、検索バーを使用します。

![](assets/unsubscribe-overview-3.png)

管理者の場合は、購読解除グループに移動して、[!UICONTROL &#x200B; アカウント購読解除]でフィルタリングし、人物データベースで収集されたすべての購読解除を確認できます。

![](assets/unsubscribe-overview-4.png)

## 登録解除履歴カード {#unsubscribe-history-card}

[!UICONTROL 登録解除履歴]カードを使用すると、管理者やユーザは、取引先責任者の登録解除履歴に関するコンテキスト情報を取得できます。 「[!UICONTROL 人物]」タブに移動し、人物を選択して移動します。 人物の詳細ビューの「[!UICONTROL 約]」タブの下部にあります。

>[!NOTE]
>
>その人物がある時点で&#x200B;_再購読_&#x200B;した場合、[!UICONTROL 登録解除履歴]カードのみ表示されます。

![](assets/unsubscribe-overview-5.png)

<table>
 <colgroup>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <td><strong>[!UICONTROL 日付]</strong></td>
   <td><p>登録解除／再購読が行われた日付を表示します。</p></td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL 詳細]</strong></td>
   <td><p>再購読：[!DNL Sales Connect] 管理者が、取引先責任者レコードから登録解除を手動で削除した。 また、取引先責任者の配信停止理由に関する詳細も表示されます。</p><p>配信停止：取引先責任者が配信停止された。</p></td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL ソース]</strong></td>
   <td><p>[!DNL Salesforce] 同期：登録解除が [!DNL Salesforce] の同期によって取得された。</p><p>手動：ユーザが「配信停止」ボタンをクリックしてオプトアウトした。</p><p>リンクをクリック：メールの受信者が配信停止リンクをクリックした。</p><p>「管理者名」：管理者の名前は、アクションが取引先責任者の再購読の場合に表示されます。 ユーザーは誰が登録解除を削除したかを知ることができます。</p></td>
  </tr>
 </tbody>
</table>

>[!MORELIKETHIS]
>
>[配信停止リンクメッセージのカスタマイズ](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
