---
unique-page-id: 2950799
description: トークンの概要 — Marketto Docs — 製品ドキュメント
title: トークンの概要
translation-type: tm+mt
source-git-commit: efadb7eb3845012c273e1a60f9cd98ac884eb543
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---


# トークンの概要 {#tokens-overview}

トークンは、Marketo [スマートキャンペーンフローステップ](http://docs.marketo.com/display/DOCS/Smart+Campaigns) 、電子メール [、](http://docs.marketo.com/display/DOCS/General)ランディングページ [、スニペット、Webキャンペーン、](http://docs.marketo.com/display/DOCS/Landing+Pages)Webペットなど、Marketto Smartフローステップで使用できる変数 [](http://docs.marketo.com/display/DOCS/Segmentation+and+Snippets)[](http://docs.marketo.com/display/public/DOCS/Using+the+Web+Personalization+Rich+Text+Editor)です。

>[!NOTE]
>
>**FYI**
>
>Marketoは現在、すべての購読で言語を標準化しているので、購読およびdocs.marketo.comの人物/人物にリード/リードを表示できます。 これらの用語は同じことを意味し、記事の説明には影響しません。 他にも変化がある。 [詳細情報](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

## デフォルト値について {#understanding-default-values}

トークンを使用する場合は、デフォルト値も指定する必要があります。 これは、参照しているフィールドの値がユーザーにない場合に表示するテキストです。

![](assets/image2014-12-2-13-3a16-3a48.png)

この例では、電子メールは「Greetings, (first name)」または「Greetings, earthling」（デフォルト値）と表示されます。

![](assets/two.png)

>[!CAUTION]
>
>Marketoの電子メールエディターを使用している場合、プリヘッダーでトークンが機能しません。 プリヘッダーでトークンを使用するには、電子メールテンプレート内の独自のHTMLを使用する必要があります。

>[!NOTE]
>
>このリストは完全なものではありません。 また、Marketoにあるすべてのカスタムフィールドに対して、トークンが作成されます。

## Personトークン {#person-tokens}

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
* カスタムユーザーフィールドも、例えば `{{lead.Custom Field Name}}`

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
* カスタム会社フィールドも、表示名exを使用する場合は機能します。 `{{Company.Custom Field Name}}`

## キャンペーントークン {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## システムトークン {#system-tokens}

>[!NOTE]
>
>これらのトークンの詳細については、「 [システムトークン用語集](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md)」を参照してください。

* `{{system.date}}`
* `{{system.time}}`
* `{{system.dateTime}}`
* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

## トークンのトリガー {#trigger-tokens}

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
>スマート [キャンペーンで使用されるトリガーに基づいて](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/tokens-for-interesting-moments.md) 、興味深い瞬間のトークンに関する詳細を確認できます。

## プログラムトークン {#program-tokens}

* `{{program.Name}}`

* `{{program.Description}}`

* `{{program.id}}`

## マイトークン {#my-tokens}

My Tokensはプログラム内で定義され、先頭にトークン用に作成した名前が `{{my.` 続きます。 プログラム内の [マイトークンの詳細を表示します](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)。

## メンバートークン {#member-token}

メンバートークンは、統合サービスパートナーから一意の値を挿入するために使用されます。 メンバートークンは、ウェビナーの出席者固有のURLに使用するのが一般的です。 各ユーザーは、トークンを使用して挿入できるウェビナーにアクセスするための固有のURLを持ってい `{{member.webinar url}}` ます。 トー `{{member.webinar url}}` クンは、サービスプロバイダーが生成したユーザー固有の確認URLを自動的に解決します。

* `{{member.webinar url}}`

>[!CAUTION]
>
>トー `{{member.webinar url}}` クンは、電子メールを送信するスマートキャンペーンがイベントプログラムの子アセットである場合にのみ設定されます。
