---
description: プライバシーリクエスト — Marketoドキュメント — 製品ドキュメント
title: プライバシーリクエスト
exl-id: ae61eabc-ad8f-4c7b-8097-838e89c1a3ec
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# プライバシーリクエスト {#privacy-requests}

このドキュメントでは、Privacy ServiceUI および **Privacy ServiceAPI**.

>[!NOTE]
>
>Marketo Engage用にPrivacy ServiceUI または API を通じて送信されたプライバシーリクエストは、Marketo Engage+ RT-CDP、B2B および B2P エディションを持つユーザーにのみ適用されます。

消費者データにアクセスしてMarketo Engageから削除する個々のリクエストを送信するには、次の 2 つの方法があります。

* を通じて [Privacy ServiceUI](https://privacyui.cloud.adobe.io/). ドキュメントを参照してください [ここ](https://www.adobe.io/apis/experienceplatform/home/services/privacy-service.html#!api-specification/markdown/narrative/tutorials/privacy_service_tutorial/privacy_service_ui_tutorial.md).
* を通じて **Privacy ServiceAPI**. ドキュメントを参照してください [ここ](https://www.adobe.io/apis/experienceplatform/home/services/privacy-service.html#!api-specification/markdown/narrative/tutorials/privacy_service_tutorial/privacy_service_api_tutorial.md) と API リファレンス [ここ](https://www.adobe.io/apis/experiencecloud/gdpr/api-reference.html#!acpdr/swagger-specs/privacy-service.yaml).

この [Privacy Service](https://www.adobe.io/apis/experienceplatform/home/services/privacy-service.html) は、次の 2 種類のリクエストをサポートします。データアクセスとデータ削除に関する情報です。

ここでは、アクセスリクエストと削除リクエストの作成方法について説明します。

## Marketo Engageのリクエストを送信するために必要な設定 {#required-setup-to-send-requests-for-marketo-engage}

データのアクセスおよび削除をリクエストしてMarketo Engageを実行するには、次の操作を行う必要があります。

1. 以下を特定します。

   a.IMS Org ID<br/>
b.行動を起こす人のメールアドレス

   IMS Org ID は、24 文字の英数字から成る文字列で、末尾に@AdobeOrgが付きます。 マーケティングチームまたは内部Adobeシステム管理者が組織の IMS Org ID を把握していない場合は、Adobeカスタマーケア (gdprsupport@adobe.com) にお問い合わせください。 プライバシー API にリクエストを送信するには、IMS Org ID が必要です。

1. Privacy Serviceでは、アクセス要求と削除要求をMarketo Engageに送信し、既存の要求のステータスを確認できます。

## Marketo EngageJSON リクエストの必須フィールド値 {#required-field-values-in-marketo-engage-json-requests}

&quot;companyContexts&quot;:

* &quot;namespace&quot;: **imsOrgID**
* “値”: `<Your IMS Org ID Value>`

“ユーザー”:

* &quot;action&quot;:どちらか **アクセス** または **削除**
* &quot;userIDs&quot;:
   * &quot;namespace&quot;: **電子メール**
   * &quot;type&quot;: **標準**
   * “値”: `<Data Subject’s Email Address>`

&quot;include&quot;:

* **marketo** ( リクエストに適用されるAdobe製品 )

&quot;regulation&quot;:

* **gdpr**, **ccpa**, **pdpa**, **lgpd_bra**&#x200B;または **nzpa_nzl**  （リクエストに適用されるプライバシー規則）

## 例 1:GDPR 削除要求 {#gdpr-delete-request}

JSON リクエスト

```text
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "1231659F56A68A8B7F000101@AdobeOrg"
    }
  ],
  "users": [
    {
      "action": [
        "delete"
      ],
      "userIDs": [
        {
          "namespace": "email",
          "type": "standard",
          "value": "john.doe@adobe.com"
        }
      ]
    }
  ],
  "include": [
    "marketo"
  ],
  "regulation": "gdpr",
}
```

JSON 応答

```text
{
  "requestId": "16331241037112570RX-245",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": "997b01e3-9568-402c-904b-b4e60a437875",
      "customer": {
        "user": {
          "action": [
            "delete"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": "john.doe@adobe.com",
              "type": "standard",
              "namespaceId": 6,
              "isDeletedClientSide": false
            }
          ]
        }
      }
    }
  ]
}
```

## 例 2:CCPA アクセス要求 {#ccpa-access-request}

JSON リクエスト

```text
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "1231659F56A68A8B7F000101@AdobeOrg"
    }
  ],
  "users": [
    {
      "action": [
        "access"
      ],
      "userIDs": [
        {
          "namespace": "email",
          "type": "standard",
          "value": "john.doe@adobe.com"
        }
      ]
    }
  ],
  "include": [
    "marketo"
  ],
  "regulation": "ccpa",
}
```

JSON 応答

```text
{
  "requestId": "16329573462631890RX-207",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": "3115e42d-011b-47ab-a2b0-ed4356af4d3e",
      "customer": {
        "user": {
          "action": [
            "access"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": "john.doe@adobe.com",
              "type": "standard",
              "namespaceId": 6,
              "isDeletedClientSide": false
            }
          ]
        }
      }
    }
  ]
}
```

>[!MORELIKETHIS]
>
>[プライバシー管理](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md)
