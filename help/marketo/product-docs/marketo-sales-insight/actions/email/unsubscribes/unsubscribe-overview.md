---
description: Sales Insight アクションでの購読解除の処理について説明します。 購読解除の仕組みとMarketoおよびSalesforceとの同期について説明します。
title: 配信停止の概要
exl-id: 7598efa9-9686-4dd0-840b-f8b6de4ab2be
feature: Sales Insight Actions
TQID: 'https://experienceleague.adobe.com/cY3Vm4hAQvzV4ABOqhjFELHzaGyf0Rt7UKg-5JF-PvQ'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: 412786a7-b8da-5b9d-8c3f-2539a3faad9f
    internal-label: Sales Insight Actions
topic_v2:
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
    internal-label: Privacy
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 82%
---
# 登録解除の概要 {#unsubscribe-overview}

組織によるメールのプライバシーに関する法律への準拠はますます重要になっています。 これに対応するために、アドビは登録解除エクスペリエンスをいくつか強化しました。

* 登録解除リンクは、[!DNL Marketo Sales] および [!DNL Salesforce] から送信されるすべてのメールに配置されます（[!DNL Outlook] または Gmail から送信されるカスタムメールには適用されません）
* 管理者は、チーム全体の登録解除メッセージを編集できます。
* 登録解除情報は PDV に保存されます。
* 登録解除は手動で行うことができます。クリック済みリンク、[!DNL Salesforce] 同期、バウンスです。
* 新しい登録解除リンク付きランディングページ

## 登録解除リンクのランディングページ {#unsubscribe-link-landing-page}

人物が登録解除リンクをクリックすると、登録解除用のランディングページが表示され、登録解除する対象とその理由を選択できます。

![](assets/unsubscribe-overview-1.png)

この情報は、後で表示できるように人物の詳細ビューに保存されます。

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
   <td><p>再購読：[!DNL Sales Connect] 管理者が、取引先責任者レコードから登録解除を手動で削除した。 また、取引先責任者の配信停止理由に関する詳細も表示されます。</p><p>登録解除：取引先責任者が登録解除されました。</p></td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL ソース]</strong></td>
   <td><p>[!DNL Salesforce] 同期：登録解除が [!DNL Salesforce] の同期によって取得された。</p><p>手動：ユーザーが「登録解除」ボタンをクリックしてオプトアウトしました。</p><p>リンクをクリック：メールの受信者が登録解除リンクをクリックしました。</p><p>「管理者名」：管理者の名前は、アクションが取引先責任者の再購読の場合に表示されます。 これにより、配信停止を削除した人をユーザに知らせます。</p></td>
  </tr>
 </tbody>
</table>

>[!MORELIKETHIS]
>
>[配信停止リンクメッセージのカスタマイズ](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
