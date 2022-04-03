---
unique-page-id: 2952678
description: アラート情報送信トークン {{SP_Send_Alert_Info}} の使用 - Marketo ドキュメント - 製品ドキュメント
title: アラート情報送信トークンの使用
exl-id: 950eb4d1-35d5-4e5c-9624-a38284bff987
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '264'
ht-degree: 100%

---

# アラート情報送信トークンの使用 {#use-the-send-alert-info-token-sp-send-alert-info}

`{{SP_Send_Alert_Info}}` トークンは、セールスチームのアラートメールを作成する際に使用する特別なトークンです。

>[!TIP]
>
>このトークンは、そのトークンを含むメールを[アラートを送信](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md)フローステップで送信する場合のみに機能します。メールを送信フローステップで使用された場合は機能しません。

アラートの例：

![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>ご注意ください。アラート内の URL には有効期限があるので、これらのタイプのメッセージをサポートするケイデンスが設定されていることを確認してください。有効期限は[管理者が設定](/help/marketo/product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md)します。

以下の情報が `{{SP_Send_Alert_Info}}` の一部として含まれています。

* Marketo でのユーザーの詳細へのリンクとしての姓と名
* CRM 内のユーザーへのリンク
* アラートを送信した Marketo のキャンペーン名
* アラートが送信された時刻

>[!NOTE]
>
>CRM へのリンクは、そのユーザーが CRM システムに存在する（現在 Dynamics CRM では使用不可）場合にのみ表示されます。このリンクには、Marketo ユーザーと Marketo 以外のユーザーの両方がアクセスできます。

## SP_Send_Alert_Info トークンをメールに追加する {#add-the-sp-send-alert-info-token-to-an-email}

1. メールを選択して、「**ドラフトを編集**」をクリックします。

   ![](assets/one-3.png)

1. トークンを追加する編集可能領域をダブルクリックします。

   ![](assets/two-3.png)

1. トークンを配置する場所にカーソルを置き、「**トークンを挿入**」ボタンをクリックします。

   ![](assets/three-3.png)

1. **`{{SP_Send_Alert_Info}}`** トークンを検索して選択し、「**挿入**」をクリックします。

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. 「**保存**」をクリックします。

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>忘れずにメールを承認してください。

これは強力です。このトークンは非常に役に立つので、セールスチームに対して作成するすべてのアラートでご使用ください。
