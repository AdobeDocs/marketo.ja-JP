---
unique-page-id: 2952678
description: メールでアラート情報を送信トークンを使用する方法を説明します。 時間やプログラム名などの送信詳細を動的に挿入します。
title: アラート情報送信トークンの使用
exl-id: 950eb4d1-35d5-4e5c-9624-a38284bff987
feature: Tokens
TQID: 'https://experienceleague.adobe.com/aGDNauucFt-af6OXYlELf-jPMbWKoWZx1VAs7rOIhRs'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: a6d52c76-712f-5f64-a879-9c65c1499322
    internal-label: Tokens
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 92%
---
# アラート情報送信トークンの使用 {#use-the-send-alert-info-token-sp-send-alert-info}

`{{SP_Send_Alert_Info}}` トークンは、セールスチームのアラートメールを作成する際に使用する特別なトークンです。

>[!TIP]
>
>このトークンは、そのトークンを含むメールを[アラートを送信](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md)フローステップで送信する場合のみに機能します。 Send Email フローステップで使用された場合は機能しません。

アラートの例：

![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>ご注意ください。 アラート内の URL には有効期限があるので、これらのタイプのメッセージをサポートするケイデンスが設定されていることを確認してください。 有効期限は[管理者が設定](/help/marketo/product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md)します。

以下の情報が `{{SP_Send_Alert_Info}}` の一部として含まれています。

* Marketo の人物詳細へのリンクとして表示される名と姓
* CRM 内の人物へのリンク
* アラートを送信した Marketo のキャンペーン名
* アラートが送信された時刻

>[!NOTE]
>
>CRM へのリンクは、その人物が CRM システムに存在する場合にのみ表示されます（現在は Dynamics CRM では使用できません）。 このリンクには、Marketo ユーザーと Marketo 以外のユーザーの両方がアクセスできます。

## SP_Send_Alert_Info トークンをメールに追加する {#add-the-sp-send-alert-info-token-to-an-email}

1. メールを選択して、「**[!UICONTROL ドラフトを編集]**」をクリックします。

   ![](assets/one-3.png)

1. トークンを追加する編集可能領域をダブルクリックします。

   ![](assets/two-3.png)

1. トークンを配置する場所にカーソルを置き、「**[!UICONTROL トークンを挿入]**」ボタンをクリックします。

   ![](assets/three-3.png)

1. **[!UICONTROL `{{SP_Send_Alert_Info}}`]** トークンを検索して選択し、「**[!UICONTROL 挿入]**」をクリックします。

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>忘れずにメールを承認してください。

これは強力です。 このトークンは非常に役に立つので、セールスチーム向けに作成するすべてのアラートで使用してください。
