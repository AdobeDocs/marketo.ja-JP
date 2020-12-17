---
unique-page-id: 2952678
description: アラート情報トークンの送信{{SP_Send_Alert_Info}} - Marketto Docs — 製品ドキュメントの使用
title: アラート情報トークンの送信の使用
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# アラート情報トークンの送信{#use-the-send-alert-info-token-sp-send-alert-info}を使用

`{{SP_Send_Alert_Info}}`トークンは、セールスチーム向けのアラート電子メールを作成する際に使用する特別なトークンです。

>[!TIP]
>
>このトークンは、[アラート](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md)の送信フロー手順を含む電子メールを送信する場合にのみ意図したとおりに機能します。 「電子メールの送信」フローステップで使用する場合は機能しません。

アラートの例：   ![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>立て！ アラート内のURLには有効期限があるので、これらのタイプのメッセージをサポートするカデンスがあることを確認してください。 有効期限は管理者[が設定した&lt;a0/>日付です。](../../../../product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md)

`{{SP_Send_Alert_Info}}`には次の情報が含まれています。

* マーケティング担当者の詳細へのリンクとしての名と姓
* CRM内のユーザーへのリンク
* アラートを送信したマーケティング担当者のキャンペーン名。
* アラートが送信された時刻

>[!NOTE]
>
>CRMへのリンクは、そのユーザーがCRMシステムにいる場合（現在、Dynamics CRMでは利用できません）にのみ表示されます。 リンクは、マーケティング担当者と非マーケティング担当者の両方のユーザーがアクセスできます。

## SP_追加Send_Alert_Infoトークンを電子メールに送信{#add-the-sp-send-alert-info-token-to-an-email}

1. 電子メールを選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/one-3.png)

1. トークンを追加する編集可能領域を重複キーを押しながらクリックします。

   ![](assets/two-3.png)

1. トークンを挿入する場所にカーソルを置き、**「トークンを挿入**」ボタンをクリックします。

   ![](assets/three-3.png)

1. **`{{SP_Send_Alert_Info}}`**&#x200B;トークンを探して選択し、**挿入**&#x200B;をクリックします。

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. 「**保存**」をクリックします。

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>**Reminder**
>
>メールを承認するのを忘れないでください。

いい物だ！ このトークンは非常に役立つので、営業チームに対して作成するすべてのアラートで使用する必要があります。