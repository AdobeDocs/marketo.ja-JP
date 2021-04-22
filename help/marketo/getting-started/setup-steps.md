---
unique-page-id: 2949469
description: セットアップ手順 —Marketoドキュメント — 製品ドキュメント
title: 設定手順
exl-id: ef6b7311-55ca-4384-a24c-714eae89a57d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '2004'
ht-degree: 0%

---

# セットアップ手順{#setup-steps}

**Marketo へようこそ!**

Marketoの使い方を学ぶ前に、いくつかの手順を完了する必要があります。

次の手順を実行します。

* いくつかの基本的なアカウント設定
* 信頼性と配信品質を向上させるために、ランディングページのURLと電子メールのリンクのブランド化を行う
* CRMの同期
* 会社のWebサイトへのトラッキングコードの追加

>[!NOTE]
>
>会社が&#x200B;**Marketo**&#x200B;に新しい場合にのみ、これらの手順を実行する必要があります。 そうでない場合は、既に設定が完了している可能性があります。

一部の手順では、ITチームからの支援が必要です。

>[!TIP]
>
>[このチェックリスト](/help/marketo/getting-started/setup-steps/setup-checklist.md)を印刷すると、項目を完了する際にチェックオフできます。

## ログインして、追加のMarketoユーザーを作成{#log-in-and-create-additional-marketo-users}

1. 電子メールで受け取った資格情報を使用して、Marketo[ここ](https://app.marketo.com/)にログインします。

   ![](assets/new-login-screen-hand.jpg)

おめでとうございます！今はMarketoにいて、開始が調査できる マーケティングチームの同僚を招待して参加させることもできます。 これは、新しいユーザーを追加することで行うことができます。

**管理者**&#x200B;領域に移動します。

>[!TIP]
>
>ここにいる間に、「**マイアカウント**」をクリックしてアカウントと場所の設定を変更し、新しい購読名を設定できます。

![](assets/admin.png)

>[!NOTE]
>
>**必要な管理者権限**

「**ユーザーとロール**」をクリックします。

![](assets/image2015-1-6-13-3a14-3a43.png)

「**新しいユーザーを招待**」をクリックします。

![](assets/image2015-1-6-13-3a14-3a6.png)

同僚の電子メールアドレス、名、姓を入力します。

![](assets/image2016-5-24-10-3a11-3a12.png)

必要に応じて、カレンダーピッカーを使用して、招待の理由とアクセス有効期限を入力します。 「**OK**」をクリックします。

![](assets/image2016-5-24-10-3a13-3a9.png)

「**次へ**」をクリックします。

![](assets/image2016-5-24-10-3a14-3a9.png)

>[!TIP]
>
>有効期限は、短期間のみMarketoにアクセスする必要がある、外部の関係者またはコンサルタントに適しています。

>[!NOTE]
>
>有効期限が到達すると、ユーザーは有効期限の通知を受け取り、アカウントはロックされます。

ロールを選択し、「**次へ**」をクリックします。 標準ユーザーは、管理者以外のすべての領域にアクセスできます。

![](assets/image2016-5-24-10-3a14-3a51.png)

>[!NOTE]
>
>5つの組み込みの役割に加えて、カスタムの役割を作成することもできます。 [ユーザーの役割と権限の管理](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md)の詳細を参照してください。

招待のテキストは自由に調整してください。 「**送信**」をクリックします。

![](assets/image2016-5-24-10-3a15-3a52.png)

これで、新しいユーザーが「ユーザー」タブに表示され、パスワードとログインを作成するためのリンクが記載された電子メールを受信します。 次のステップ！

![](assets/image2016-5-24-10-3a23-3a10.png)

## 承認されたサポートの連絡先を設定{#set-up-your-authorized-support-contacts}

お客様は、お客様の会社のMarketoカスタマーサポート管理者であることを伝える電子メールをMarketoサポートから受け取った可能性があります。 その場合は、**承認されたサポートの連絡先**&#x200B;をチーム用に設定できます。 [Marketoサポートポータル](https://support.marketo.com)を介して直接、Marketoカスタマーサポートに連絡できるのは、承認されたサポート担当者のみです。

>[!NOTE]
>
>作成できるサポートの連絡先の数は、購入したパッケージによって異なります。 この制限は、Marketoサポートからの電子メールで指定します。

認定サポート連絡先ドキュメントは、Marketoコミュニティに移動しました。 [この記事](https://nation.marketo.com/t5/Knowledgebase/Managing-Authorized-Support-Contacts/ta-p/254341)を参照してください。

>[!NOTE]
>
>Marketoコミュニティにログインした人のみがリストに表示されます。 そのユーザーが見つからない場合は、まずコミュニティにログインしていることを確認してください。

## CNAME {#customize-your-landing-page-urls-with-a-cname}でランディングページURLをカスタマイズする

>[!NOTE]
>
>Launch Packのお客様ですか。 この手順はスキップできます。 キックオフ会議中に、担当のコンサルタントからITのセットアップに関する指示ドキュメントが提供されます。

>[!NOTE]
>
>**必要な管理者権限**

ランディングページのCNAMEを選択します。 例を次に示します。

    * **go**.[CompanyDomain].com
    * **www2**.[CompanyDomain].com
    * **lp**.[CompanyDomain].com

>[!TIP]
>
>手短に！ 短いURLを指定すると、覚えやすくなります。 「行く」をドメインとしてお勧めします。

最初の部分（太字）は`[LandingPageCNAME]`です。 手順5で必要になります。

ランディングページのCNAMEと置き換えるアカウント文字列を取得するには、「管理者」領域に移動します。

![](assets/admin.png)

**ランディングページ**&#x200B;をクリックします。

![](assets/image2015-1-6-13-3a52-3a6.png)

ランディングページ設定から「アカウント文字列」をコピーします。

![](assets/image2015-1-6-13-3a53-3a19.png)

これは`[AccountString]`です。 保存します。 手順5でITに渡す必要があります。

ランディングページが（ドメインがホストされている場所で）Marketoのドメインではなく、会社のドメインを使用するように、ドメイン設定を指定します。

## 電子メールの配信品質を確認{#ensure-email-deliverability}

>[!NOTE]
>
>Launch Packのお客様ですか。 この手順はスキップできます。 キックオフ会議中に、担当のコンサルタントからITのセットアップに関する指示ドキュメントが提供されます。

電子メールができるだけ多くの人に届くように、いくつかの方法が考えられます。

    1.**トラッキングリンクをブランド化** CNAMEを選択して、(Marketoの代わりに)Marketoからの電子メールに含めるリンクに、自分のドメインを使用できます。 これにより、ドメインのブランディングが強化され、受信者の信頼と配信品質が向上します。
    1.**追加Marketoを社内の電子メール許可リストに送信します。**テスト用の電子メールを実際のユーザーに送信する前に、テスト用の電子メールをテストアカウントに送信するのは、一般的なベストプラクティスです。 Marketo許可リストに加えるは、これらのテスト電子メールがブロックされたりスパムとしてフラグ付けされたりするのを防ぐことができます。
    1.**SPFとDKIMを設定します。**これらのテクノロジーは、Marketoの電子メールがスパムでないことを受信者に保証します。 受信者のスパムフィルターがMarketo電子メールを拒否するのを防ぐには、次の手順に従って[Setup a SPF and DKIM for Your Email Deliverability](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md)を実行します。
    1.**ドメインのMXレコードを設定します。** MXレコードを使用すると、返信や自動返信を処理するために、電子メールの送信元のドメインにメールを受信できます。 会社ドメインから送信する場合は、既にこの設定が行われている可能性があります。 そうでない場合は、通常、会社ドメインのMXレコードにマップするように設定できます。
    1.**送信元アドレスの推奨設定**すべての電子メールキャンペーンの「送信者アドレス」に、有効な既存の有効な電子メールドメインおよび作業中の電子メールドメインを使用する必要があります。 会社ドメインから送信するのではなく、会社ドメインのサブドメインを設定する方が効果的な場合があります。 これにより、会社のメールストリームの問題がMarketoのメールストリームに影響を与えず、逆も同様に影響を与えません。 さらに、something@nonexistentdomain.comからのメールの送信は、電子メールがフィルタされたりブロックされたりする原因となります。 送信者の差出人アドレスで使用されるドメインには、有効で作業中のpostmaster@アカウントとavuse@アカウントが必要です。
    Googleアプリを使用して会社の電子メールをホストしている場合は、ドメインの下で悪用箇所@電子メールまたはポストマスター@電子メールを作成できません。この問題を回避するには、「abuse」および「postmaster」という名前のグループを作成する必要があります。 これらのグループのメンバーであるユーザーは、これらのアドレスに送信された電子メール(例：postmaster@domain.com)を受信します。 グループ作成の詳しい手順は、[ここ](https://support.google.com/a/answer/33343#adminconsole).
を参照してください。
E メールトラッキングログリンクのCNAMEを選択します(手順3で選択したランディングページCNAMEから&#x200B;_異なる_&#x200B;を選択します)。 例を次に示します。

    * go2.[CompanyDomain].com
    * em.[CompanyDomain].com
    *わあ。[CompanyDomain].com

最初の部分はE メールトラッキングログCNAME `[EmailTrackingCNAME]`です。 手順5でITに渡す必要があります。

>[!CAUTION]
>
>電子メールCNAMEとランディングページCNAMEは異なる必要があります。 また、「track」や「link」のようなCNAMEは使用しないでください。 多くの場合、スパムとしてフラグ付けされます

Marketoトラッキングのリンクを探すには、**管理者**&#x200B;領域に移動します。

![](assets/admin.png)

「**電子メール**」をクリックします。

![](assets/image2015-1-6-13-3a55-3a32.png)

電子メール設定からトラッキングリンクをコピーします。

トラッキングリンクは次の形式で表示されます。`mkto-[a-z][4 digits].com`.

![](assets/email-tracking-link-hand.jpg)

これが`[MktoTrackingLink]`です。 保存します。 手順5でITに渡す必要があります。

「送信者」ドメインを収集します。 Marketoからの電子メール送信に使用するすべての「From」ドメイン（例：`[Sender]@[FromDomain].com`）のリストを作成します。 ほとんどの場合、1つしかありません。

例えば、「marketo.com」、「info.marketo.com」のように指定します。 `[FromDomain1]`、`[FromDomain2]`など 保存します。 手順5でITに渡す必要があります。

リクエストをITに送信するために必要な情報がすべて揃いました。

## ITにプロトコルの設定を依頼{#ask-it-to-configure-protocols}

>[!NOTE]
>
>Launch Packのお客様ですか。 この手順はスキップできます。 キックオフ会議中に、担当のコンサルタントからITのセットアップに関する指示ドキュメントが提供されます。

必要な情報をすべて収集したら、IT部門にリクエストを送信する準備が整います。 以下のテキストをテンプレートとして使用し、太字のテキストを独自の情報に置き換えることができます。

[この記事へのリンクを含めます](/help/marketo/getting-started/setup-steps/configure-protocols-for-marketo.md)。

電子メールにこのテキストを貼り付け、太字のプレースホルダーを置き換えます。

>[!NOTE]
>
>プレースホルダを置き換えるテキストについては、上記の手順3と4を参照してください。 `[LandingPageCNAME]`と`[EmailTrackingCNAME]`は異なる必要があります。

`---------------------------------------------`

Awesome IT管理者様、

マーケティングチームは、現在、Marketoプラットフォームを使用して、アドビの従業員と通信しています。 優れた電子メールの配信品質を確保するには、次の変更を行う必要があります。

`1)` ランディングページに対して、LandingPageCNAMEのDNSエントリ(CNAME)を追加し **[ます]**。**[CompanyDomain]**.com( **[AccountString]**.mktoweb.comを参照)。

`2)` 電子メール内のトラッキングリンクに、EmailTrackingCNAMEにDNSエントリ(CNAME)を追加し **[ます]**。**[CompanyDomain]**.com。MktoTrackingLink **[を参照]**。

`3)` 許可リストMarketo

    *電子メール許可リストでIPアドレスを使用する場合は、次のIPを追加します。199.15.212.0/22192.28.144.0/20
    192.28.160.0/19
    
    185.28.196.0/22
    
    130.248.172.0/24
    
    130.
    
    248.173.0/24
    
    130.
    
    237.104.0/22103.
    
    236.119.0/26103.)4.

注意：IPの短縮リストを環境に固有のにする場合は、Marketoサポートにお問い合わせくだ許可リストさい。

    *スパム対策システムで送信元ドメインを使用している場合は、次を追加します。

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)` SPFとDKIMを設定し、Marketoが署名済みの電子メールを送信する権限を持つようにする必要があります。

`a.` SPFを設定するには、DNSエントリに次の行を追加してください。

IN TXT **[ドメイン]**: v=spf1 mx ip4:**[企業IP]**
<br/>含める：mktomail.com ～all

DNSエントリに既にSPFレコードが存在する場合は、次を追加します。

include:mktomail.com

`[`「 **From** Domain」をドメインからの電子メールに置き換えます(例：会社.com)と **** CorpIP（会社の電子メールサーバーのIPアドレス）255.255.255.255)。Marketo経由で複数のドメインから電子メールを送信する場合は、ITスタッフに各ドメインに対してこの行を1行に追加してもらう必要があります。`]`

`b.` DKIMの場合は、セットアップするドメインごとにDNSリソースレコードを作成してください。署名する各ドメインのホストレコードとTXT値を以下に示します。

**`[DKIMDomain1]`**:「Host Record」 **`[HostRecord1]`** はで、「TXT Value」は **[TXTValue1]**&#x200B;です。

**`[DKIMDomain2]`**:「Host Record」 **`[HostRecord2]`** はで、「TXT Value」はで **`[TXTValue2]`**&#x200B;す。

`[`ここでの **** 手順に従って、各 **** DKIMDomainの設定に対してHostRecordと **** TXTValueをコピーし [ます](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md)。ITスタッフがこの手順を完了した後、**管理者/電子メール/DKIM**&#x200B;の各ドメインを必ず確認してください。`]`

`5)` FROMドメインFromDomain1 **[、FromDomain2]** **[]**&#x200B;などに有効なMXレコードがあることを確認する必要があります。確認できる？ そうでない場合は、弊社の企業ドメインMXレコードにマップするように設定してください。 これにより、Marketo宛ての返信/自動返信を確実に処理できます。

この手順が完了したら、お知らせください。Marketoとのセットアッププロセスを完了できます。

ありがとう！ お前は最高だ！

愛

**`[Your Name]`**

`---------------------------------------------`

電子メールをITに送信します。 ITがこれらのタスクを完了するには、時間がかかる場合があることを理解しています。 手順7に進むこともできますが、Marketoのセットアップを完了するには、手順6に戻る必要があることに注意してください。

## ITが{#complete-your-marketo-setup-after-it-finishes}を終了したら、Marketoのセットアップを完了します。

IT部門がタスクを完了したら、次の手順に従ってランディングページと電子メールのCNAMEを追加し、DKIM署名をアクティブにします。

**Admin**&#x200B;領域に移動し、ランディングページCNAME追加を指定します。

![](assets/admin.png)

ランディングページを選択し、「設定」領域の「**編集**」をクリックします。

![](assets/image2015-1-6-13-3a59-3a15.png)

「ランディングページのドメイン名」フィールドに新しいドメイン名を入力します。 これは次の形式になります。

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/image2015-1-6-14-3a3-3a6.png)

「フォールバックページ」フィールドに、ランディングページが利用できない場合に訪問者に通知するURLを入力します。 フォールバックページがない場合は、会社ホームページを使用できます。 「ホームページ」フィールドに、会社のWebサイトを入力します。

![](assets/image2015-1-6-14-3a2-3a46.png)

「管理者」領域で、「電子メールCNAMEへ追加の電子メール」を選択します

![](assets/image2015-1-6-14-3a5-3a3.png)

下にスクロールし、「**編集**」をクリックします。

![](assets/edit-branding-domain.png)

「Domain」フィールドに、E メールトラッキングログドメインを入力します。 これは次の形式になります。

`[EmailTrackingCNAME].[CompanyDomain].com`.「**保存**」をクリックします。

![](assets/new-branding-domain-9-1.png)

## CRMの統合{#integrate-your-crm}

これは、お客様の設定の最もエキサイティングなステップです。CRMに保存したすべてのリードや連絡先をMarketoに埋め込むタイミングです。

会社が使用するCRMに応じて、次の中から選択します。

    * [MarketoとSalesforce.comの統合](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
    * [MarketoとMicrosoft Dynamicsの統合](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

>[!NOTE]
>
>これらの手順を実行するには、会社のCRM管理者の支援が必要です。

## Webサイト追加へのトラッキングコード{#add-tracking-code-to-your-website}

>[!NOTE]
>
>Launch Packのお客様ですか。 この手順はスキップできます。 担当のコンサルタントが、ITセットアップ手順ドキュメントのMunchkinコードの手順を提供します。

Marketoには、任意のウェブページ上の個人アクティビティを追跡するために使用できる、カスタムの追跡JavaScript(Munchkin)が用意されています。 Munchkinは、貴社のウェブサイトをMarketoに統合するために必要です。 以下の手順に従って、[追加貴社のウェブサイト](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)に対するマンチキントラッキングコードを作成します。

>[!NOTE]
>
>トラッキングコードの追加に必要なHTMLの使用経験がある。

すべての設定手順は終了です。 あとはMarketoに飛び込んで使うだけ！
