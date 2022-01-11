---
description: 最新のリリースノート — Marketoドキュメント — 製品ドキュメント
title: 最新のリリースノート
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: f00d43080136dd986a6d81d6bc8102cdaf788b4c
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 7%

---

# リリースノート：2022年1月 {#release-notes-jan-22}

2022 年 1 月リリースには、次の機能が含まれています。 AdobeMarketo Engageエディションの機能の可用性を確認してください。

>[!AVAILABILITY]
>
>星形 (![星](assets/yellow-star.png)) は有料のアドオンです。 詳細は Marketo Engage 担当営業にお問い合わせください。

**_四半期リリース_**

以下の機能は **2022 年 1 月 21 日**（PT）にリリースされます。

## 次世代のエクスペリエンス {#next-generation-experience}

* **次世代のエクスペリエンスの画面の更新**:次世代のエクスペリエンスで、トグルスイッチを介してアクセス可能な、最新のデザインと操作性の強化を提供する、新しい画面を追加で提供しています。

   * デザインスタジオでのランディングページアセットの詳細
   * マーケティングアクティビティのランディングページアセットの詳細

## Microsoft Dynamics 統合 {#microsoft-dynamics-integration}

* **一般に利用可能な Multiselect Optionset フィールドタイプの同期**:Microsoft Dynamics の複数選択オプションセットフィールドタイプを同期して、スマートリストとスマートキャンペーンで活用し、より詳細なオーディエンスターゲティングを実現します。 以下に例を示します。トピック/関心のある製品、好みのコミュニケーションモードなど。 この新しい同期は、Microsoft Dynamics バージョン 9.X （Dynamics 365 Online を含む）で使用できます。

* **Microsoft Dynamics 365 Online のサーバー間認証**:セキュリティを強化するため、Microsoft Dynamics 365 Online への非インタラクティブアクセス用に、Azure Active Directory のMarketo Engage同期ユーザーの認証の追加モードとして、サーバー間 (S2S) をサポートするようになりました。 これにより、すべての認証とサインオンが OAuth（クライアント ID とクライアント秘密鍵のみ）に基づくので、多要素認証を使用できます。

>[!NOTE]
>
>S2S モードは、追加のライセンスの使用を保存する Licensed User ではなく、Application User に基づいています。

## 管理 {#administration}

* **フォーム検証ルール**:問題のある、または望ましくない E メールドメインがMarketo Engage・フォームを送信するのを防ぐ機能を備え、データベースの正常性を維持します。 グローバルフォーム検証ルールパネルを使用すると、管理者はブロックリスト、フォームをブロックする自由消費者ドメインの事前定義済みリストを定義するか、有効にすることができます。

* **ランディングページヘッダーのセキュリティ**:管理者は、ランディングページドメインで Strict Transport Security ヘッダーと X-Frame Options ヘッダーを管理して、強力なセキュリティ要件を強化できます。

**_四半期を通した段階的リリース_**

以下の機能はリリース後約 1 ～ 2 か月の間に段階的にリリースされます。

## AEPMarketo Engage宛先コネクタ — 新規リードを作成 {#aep-marketo-engage-destination-connector}

Adobe Experience Platform(AEP) も使用するMarketo Engageのお客様は、AEP の宛先コネクタを介して新しい人物レコードを AEP からMarketo Engageにプッシュできるので、データベースを最大化できます。 AEP からMarketo Engageにオーディエンスセグメントを送信する際、Marketo Engageデータベースにまだ存在しないセグメント内のユーザーが自動的に追加されます。

## Sales Insight {#sales-insight}

![（星印）](assets/yellow-star.png)

**Salesforce CRM 用 Sales Insight**

* **最優先の新しいタイプ列**:販売者は、「タイプ」というラベルの付いた新しい列を使用して、「最優先」ページのリードと連絡先を区別し、より迅速にインサイトを得ることができます。

* **Salesforce Platform API 更新**:Salesforce が Salesforce Platform API バージョン 21.0 ～ 30.0 を廃止したのに対応して、Sales Insight パッケージが最新の API で更新されました。

* **更新されたブランディング**:すべての Sales Insight ページは、Adobeのブランディングに合わせて更新されています。

**Microsoft Dynamics 向け Sales Insight**

* **更新されたアカウントのレイアウト**:販売者は、次のようなトップアクティビティを総合的に把握できます。アカウント内のすべての連絡先に関するメールアクティビティ、Web アクティビティ、注目のアクティビティ、スコア変更。

## Sales Connect {#sales-connect}

![（星印）](assets/yellow-star.png)

* **通話の結果と理由**:完全にカスタマイズ可能な新しい通話結果と通話理由オプションを使用して、セールスチームの発信活動をより詳細に把握し、追跡します。 これらの新しいフィールドに加えて、販売者が通話を行う間に、通話理由と結果の選択を強制する新しいガバナンス、通話理由と結果を有効または無効にする新しい通話理由と通話結果 Salesforce アクティビティカスタムフィールドが導入されました。 [こちら](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812)をクリックすると、詳細が表示されます。

* **Salesforce アクティビティ詳細のカスタマイズ**:セールス活動がセールスコネクトから Salesforce に記録される際に、Salesforce タスク件名フィールドに追加される情報をカスタマイズすることで、Salesforce でより多くのセールス活動とタスクデータを取り込みます。 [こちら](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819)をクリックすると、詳細が表示されます。

## お知らせ {#announcements}

* **Marketo Sky日没**:3 月 11 日には、Marketo Skyは利用できなくなります。これは、リソースが次世代のユーザーエクスペリエンスを提供することに注力しているためです。 今日、Marketo Sky専用の機能へのアクセスを維持するため、3 月には、アセットの有効期限とスマートキャンペーンの優先順位の上書きがメインストリームエクスペリエンスに取り入れられます。

* **フォームエンドポイントの廃止**:leadCapture/save2 エンドポイントに対する、サポートされていないプログラム形式の POST は、Marketo Engageフォームによって拒否されます。 [こちら](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631)をクリックすると、詳細が表示されます。

* **メールの検証**:このリリース以降、Marketo Engage購読では、「非 API のみ」のユーザーが電子メールアドレスを確認するようになります。 ディレクトリサービスの認証済みユーザーは、電子メールの検証でサブスクリプションが有効になっている場合、自動的に電子メールを検証します。 「ユーザーを招待ダイアログでログイン」機能を使用しているユーザーや、購読内の複数のユーザーに関連付けられた単一の E メールを持つ購読者のメール検証は、3 月に廃止される機能と一致して延期されます。

* **ユーザーを招待ダイアログにログイン**:3 月には、既存のオプション機能「ユーザーを招待ダイアログでログイン」は廃止されます。 「Login in Invite User Dialog」機能は、今後のAdobeIdentity Management System Integration に必要なユニバーサル ID 機能によって上書きされ、2021 年 8 月にすべてのサブスクリプションで有効になりました。 廃止の結果、Marketo Engageは、サブスクリプション内の E メールアドレスごとに関連付けられるユーザーを 1 つだけ強制します。

**Marketo Engageドメイン — Sales Insight 設定**:SSL 証明書がプロビジョニングされていないMarketo Engageドメインおよびhttps://の場合、呼び出しは SSL ハンドシェイクエラーで失敗します。 したがって、これらのドメインは廃止される予定です。 その結果、これらのドメインを指す古い設定を持つ Sales Insight ユーザーは、リード、連絡先、アカウント、商談パネル、またはMarketoグローバルページでシステムコールアウトエラーが発生する可能性があります。 お勧めの [Marketo Engage設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) Salesforce で、このエラーが発生した場合。 ドキュメントの「Marketo Sales Insight 設定」セクションでハイライト表示されたMarketo Engage資格情報のみを更新する必要があります。

**_製品リリースウェビナー_**

2022 年 1 月 27 日 (PT) 午前 9 時/午後 12 時 (ET) にご参加ください。 [ライブウェビナー](https://engage.marketo.com/2022_January_Release_Webinar_RegistrationPage.html) アドビの製品チームが主催し、最新の製品イノベーションの使用方法を学ぶことができます。
