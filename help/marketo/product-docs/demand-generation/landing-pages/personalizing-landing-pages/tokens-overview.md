---
unique-page-id: 2950799
description: トークンの概要 - Marketo ドキュメント - 製品ドキュメント
title: トークンの概要
exl-id: d60816ce-33fb-4e18-8acd-71d4e90f47de
source-git-commit: 4fc3cf6e6458f07df7cced9399831b8c6b50e0ad
workflow-type: ht
source-wordcount: '300'
ht-degree: 100%

---

# トークンの概要 {#tokens-overview}

トークンは、Marketo スマートキャンペーンのフローステップ、メール、ランディングページ、スニペット、Web キャンペーンで使用できる変数です。

## デフォルト値について {#understanding-default-values}

トークンを使用する場合は、デフォルト値も指定する必要があります。これは、参照しているフィールドの値がユーザーに割り当てられていない場合に示すテキストです。

![](assets/image2014-12-2-13-3a16-3a48.png)

この例では、メールに「Greetings, （名前）」または「Greetings, earthling」（デフォルト値）と表示されます。

![](assets/two.png)

>[!CAUTION]
>
>Marketo メールエディターを使用している際には、トークンはプリヘッダーで機能しません。プリヘッダーでトークンを使用するには、メールテンプレートで独自の HTML を使用する必要があります。

>[!NOTE]
>
>このリストは完全なものではありません。また、トークンは、Marketo のすべてのカスタムフィールドに対しても作成されます。

## ユーザートークン {#person-tokens}

* `{{lead.Acquisition Date}}`
* `{{lead.Acquisition Program Name}}`
* `{{lead.Acquisition Program}}`
* `{{lead.Address}}`
* `{{lead.Anonymous IP}}`
* `{{lead.Black Listed}}`
* `{{lead.City}}`
* `{{lead.Country}}`
* `{{lead.Created At}}`
* `{{lead.Date of Birth}}`
* `{{lead.Department}}`
* `{{lead.Do Not Call}}`
* `{{lead.Do Not Call Reason}}`
* `{{lead.Email Address}}`
* `{{lead.Email Invalid}}`
* `{{lead.Email Invalid Cause}}`
* `{{lead.Fax Number}}`
* `{{lead.First Name}}`
* `{{lead.Full Name}}`
* `{{lead.Id}}`
* `{{lead.Inferred City}}`
* `{{lead.Inferred Company}}`
* `{{lead.Inferred Country}}`
* `{{lead.Inferred Metropolitan Area}}`
* `{{lead.Inferred Phone Area Code}}`
* `{{lead.Inferred Postal Code}}`
* `{{lead.Inferred State Region}}`
* `{{lead.Is Customer}}`
* `{{lead.Is Employee}}`
* `{{lead.Is Partner}}`
* `{{lead.Job Title}}`
* `{{lead.Last Name}}`
* `{{lead.Lead Source}}`
* `{{lead.Marketing Suspended}}`
* `{{lead.Middle Name}}`
* `{{lead.Mobile Phone Number}}`
* `{{lead.Original Referrer}}`
* `{{lead.Original Search Engine}}`
* `{{lead.Original Search Phrase}}`
* `{{lead.Original Source Info}}`
* `{{lead.Original Source Type}}`
* `{{lead.Person Notes}}`
* `{{lead.Phone Number}}`
* `{{lead.Registration Source Info}}`
* `{{lead.Registration Source Type}}`
* `{{lead.Salutation}}`
* `{{lead.SFDC Created Date}}`
* `{{lead.SFDC Is Deleted}}`
* `{{lead.SFDC Type}}`
* `{{lead.Unsubscribed}}`
* `{{lead.Unsubscribed Reason}}`
* `{{lead.Updated At}}`
* カスタムユーザーフィールドは、表示名を使用する場合にも機能します（例：`{{lead.Custom Field Name}}`）。

## 会社トークン {#company-tokens}

* `{{Company.Account Owner Email Address}}`
* `{{Company.Address}}`
* `{{Company.Annual Revenue}}`
* `{{Company.City}}`
* `{{Company.Company Name}}`
* `{{Company.Company Notes}}`
* `{{Company.Country}}`
* `{{Company.Industry}}`
* `{{Company.Main Phone}}`
* `{{Company.Num Employees}}`
* `{{Company.Parent Company Name}}`
* `{{Company.Postal Code}}`
* `{{Company.SFDC Account Num}}`
* `{{Company.SFDC Created Date}}`
* `{{Company.SFDC Type}}`
* `{{Company.SIC Code}}`
* `{{Company.Site}}`
* `{{Company.State}}`
* `{{Company.Website}}`
* また、表示名の例を使用する場合は、カスタムの会社フィールドも機能します（例：`{{Company.Custom Field Name}}`）。

## キャンペーントークン {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## システムトークン {#system-tokens}

>[!NOTE]
>
>これらのトークンの詳細については、[システムトークンの用語集](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md)を参照してください。

* `{{system.date}}`
* `{{system.time}}`
* `{{system.dateTime}}`
* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

## トリガートークン {#trigger-tokens}

* `{{trigger.Trigger Name}}`
* `{{trigger.Name}}`
* `{{trigger.Link}}`
* `{{trigger.Subject}}`
* `{{trigger.Category}}`
* `{{trigger.Details}}`
* `{{trigger.Web Page}}`
* `{{trigger.Client IP Address}}`
* `{{trigger.Sent By}}`
* `{{trigger.Received By}}`
* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!NOTE]
>
>スマートキャンペーンで使用されるトリガーに基づいて、[興味深い瞬間のトークン](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md)に関する詳細を検索します。

## プログラムトークン {#program-tokens}

* `{{program.Name}}`
* `{{program.Description}}`
* `{{program.id}}`

## マイトークン {#my-tokens}

マイトークンはプログラム内で定義されれいます。マイトークンは `{{my.` から始まり、その後に、トークン用に作成した名前が続きます。[プログラム内のマイトークン](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)を参照してください。

## メンバートークン {#member-token}

メンバートークンは、統合サービスパートナーから一意の値を挿入するために使用されます。メンバートークンの一般的な使用方法は、ウェビナー参加者向けの一意の URL です。各人は、`{{member.webinar url}}` トークンを使用して挿入できるウェビナーにアクセスするための一意の URL を持っています。`{{member.webinar url}}` トークンは、サービスプロバイダーによって生成されたユーザーの一意の確認 URL を自動的に解決します。

* `{{member.webinar url}}`

>[!CAUTION]
>
>`{{member.webinar url}}` トークンは、メールを送信するスマートキャンペーンがイベントプログラムの子アセットである場合にのみ入力されます。
