---
description: 配信停止の概要 - Marketo ドキュメント - 製品ドキュメント
title: 配信停止の概要
exl-id: 7598efa9-9686-4dd0-840b-f8b6de4ab2be
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 58%

---

# 配信停止の概要 {#unsubscribe-overview}

組織がメールのプライバシーに関する法律に準拠する重要性が高まっています。これを支援するために、アドビは配信停止エクスペリエンスをいくつか強化しました。

* 購読解除リンクは、[!DNL Marketo Sales] および [!DNL Salesforce] から送信されるすべてのメールに配置されます（[!DNL Outlook] または Gmail から送信されるカスタムメールには適用されません）
* 管理者は、チーム全体の配信停止メッセージを編集できます
* 配信停止情報は PDV に保存されます
* 購読解除は、クリックされたリンク、[!DNL Salesforce] 同期、バウンスから手動で行うことができます
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

管理者の場合は、購読解除グループに移動して [!UICONTROL  アカウントの購読解除 ] でフィルタリングすると、人物データベースに収集されたすべての購読解除を確認できます。

![](assets/unsubscribe-overview-4.png)

## 登録解除履歴カード {#unsubscribe-history-card}

[!UICONTROL  購読解除履歴 ] カードは、管理者とユーザーが連絡先の購読解除履歴に関するコンテキスト情報を取得するのに役立ちます。 [!UICONTROL  人物 ] タブに移動し、人物を選択して、そこに移動します。 これは、人物の詳細表示の [!UICONTROL  説明 ] タブの下部にあります。

>[!NOTE]
>
>ユーザーが [!UICONTROL  再登録 ] した場合にのみ、_登録解除履歴_ カードが表示されます。

![](assets/unsubscribe-overview-5.png)

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL 日付 ]</strong></td> 
   <td><p>配信停止／再購読が行われた日付を表示します。</p></td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL の詳細 ]</strong></td> 
   <td><p>再購読：[!DNL Sales Connect] 管理者が連絡先レコードから手動で購読解除を削除しました。 また、取引先責任者の配信停止理由に関する詳細も表示されます。</p><p>配信停止：取引先責任者が配信停止された。</p></td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Source]</strong></td> 
   <td><p>[!DNL Salesforce] 同期：購読解除が [!DNL Salesforce] からの同期によってキャプチャされました。</p><p>手動：ユーザが「配信停止」ボタンをクリックしてオプトアウトした。</p><p>リンクをクリック：メールの受信者が配信停止リンクをクリックした。</p><p>「管理者名」：管理者の名前は、アクションが取引先責任者の再購読の場合に表示されます。これにより、配信停止を削除した人をユーザに知らせます。</p></td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[配信停止リンクメッセージのカスタマイズ](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
