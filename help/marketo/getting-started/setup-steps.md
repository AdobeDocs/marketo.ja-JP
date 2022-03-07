---
unique-page-id: 2949469
description: 設定手順 - Marketo ドキュメント - 製品ドキュメント
title: 設定手順
exl-id: ef6b7311-55ca-4384-a24c-714eae89a57d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '2004'
ht-degree: 100%

---

# 設定手順 {#setup-steps}

**Marketo へようこそ！**

Marketo を使用する前に、いくつかの手順を完了する必要があります。

次の手順が含まれます。

* いくつかの基本的なアカウント設定
* ランディングページの URL とメールリンクのブランディングによる信頼性と配信品質の向上
* CRM の同期
* 会社の web サイトへのトラッキングコードの追加

>[!NOTE]
>
>自社に **Marketo を初めて導入する**&#x200B;お客様は、これらの手順を行うだけで完了できます。初めてではない場合は、既に設定が完了している可能性があります。

一部の手順では、IT チームのサポートが必要です。

>[!TIP]
>
>[このチェックリストを印刷する](/help/marketo/getting-started/setup-steps/setup-checklist.md)と、チェックを入れて完了を確認することができます。

## ログインして追加の Marketo ユーザーを作成する {#log-in-and-create-additional-marketo-users}

1. メールで受け取った資格情報を使用して、[ここ](https://app.marketo.com/)から Marketo にログインします。

   ![](assets/new-login-screen-hand.jpg)

おめでとうございます！Marketo で探索を開始できます。マーケティングチームの同僚を招待して参加させるには、新しいユーザーを追加します。

「**管理者**」領域に移動します。

>[!TIP]
>
>ここで、「**マイアカウント**」をクリックして、アカウントと場所の設定の変更と、新しいサブスクリプション名を設定できます。

![](assets/admin.png)

>[!NOTE]
>
>**管理者権限が必要**

「**ユーザーと役割**」をクリックします。

![](assets/image2015-1-6-13-3a14-3a43.png)

「**新しいユーザーを招待**」をクリックします。

![](assets/image2015-1-6-13-3a14-3a6.png)

同僚のメールアドレス、氏名を入力します。

![](assets/image2016-5-24-10-3a11-3a12.png)

必要に応じて、招待の理由と、カレンダーピッカーを使用してアクセス有効期限を入力します。「**OK**」をクリックします。

![](assets/image2016-5-24-10-3a13-3a9.png)

「**次へ**」をクリックします。

![](assets/image2016-5-24-10-3a14-3a9.png)

>[!TIP]
>
>有効期限は、Marketo に短時間のみアクセスする必要がある、短期間の外部の関係者やコンサルタントに最適です。

>[!NOTE]
>
>有効期限が来ると、ユーザーは有効期限通知を受け取り、アカウントがロックされます。

役割を選択し、「**次へ**」をクリックします。標準ユーザーは、管理者領域を除くすべての領域にアクセスできます。

![](assets/image2016-5-24-10-3a14-3a51.png)

>[!NOTE]
>
>5 つの組み込みの役割に加えて、カスタムの役割を作成することもできます。詳しくは、[ユーザーの役割と権限の管理](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md)を参照してください。

招待のテキストは自由に変更できます。「**送信**」をクリックします。

![](assets/image2016-5-24-10-3a15-3a52.png)

新しいユーザーが「ユーザー」タブに表示され、ユーザーは、パスワードとログインを作成するためのリンクが記載されたメールを受け取ります。次の手順へ進みます。

![](assets/image2016-5-24-10-3a23-3a10.png)

## 認証済みのサポート連絡先を設定する {#set-up-your-authorized-support-contacts}

Marketo サポートから、ご自身が自社の Marketo カスタマーサポート管理者であることを示すメールを受け取っている可能性があります。その場合は、ご自身のチームに&#x200B;**認証済みのサポート連絡先**&#x200B;を設定できます。認証済みのサポート連絡先のみが、[Marketo サポートポータル](https://support.marketo.com)を使用して、直接 Marketo カスタマーサポートに問い合わせることができます。

>[!NOTE]
>
>作成できるサポート連絡先の数は、購入したパッケージによって異なります。この制限は、Marketo サポートからメールで指定されます。

認証済みサポート連絡先ドキュメントは、Marketo コミュニティに移動しました。詳しくは、[この記事](https://nation.marketo.com/t5/Knowledgebase/Managing-Authorized-Support-Contacts/ta-p/254341)を参照してください。

>[!NOTE]
>
>Marketo コミュニティにログインしたユーザーのみがリストに表示されます。ユーザーが見つからない場合は、最初にコミュニティにログインしてください。

## CNAME を使用したランディングページ URL をカスタマイズ {#customize-your-landing-page-urls-with-a-cname}

>[!NOTE]
>
>Launch Pack をご利用の場合は、この手順をスキップできます。初回コール時に、担当のコンサルタントが IT セットアップ手順書を提供します。

>[!NOTE]
>
>**管理者権限が必要**

ランディングページの CNAME を選択します。次に例を示します。

    * **go**.[CompanyDomain].com
    * **www2**.[CompanyDomain].com
    * **lp**.[CompanyDomain].com

>[!TIP]
>
>短くするようにします。URL は短いほど覚えやすくなります。ドメインには「go」を指定することをお勧めします。

最初の部分（太字）が `[LandingPageCNAME]` です。これは、手順 5 で必要になります。

ランディングページ CNAME に置き換えるアカウント文字列を取得するには、「管理者」領域に移動します。

![](assets/admin.png)

「**ランディングページ**」をクリックします。

![](assets/image2015-1-6-13-3a52-3a6.png)

ランディングページ設定から、アカウント文字列をコピーします。

![](assets/image2015-1-6-13-3a53-3a19.png)

これが `[AccountString]`.です。保存します。これは、手順 5 で IT チームに渡す必要があります。

ランディングページが（ホストされている場所で）Marketo ドメインではなく、自社のドメインを使用するように、ドメイン設定を指定します。

## メールの配信品質を確保する {#ensure-email-deliverability}

>[!NOTE]
>
>Launch Pack をご利用の場合は、この手順をスキップできます。初回コール時に、担当のコンサルタントが IT セットアップ手順書を提供します。

メールができるだけ多くの人に届くように、いくつかの方法が用意されています。

    1.**トラッキングリンクのブランディング**。Marketo からのメールに含めるリンクに、（Marketo ドメインではなく）独自のドメインを使用する CNAME を選択できます。これにより、ドメインのブランディングが強化され、受信者との信頼と配信品質が向上します。
    1.**Marketo を自社のメール許可リストに追加します。**実際の人々にメールを送信する前に、テストアカウントにテストメールを送信するのが一般的なベストプラクティスです。Marketo を許可リストに加えることで、これらのテストメールがブロックされたりスパムとしてフラグ付けされたりするのを防ぐことができます。
    1.**SPF と DKIM を設定します。**これらのテクノロジーは、Marketo のメールがスパムではないことを受信者に保証します。受信者のスパムフィルターによる Marketo メールの拒否を防ぐには、次の手順に従って [メールの配信品質に SPF と DKIM を設定します]。（/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md）
    1.**ドメインの MX レコードを設定します。**MX レコードを使用すると、返信や自動返信を処理するために、メールを送信するドメインにメールを受け取ることができます。会社ドメインから送信する場合は、既にこの設定が完了している可能性があります。そうでない場合は、通常、会社ドメインの MX レコードにマッピングするように設定できます。
    1.**送信元アドレスの推奨設定。**すべてのメールキャンペーンの送信元アドレスに、有効な既存メールドメインと動作中のメールドメインを使用する必要があります。会社ドメインから送信するのではなく、会社ドメインのサブドメインを設定すると便利です。これにより、会社のメールストリームの問題が Marketo のメールストリームに影響を与えず、逆についても同様のことが言えます。さらに、something@nonexistentdomain.com からメールを送信すると、メールがフィルターされたりブロックされたりします。送信者の送信元アドレスで使用されるドメインには、有効で動作中の postmaster@ アカウントと abuse@ アカウントが必要です。
    Google アプリを使用して自社のメールをホストしている場合、お使いのドメインで abuse@ や postmaster@ のメールを作成することはできません。この問題を回避するには、「abuse」および「postmaster」という名前のグループを作成する必要があります。このグループのメンバーであるユーザーは、そのアドレスに送信されたメールを受信します（例：postmaster@domain.com）。グループ作成の詳しい手順については、[こちら]（https://support.google.com/a/answer/33343#adminconsole）を参照してください。

メールトラッキングリンクの CNAME を選択します（手順 3 で選択したランディングページ CNAME とは&#x200B;_異なる_&#x200B;ものを選択）。次に例を示します。

    * go2.[CompanyDomain].com
    * em.[CompanyDomain].com
    * wow.[CompanyDomain].com

最初の部分は、メールトラッキング CNAME `[EmailTrackingCNAME]` です。これは、手順 5 で IT チームに渡す必要があります。

>[!CAUTION]
>
>電子メールとランディングページの CNAME は別にする必要があります。また、「track」や「link」といった CNAME は使用しないでください。多くの場合、スパムとしてフラグ付けされます

Marketo のトラッキングリンクを確認するには、「**管理者**」領域に移動します。

![](assets/admin.png)

「**メール**」をクリックします。

![](assets/image2015-1-6-13-3a55-3a32.png)

メール設定からトラッキングリンクをコピーします。

トラッキングリンクは、次の形式で入力します。`mkto-[a-z][4 digits].com`

![](assets/email-tracking-link-hand.jpg)

これがご自身の `[MktoTrackingLink]` です。保存します。これは、手順 5 で IT チームに渡す必要があります。

「差出人」ドメインを収集します。Marketo からのメール送信に使用するすべての「差出人」ドメイン（`[Sender]@[FromDomain].com` のように）のリストを作成します。ほとんどの場合、1 つだけです。

例、「marketo.com」、「info.marketo.com」。これらは `[FromDomain1]`、`[FromDomain2]` 等があります。保存します。これらは、手順 5 で IT チームに渡す必要があります。

リクエストを IT チームに送信するために必要な情報がすべて揃いました。

## プロトコルの設定を IT チームに依頼する {#ask-it-to-configure-protocols}

>[!NOTE]
>
>Launch Pack をご利用の場合は、この手順をスキップできます。初回コール時に、担当のコンサルタントが IT セットアップ手順書を提供します。

必要な情報をすべて収集したら、IT チームにリクエストを送信する準備が整いました。以下のテキストをテンプレートとして使用し、太字のテキストを独自の情報に置き換えることができます。

[この記事へのリンクを含める](/help/marketo/getting-started/setup-steps/configure-protocols-for-marketo.md)。

メールにこのテキストを貼り付け、太字のプレースホルダーを置き換えます。

>[!NOTE]
>
>上記の手順 3 と 4 を参照して、プレースホルダーを置き換えるテキストを決定してください。`[LandingPageCNAME]` と `[EmailTrackingCNAME]` は、別のものを使用する必要があります。

`---------------------------------------------`

IT 管理者様

マーケティングチームは、コミュニケーションに Marketo プラットフォームを使用することになりました。優れたメール配信品質を確保するには、次の変更を行う必要があります。

`1)` ランディングページには、**[LandingPageCNAME]**.**[CompanyDomain]**.com の DNS エントリ（CNAME）を追加して、**[AccountString]**.mktoweb.com を指すようにしてください。

`2)` メール内のトラッキングリンクには、**[EmailTrackingCNAME]**.**[CompanyDomain]**.com の DNS エントリ（CNAME）を追加して、**[MktoTrackingLink]** を指すようにしてください。

`3)` Marketo を許可リストに加えてください。

    * メール許可リストに IP アドレスを使用する場合は、以下に示す IP アドレスを追加してください。
    199.15.212.0/22
    
    192.28.144.0/20
    
    192.28.160.0/19
    
    185.28.196.0/22
    
    130.248.172.0/24
    
    130.248.173.0/24
    
    103.237.104.0/22
    
    94.236.119.0/26

注意：ご使用の環境に合わせた IP の短縮リストを希望する場合は、Marketo サポートにお問い合わせください。

    * スパム対策システムで送信元ドメインが使用されている場合は、次のドメインを追加してください。

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)` SPF と DKIM を設定し、Marketo が署名済みメールを会社に代わって送信する権限を付与する必要があります。

`a.` SPF を設定するには、DNS エントリに次の行を追加してください。

IN  TXT **[From Domain]**:  v=spf1 mx ip4:**[Corporate IP(s)]**
<br/>include: mktomail.com ~all

DNS エントリに既に SPF レコードが存在する場合は、次のコードを追加してください。

include: mktomail.com

`[`**From Domain** をメール送信元ドメイン（例：company.com）に、**CorpIP** を会社のメールサーバーの IP アドレス（例：255.255.255.255）に置き換えます。Marketo を通じて複数のドメインからメールを送信する場合は、IT スタッフに各ドメインに対してこの行を（1 行で）追加してもらう必要があります。`]`

`b.`DKIM の場合は、設定するドメインごとに DNS リソースレコードを作成してください。署名する各ドメインのホストレコードと TXT 値を次に示します。

**`[DKIMDomain1]`**：ホストレコードが **`[HostRecord1]`** で、TXT 値が **[TXTValue1]**.です。

**`[DKIMDomain2]`**：ホストレコードが **`[HostRecord2]`** で、TXT 値が **`[TXTValue2]`** です。

`[`[こちらの手順に従って](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md)、設定した **DKIMDomain** ごとに **HostRecord** と **TXTValue** をコピーします。IT スタッフがこの手順を完了したら、必ず&#x200B;**管理者／メール／DKIM** で各ドメインを確認してください。`]`

`5)` **[FromDomain1]**、**[FromDomain2]** など、送信元ドメインに有効な MX レコードがある必要があります。確認できますか？そうでない場合は、会社のドメイン MX レコードにマッピングするように設定してください。これにより、Marketo 宛ての返信／自動応答を確実に処理できます。

これらの手順が完了したらお知らせください。Marketo で設定プロセスを完了します。

ありがとうございました。ご協力感謝します。

よろしくお願いします。

**`[Your Name]`**

`---------------------------------------------`

IT チームにメールを送信します。IT チームがこれらのタスクを完了するまでに時間がかかる場合があることを承知しています。手順 7 に進むことはできますが、Marketo の設定を完了するには、手順 6 に戻る必要があります。

## IT チームの作業完了後に、Marketo の設定を完了する {#complete-your-marketo-setup-after-it-finishes}

IT チームが作業を完了したら、次の手順に従ってランディングページとメールの CNAME を追加し、DKIM 署名を有効にします。

「**管理者**」領域に移動してランディングページ CNAME を追加します。

![](assets/admin.png)

ランディングページを選択し、設定領域の「**編集**」をクリックします。

![](assets/image2015-1-6-13-3a59-3a15.png)

ランディングページの「ドメイン名」フィールドに新しいドメイン名を入力します。これは次の形式で記述します。

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/image2015-1-6-14-3a3-3a6.png)

「フォールバックページ」フィールドに、ランディングページが利用できない場合に訪問者に表示する URL を入力します。フォールバックページがない場合は、会社のホームページを使用できます。「ホームページ」フィールドに、会社の web サイトを入力します。

![](assets/image2015-1-6-14-3a2-3a46.png)

「管理者」領域で「メール」を選択して、メール CNAME を追加します

![](assets/image2015-1-6-14-3a5-3a3.png)

下にスクロールして、「**編集**」をクリックします。

![](assets/edit-branding-domain.png)

「ドメイン」フィールドに、メールトラッキングドメインを入力します。これは次の形式で記述します。

`[EmailTrackingCNAME].[CompanyDomain].com`.「**保存**」をクリックします。

![](assets/new-branding-domain-9-1.png)

## CRM を統合する {#integrate-your-crm}

これはおそらく、設定の最もエキサイティングな手順です。CRM に保存したすべてのリードと連絡先を Marketo に取り込みます。

会社が使用している CRM に応じて、次の中から選択します。

    * [Marketo と Salesforce.com の統合](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
    * [Marketo と Microsoft Dynamics の統合](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

>[!NOTE]
>
>これらの手順を完了するには、会社の CRM 管理者の支援が必要です。

## Web サイトへのトラッキングコードの追加 {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Launch Pack をご利用の場合は、この手順をスキップできます。担当のコンサルタントが、IT セットアップ手順ドキュメントに Munchkin コード手順を提供します。

Marketo には、任意の web ページ上のユーザーアクティビティのトラッキングに使用できるカスタムトラッキング JavaScript（Munchkin と呼ばれます）が用意されています。Web サイトを Marketo に統合するには、Munchkin が必要です。次の手順に従って、[web サイトに Munchkin トラッキングコードを追加します](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)。

>[!NOTE]
>
>トラッキングコードの追加には、HTML の知識が必要です。

すべての設定手順が完了しました。さっそく Marketo を使用してみましょう。
