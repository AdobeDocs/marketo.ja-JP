---
description: プライバシーリクエスト - Marketo ドキュメント - 製品ドキュメント
title: プライバシーリクエスト
exl-id: ae61eabc-ad8f-4c7b-8097-838e89c1a3ec
source-git-commit: 0abb315be0f9cb5f42fa41d72b446de8c2f62c1e
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 85%

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
>* Adobe Identity Management システムに既に存在する別の Experience Cloud 製品（RT-CDP、B2B および B2P エディション、Audience Manager など）を使用する Marketo Engage ユーザ。

消費者データにアクセスして Marketo Engage から削除する個々のリクエストを送信するには、次の 2 つの方法があります。

* [Privacy ServiceUI](https://privacyui.cloud.adobe.io/).を使用する。ドキュメントを参照してください [ここ](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html?lang=ja){target="_blank"}.
* Privacy ServiceAPI.を使用する。ドキュメントを参照してください [ここ](https://developer.adobe.com/experience-platform-apis/references/privacy-service/){target="_blank"} and API information [here](https://developer.adobe.com/experience-platform-apis/){target="_blank"}.

[Privacy Service](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html?lang=ja) では、データアクセスとデータ削除の 2 種類のリクエストがサポートされます。{target="_blank"}

ここでは、アクセスリクエストと削除リクエストの作成方法について説明します。

## Marketo Engage のリクエストを送信するために必要な設定 {#required-setup-to-send-requests-for-marketo-engage}

データのアクセスおよび削除をリクエストして Marketo Engage を実行するには、次の操作をおこなう必要があります。

1. 以下を特定します。

   a. IMS 組織 ID<br/>
b. アクションの対象となるユーザのメールアドレス

   IMS 組織 ID は、24 文字の英数字から成る文字列で、末尾に @AdobeOrg が付きます。マーケティングチームまたは内部Adobeシステム管理者が組織の IMS Org ID を把握していない場合は、Adobeカスタマーケア ( `gdprsupport@adobe.com`. Privacy API にリクエストを送信するには、IMS 組織 ID が必要です。

1. Privacy Service では、アクセスリクエストと削除リクエストを Marketo Engage に送信し、既存のリクエストのステータスを確認できます。

## Marketo Engage JSON リクエストの必須フィールド値 {#required-field-values-in-marketo-engage-json-requests}

&quot;companyContexts&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;value&quot;: `<Your IMS Org ID Value>`

&quot;users&quot;:

* &quot;action&quot;：次のいずれか **アクセス** または **削除**
* &quot;userIDs&quot;:
   * &quot;namespace&quot;: **電子メール**
   * &quot;type&quot;: **標準**
   * &quot;value&quot;: `<Data Subject's Email Address>`

&quot;include&quot;:

* **marketo**（リクエストに適用される Adobe 製品）

&quot;regulation&quot;:

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
