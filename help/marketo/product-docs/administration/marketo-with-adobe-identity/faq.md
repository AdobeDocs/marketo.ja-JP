---
description: Adobe Identity Management に関するよくある質問 - Marketo ドキュメント - 製品ドキュメント
title: Adobe Identity Management に関するよくある質問
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1645'
ht-degree: 100%

---

# Adobe Identity Management に関するよくある質問 {#adobe-identity-management-faq}

**Adobe ID とは何ですか？**

Adobe Identity Management システムは、3 つのコンポーネントで構成されています。

* [!DNL Adobe Identity Service]：フェデレーションとランタイムシングルサインオン（SSO）を含む、エンドユーザーの認証と検証を処理します。

* Adobe Admin Console：Admin Console では、組織全体にわたるアドビの使用権限を一元的に管理できます。 ユーザー管理、クラウドサービス、デスクトップライセンスの使用権限、フェデレーション設定を処理し、データ消失防止のセキュリティ機能を提供します。

* Adobe User Management API（UMAPI）：組織が Adobe Admin Console で API レベルでエンタープライズユーザーとエンタイトルメントを管理できるようにします。

**既存の Marketo Engage サブスクリプションは、いつ IMS と統合されますか？**

既存の Marketo Engage サブスクリプションは現在、更新、再契約イベント、追加などの販売イベントの際に Adobe IMS に移行されています。 2024年10月から、販売イベント以外での移行がサポートされています。

**移行後、Marketo Engage URL は変わりませんか？**

いいえ、できません。 移行後に URL は `https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/` の形式で表示されます（XXX は Munchkin ID を表し、@tenantID は Adobe 組織のもの）。

**URL の変更に備えて必要なことはありますか？**

はい。 移行後、Marketo Engage は experience.adobe.com から Adobe Experience Cloud に提供されるようになります。 Marketo Engage へのアクセスが中断されないようにするには、IT チームと協力して、[この記事の上部](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"}に記載されているすべての Adobe ドメインを許可リストに登録する必要があります。

engagement-xx.marketo.com ドメイン上の Marketo Engage アセットへの以前のリンクとブックマークは引き続き機能する&#x200B;_予定_&#x200B;です。 ただし、まず、移動先の URL の Marketo Engage インスタンスにログインする必要があります。 例えば、Munchkin ID 123-ABC-456 のインスタンスのスマートキャンペーンのブックマークに移動するには、まず Munchkin ID 123-ABC-456 で Marketo Engage インスタンスにログインする必要があります。

予定はありませんが、今後の開発作業でこのリダイレクト機能が機能しなくなる可能性があります。予期しない中断を避けるために、できるだけ早い時期にブックマークを更新することをお勧めします。

**SSO はサポートされていますか？**

はい。 Adobe IMS との統合では、ユニバーサル ID ユーザと SSO がサポートされています。 SSO は Adobe IMS によって駆動され、Adobe Admin Console で組織レベルで設定されます。 ただし、Marketo Engage IdP 開始サポートとアドビの SP 開始サポートには違いがあります（[詳しくは、こちらを参照してください](https://helpx.adobe.com/jp/enterprise/using/set-up-identity.html){target="_blank"}）。Admin Console に移行した後の SSO の違いに関してサポートが必要な場合は、[アドビカスタマーケア](https://helpx.adobe.com/jp/contact.html){target="_blank"}にお問い合わせください。

**製品管理者とアドビ管理者の違いは何ですか。**

* アドビ製品管理者は、Marketo プラットフォームの新しいロールです。
* アドビ製品管理者のロールは、Adobe Admin Console で製品管理者として追加されたユーザーに付与されます。
* アドビ製品管理者のロールは読み取り専用で、Marketo Engage から編集または削除することはできません。
* アドビ製品管理者は、標準の Marketo 管理者と同じ権限を持っています。
* Marketo Engage 管理者のロールは、引き続き管理者で、Marketo Engage でユーザーに付与されます。
* Marketo のデフォルトの管理者ロールを持つユーザのみが、Admin Console の Marketo 製品管理者として割り当てられます。

**User Management API クライアントのサポートに何か変更はありますか？**

はい。 Adobe IMS に転送されたユーザは、既存の Marketo User Management API の一部を利用できます。ユーザの招待、更新、削除のアクションには、Adobe [IMS API](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} を使用する必要があります。ロール管理の場合は、Marketo User Management API が引き続き適用されます。これ以外には、Marketo REST API クライアントのサポートに対する変更はありません。

**IMS と統合された場合、サポートの問い合わせ先はどこですか？**

* ユーザ移行前：[マーケティングネーションコミュニティ](https://nation.marketo.com/t5/support/ct-p/Support)またはメール（`customercare@marketo.com`）でサポートケースを申請します。

* ユーザ移行後：[マーケティングネーションコミュニティ](https://nation.marketo.com/t5/support/ct-p/Support)またはメール（`customercare@marketo.com`）でサポートケースを申請します。

* サポート終了後の移行完了：製品サポート管理者は、Experience League サポートポータルからケースを申請できます。

Ultimate Success を利用している場合は、Admin Console Migration White Glove Service にアクセスできます。 サポートが必要な場合は、アドビのアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

**Adobe ID を使用して他のアドビアプリケーションにアクセスする場合、それを使用して Marketo にアクセスできますか？**

他のアドビ製品がある場合でも、サブスクリプションが IMS に移行されるまで、Adobe ID を使用して Marketo にアクセスできません。

**Marketo のユーザーのロール（ワークスペース内）は Adobe Admin Console で管理されますか？**

いいえ、できません。 （ワークスペース内の）ユーザーのロール管理は、Marketo Engage で完了します。

**私は IMS 統合サブスクリプションの Marketo 管理者ですが、Admin Console へのアクセス権がありません。 アクセス権を取得する方法を教えてください。**

組織の Admin Console にアクセスできるアドビシステムまたは製品管理者なら誰でもアクセスを許可できます。組織内で誰がコンソールの管理者権限を持っているかが不明な場合は、[アドビカスタマーケア](https://helpx.adobe.com/jp/contact.html){target="_blank"}にお問い合わせください。

**管理者はどのように Marketo [!DNL Sales Connect] にユーザーを追加しますか？**

[!DNL Sales Connect] の Admin Console には製品カードがありますが、Admin Console を使用してユーザーを追加／管理することはできません。 次のリンクを使用すると、Marketo [!DNL Sales Connect]を経由して管理者はユーザーを管理できます：[https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}。

**Adobe Admin Console の詳細はどこで確認できますか？**

[Https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/jp/enterprise/admin-guide.html){target="_blank"} にアクセスしてください。

**マイアカウントのユーザアカウントに変更を加えるためには、Marketo の管理者セクションにアクセスするのでしょうか？**

いいえ、[account.adobe.com](https://account.adobe.com){target="_blank"}.にアクセスする必要があります。

**Marketo Universal ID との連携方法を教えてください。**

Adobe ID に転送されたユーザーは、製品の購読切り替えボタンを使用して、IMS 対応のすべての購読にシームレスにアクセスできます。

**SSO はサポートされていますか？**

はい。 Marketo と Adobe IMS の統合では、ユニバーサル ID ユーザーと SSO がサポートされています。 SSO は Adobe IMS によって駆動され、Adobe Admin Console で組織レベルで設定されます。[詳細はこちら](https://helpx.adobe.com/jp/enterprise/using/set-up-identity.html){target="_blank"}を参照してください。

**既に Adobe ID にオンボードされているので、SSO を実装したいと考えています。 どうすればいいですか？**

シングルサインオンの実装を希望しており、アドビ組織に SSO が実装されていない状態でサブスクリプションが Adobe ID に既にオンボードされている場合は、[Marketo サポート](https://nation.marketo.com/){target="_blank"}にチケットを送信し、「Admin Console での Marketo、SSO の実装」というトピックを指定してください。

**デバイス認証はどのように機能しますか？**

Adobe IMS は、現在、Marketo のデバイス認証機能などをサポートしていません。

**「ユーザーを招待ダイアログでログイン」機能を使用して、ユーザーのログインをメールから一意にすることは可能ですか？**

いいえ、できません。 サブスクリプションが IMS 有効の場合、ユーザー招待ワークフローはアクティブでなくなったので、この機能は無効になりました。 Adobe ID では、ユーザーの ID としてメールを使用します。

**Adobe IMS の場合、Adobe ID、Enterprise ID、Federated ID を使用できますか？**

はい、サポートする ID のタイプを決定するのは組織です。詳しくは、[ID の概要](https://helpx.adobe.com/jp/enterprise/using/identity.html)と [ID の設定](https://helpx.adobe.com/jp/enterprise/using/set-up-identity.html){target="_blank"}を確認してください。

**Adobe Admin Console でサポートされている製品カードは何ですか。**

サポートされる製品カードは、Marketo Engage、Marketo Measure、Marketo Dynamic Chat、Marketo Sales Connect、Marketo Sales Insight Actions です。

**Adobe ID に移行する際に、ユーザのログイン情報がメールアドレスと一致しない場合はどうすればいいですか？**

メールアドレスとは異なるログイン情報を使用している現在の Marketo Engage ユーザは、Adobe ID に移行すると、その資格情報ではログインできなくなります。 Adobe ID では、常にユーザのメールアドレスを使用して認証します。 Adobe ID のメールアドレスは [account.adobe.com](https://account.adobe.com){target="_blank"} で更新できます。

**サブスクリプションで IP 制限設定を使用している場合、Adobe ID の移行後はどうなりますか？**

サブスクリプションを Adobe ID にオンボードした場合、IP 制限設定は Adobe Admin Console に移行されません。 Marketo の IP 制限設定には、特定の IP アドレスからのアクセスのみを許可することや、特定の IP アドレスからのアクセスをブロックすることが含まれます。 現時点では、Adobe Identity Management システムは IP 制限機能をサポートしていません。

2025年半ばに、Adobe Identity Management システムは特定の IP アドレスのみを許可する機能をリリースし、現在この機能を使用している Marketo ユーザのトランジションをサポートします。現在この機能を使用しているユーザは、機能がリリースされるまでユーザの移行は行われません。 機能が提供されると、移行がスケジュールされていることがユーザに通知されます。 この機能について詳しくは、機能が利用可能になった時点で提供されます。

現在、特定のアドレスへのアクセスをブロックする IP 制限を使用しているユーザは、Adobe Identity Management システムでサポートされていないので、Adobe ID に移行すると、この機能を使用できなくなります。

**「シングルサインオンをバイパス」オプションがあるロールを持つユーザがいる場合、Adobe ID の移行後はどうなりますか？**

Adobe Admin Console には、デフォルトの Business ID ディレクトリが付属しています。アドビ組織内の Federated ID ディレクトリで要求されたドメイン外のユーザーは、Adobe ID の ID タイプでこのディレクトリに割り当てられます。これらのユーザーは、シングルサインオン（SSO）を経由せずに Marketo Engage にアクセスできます。ライセンスの所有権は個人ではなく会社に残ります。

**複数のサブスクリプションを持っていますが、すべてのサブスクリプションでシングルサインオンが有効になっているわけではありません。 Adobe ID の移行後はどうなりますか？**

サブスクリプションが Adobe ID にオンボードされると、シングルサインオン（SSO）がアドビ組織レベルで設定されます。 つまり、SSO はアドビ組織内のすべての製品インスタンスに適用されます。SSO を設定すると、そのアドビ組織内のすべての Marketo インスタンスに適用されます。 以前、Marketo はこの設定をインスタンスレベルでサポートしていました。 これは、Adobe Identity Management システムではサポートされていません。

**Adobe ID の移行後、Marketo Engage で現在使用している CNAME、SPF、DKIM に変更は必要ですか？**

いいえ、これらの設定には影響はありません。

**セッションがタイムアウトするのを防ぐにはどうすればよいですか？**

[詳細設定](https://helpx.adobe.com/jp/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"}では、目的の最長セッション有効期間をカスタマイズできます（システム管理者の権限が必要です）。この設定は、製品の移行後、ユーザの移行前に確立することをお勧めします。

**次に、Experience Cloud に移動して Marketo Engage にアクセスする必要があります。 このフローを効率化する方法はありますか？**

はい。 Marketo Engage インスタンスのエントリページで「**起動**」ボタンをクリックした後に起動するリンクのブラウザーブックマークを作成すると、そのページの進行を回避できます。

![](assets/faq-1.png)
