---
description: Marketoでアクセスおよび削除のプライバシーリクエストを管理する方法について説明します。 Privacy Service UIまたはAPIを介してリクエストを送信し、コンシューマーデータを処理します。
title: プライバシーリクエスト
exl-id: ae61eabc-ad8f-4c7b-8097-838e89c1a3ec
TQID: https://experienceleague.adobe.com/o4xyJMLpbHADyAhsfVbxnQA-WdXfhSx-LCmN9-4IvYI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2: id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 371
ht-degree: 77%

---

# プライバシーリクエスト {#privacy-requests}

このドキュメントでは、Privacy ServiceUI および Privacy Service API を介して Marketo Engage に送信できる個々のデータプライバシーリクエストの管理の概要を説明します。

>[!NOTE]
>
>Marketo Engage 用に Privacy Service UI または API を通じて送信されたプライバシーリクエストは、次に示す場合にのみ適用されます。
>
>* Adobe Identity Management システムにオンボーディングした Marketo Engage ユーザ
>
>**- または -**
>
>* Marketo Engageを使用しているユーザーは、既にAdobe Identity Managementシステム上にある別のExperience Cloud製品（RT-CDP、B2B、B2P Editions、Audience Managerなど）を使用しています。

消費者データにアクセスして Marketo Engage から削除する個々のリクエストを送信するには、次の 2 つの方法があります。

* Privacy Service UI：`https://experience.adobe.com/#/@YOURCOMPANYNAME/privacy` を使用する。 [こちら](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html?lang=ja){target="_blank"}のドキュメントを参照してください。
* Privacy Service API を使用する。 [こちら](https://developer.adobe.com/experience-platform-apis/references/privacy-service/){target="_blank"}のドキュメントと[こちら](https://developer.adobe.com/experience-platform-apis/){target="_blank"}の API 情報を参照してください。

[Privacy Service](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html?lang=ja){target="_blank"} では、データアクセスとデータ削除の 2 種類のリクエストがサポートされます。

## Marketo Engage のリクエストを送信するために必要な設定 {#required-setup-to-send-requests-for-marketo-engage}

データのアクセスおよび削除をリクエストして Marketo Engage を実行するには、次の操作をおこなう必要があります。

1. 以下を特定します。

   a. IMS Org ID<br/>
b. アクションを実行するユーザーの電子メールアドレス

   IMS 組織 ID は、24 文字の英数字から成る文字列で、末尾に @AdobeOrg が付きます。 マーケティング部門または社内のAdobe システム管理者が組織のIMS組織IDを知らない場合は、Adobe サポート（`gdprsupport@adobe.com`）にお問い合わせください。 Privacy API にリクエストを送信するには、IMS 組織 ID が必要です。

1. Privacy Service では、アクセスリクエストと削除リクエストを Marketo Engage に送信し、既存のリクエストのステータスを確認できます。

## Marketo Engage JSON リクエストの必須フィールド値 {#required-field-values-in-marketo-engage-json-requests}

“companyContexts”：

* &quot;namespace&quot;：**imsOrgID**
* &quot;value&quot;：`<Your IMS Org ID Value>`

&quot;users&quot;：

* &quot;action&quot;：**access** または **delete** のいずれか
* “userIDs”：
   * &quot;namespace&quot;: **電子メール**
   * “type”：**standard**
   * &quot;value&quot;：`<Data Subject's Email Address>`

“include”：

* **marketo**（リクエストに適用される Adobe 製品）

“regulation”：

* **gdpr、**、**ccpa**、**pdpa**、**lgpd_bra****nzpa_nzl** のいずれか（リクエストに適用されるプライバシー規則）

## 例 1：GDPR 削除リクエスト {#gdpr-delete-request}

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
          "namespace": "Email",
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
              "namespace": "Email",
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

## 例 2：CCPA アクセスリクエスト {#ccpa-access-request}

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
          "namespace": "Email",
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
              "namespace": "Email",
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
>[プライバシー管理](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md){target="_blank"}
