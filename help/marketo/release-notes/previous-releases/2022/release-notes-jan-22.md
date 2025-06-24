---
description: リリースノート - 2022年1月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2022年1月
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 60%

---

# リリースノート：2022年1月 {#release-notes-jan-22}

2022年1月リリースには、次の機能が含まれています。機能の可用性についてはお使いの Marketo Engage のエディションをご確認ください。

>[!AVAILABILITY]
>
>星（![星](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

**_四半期リリース_**

以下の機能のリリースは、**2022年1月21日**&#x200B;に始まり、（特に指定のない限り）次の週から各機能が段階的にロールアウトされます。

## 次世代エクスペリエンス {#modern-ux}

* **次世代エクスペリエンスのための画面の更新**：次世代のエクスペリエンスで、トグルスイッチを介してアクセス可能な、最新のデザインと操作性の強化を備えた新しい画面を追加しました。

   * [!UICONTROL Design Studio] のランディングページアセットの詳細
   * [!UICONTROL  マーケティングアクティビティ ] のランディングページアセットの詳細

## [!DNL Microsoft Dynamics] 統合 {#microsoft-dynamics-integration}

* **一般入手可能な複数選択オプションセットフィールドタイプの同期**：複数選択オプションセットフィールドタイプを [!DNL Microsoft Dynamics] から同期して、スマートリストやスマートキャンペーンで活用し、より詳細なオーディエンスターゲット設定を行います。 例は、トピック／関心のある製品、優先するコミュニケーションモードなどです。この新しい同期は、[!DNL Microsoft Dynamics] バージョン 9.X （Dynamics 365 Online を含む）で使用できます。

* **[!DNL Microsoft Dynamics 365 Online]** のサーバー間の認証：セキュリティを強化するために、Azure Active Directory 上のMarketo Engage sync ユーザーの認証モードとして、[!DNL Microsoft Dynamics 365 Online] への非インタラクティブアクセス用にサーバー間（S2S）をサポートするようになりました。 すべての認証とサインオンが OAuth（クライアント ID とクライアント秘密鍵のみ）に基づくため、多要素認証を使用できます。

>[!NOTE]
>
>S2S モードは、追加のライセンスの使用を保存する Licensed User ではなく、Application User に基づいています。

## 管理 {#administration}

* **[フォーム検証ルール](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**：問題のある、または望ましくないメールドメインが Marketo Engage フォームを送信するのを防ぐ機能を備え、データベースの正常性を維持します。グローバルフォーム検証ルールパネルを使用すると、管理者はブロックリスト、フォームをブロックする自由消費者ドメインの事前定義済みリストを定義するか、有効にすることができます。

* **[ランディングページヘッダーのセキュリティ](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**：管理者は、ランディングページドメインで Strict Transport Security ヘッダーと X-Frame Options ヘッダーを管理して、強力なセキュリティ要件を実施できます。

**_四半期を通した段階的リリース_**

以下の機能はリリース後約 1～2 か月の間に段階的にリリースされます。

## AEP Marketo Engage 宛先コネクタ - 新規リードを作成 {#aep-marketo-engage-destination-connector}

Adobe Experience Platform（AEP）も使用している Marketo Engage の顧客は、AEP の宛先コネクタを介して新しいリードレコードを AEP から Marketo Engage にプッシュしてデータベースを最大化できます。オーディエンスセグメントを AEP から Marketo Engage に送信する際、セグメント内のユーザのうち、Marketo Engage データベースにまだ存在しないユーザは[自動的に追加できます](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md)。

## [!DNL Sales Insight] {#sales-insight}

![（星印）](assets/yellow-star.png)

[!DNL Salesforce] CRM の **[!DNL Sales Insight]**

* **ベストベット [!UICONTROL  の新しいタイプ列]**：セラーは、「タイプ」というラベルの付いた新しい列を使用して、[!UICONTROL  ベストベット ] ページのリードと連絡先を区別することで、より迅速にインサイトを得ることができます。

* **[!DNL Salesforce]Platform API アップデート**:[!DNL Salesforce] Platform API バージョン 21.0[!DNL Salesforce]30.0 の廃止に対応して、[!DNL Sales Insight] パッケージが最新の API でアップデートされました。

* **ブランディングの更新**：すべての [!DNL Sales Insight] ページが、Adobeのブランディングに合わせて更新されています。

**[!DNL Sales Insight]for[!DNL Microsoft Dynamics]**

* **更新されたアカウントのレイアウト**：販売者は、アカウント内のすべての取引先責任者に関するメールアクティビティ、web アクティビティ、注目のアクティビティ、スコア変更のようなトップアクティビティを総合的に把握できます。

## [!DNL Sales Connect] {#sales-connect}

![（星印）](assets/yellow-star.png)

* **通話の結果と理由**：完全にカスタマイズ可能な新しい通話結果と通話理由オプションを使用して、セールスチームの発信アクティビティをより詳細に把握し、追跡します。これらの新しいフィールドに加えて、セラーが通話を行っている間に通話理由と結果の選択を適用する新しいガバナンス、通話理由と結果を有効または無効にする新しいガバナンス、[!DNL Salesforce] にデータを記録する新しい通話理由と通話結果 [!DNL Salesforce] アクティビティのカスタムフィールドが導入されています。 [こちら](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812)をクリックすると、詳細が表示されます。

* **[!DNL Salesforce]Activity Detail Customization**：営業アクティビティが [!DNL Sales Connect] から [!DNL Salesforce] にログ記録されたときに [!DNL Salesforce] のタスクの件名フィールドに追加される情報をカスタマイズして、さらに多くの営業アクティビティとタスクデータを [!DNL Salesforce] に取り込みます。 [こちら](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819)をクリックすると、詳細が表示されます。

## お知らせ {#announcements}

* **Marketo Sky の廃止**：Marketo Sky は 3月に利用できなくなります。これは、当社が次世代ユーザエクスペリエンスの提供にリソースを注力しているためです。現在 Marketo Sky 専用の機能へのアクセスを維持するため、3 月には、アセットの有効期限とスマートキャンペーンの優先順位の上書きがメインストリームエクスペリエンスに取り入れられます。[こちら](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33)をクリックすると、詳細が表示されます。

* **フォームエンドポイントの廃止**：leadCapture/save2 エンドポイントに対する、サポートされていないプログラム形式の POST は、Marketo Engage フォームによって拒否されます。[こちら](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631)をクリックすると、詳細が表示されます。

* **ユーザを招待ダイアログにログイン**：3月には、既存のオプション機能「ユーザを招待ダイアログでログイン」は廃止されます。[!UICONTROL  ユーザーを招待ダイアログでログイン ]」機能は、今後のAdobe Identity Management システム統合に必要なユニバーサル ID 機能によって上書きされます。この機能は 2021 年 8 月にすべてのサブスクリプションで有効になりました。 廃止の結果、Marketo Engage の購読では、メールアドレスごとにユーザを 1 名だけ関連付けられるようになります。

**Marketo Engage ドメイン - [!DNL Sales Insight] Configuration**:SSL 証明書がプロビジョニングされていないMarketo Engage ドメインおよびhttps://の場合、呼び出しは失敗し、SSL ハンドシェイクエラーが発生します。 したがって、これらのドメインは廃止される予定です。その結果、これらのドメインのいずれかを指す古い設定を持つ [!DNL Sales Insight] ユーザーが、リード、連絡先、アカウント、商談パネル、Marketo グローバルページでシステムコールアウトエラーに遭遇する場合があります。 このエラーが発生した場合は、[!DNL Salesforce] で [Marketo Engage設定 ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) を更新することをお勧めします。 更新する必要があるのは、ドキュメントの「[!DNL Marketo Sales Insight] Config」セクションでハイライト表示されているMarketo Engage資格情報のみです。

**_製品リリースウェビナー_**

[2022年1月の Marketo Engage リリースウェビナー](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
