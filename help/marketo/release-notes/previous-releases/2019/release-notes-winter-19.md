---
unique-page-id: 17727823
description: リリースノート - 19 年冬 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 19 年冬
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '1050'
ht-degree: 70%

---

# リリースノート：2019年冬 {#release-notes-winter}

19 年冬リリースには、次の機能が含まれています。利用可能な機能についてはお使いの Marketo のエディションをご確認ください。

各機能の詳細な記事を表示するには、タイトルリンクをクリックしてください（ある場合）。

>[!NOTE]
>
>カスタムオーディエンス統合を活用するために、[!DNL Facebook] には Business Manager アカウントが必要になりました。 [!DNL Facebook] LaunchPoint サービス *必須* が Business Manager アカウントに関連付けられている必要があります。関連付けられていない場合 **2019 年 1 月 14 日（PT）以降、統合が機能しなくなります**。 Business Manager アカウントを設定するには、[[!DNL Facebook]  ヘルプ ](https://www.facebook.com/business/help/1710077379203657) を参照してください。

>[!NOTE]
>
>Microsoftは、すべてのオンラインのお客様に対して、[!DNL Microsoft Dynamics] の最新バージョンへのアップグレードを推奨しています。 Marketo インスタンスを [!DNL Dynamics Online] と統合している場合、統合が引き続き機能することを確認するには、[2019 年 1 月 31 日 **までに ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)Marketo ソリューションの最新バージョンにアップグレード** する必要があります。

>[!NOTE]
>
>Marketo は、GoToWebinar の OAuth バージョンを 1.0 から 2.0 にアップグレードしています。OAuth 1.0 のサポートは、2019 年 1 月に廃止されます。統合が引き続き機能するようにするためには、GoToWebinar の顧客は、**2019 年 1 月 31 日**&#x200B;までに LaunchPoint（管理領域内）を介してログインを再認証する必要があります。詳細は、[コミュニティページ](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019)を参照してください。

## 主要プラットフォームの機能拡張 {#core-platform-enhancements}

**[Marketo メールのメール CC](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Marketo を通じて送信するメールは、受信者あたり 5 件までの CC アドレスを含めることができます。

**API**

* **アセット API のマルチブランディングドメインサポート**：アセットの承認と複製により、API と UI 内で同じ結果が得られます。
* **アセット API のメール CC サポート**：API を使用したメールの複製、承認、処理をおこなうユーザーは、UI 設定と同等の性能を維持します。

**[[!DNL Munchkin] v155 （Beta） ](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **API のみのモード**：Marketo の自動追跡に頼るのではなく、単一ページの Web アプリが Web ページへのアクセスを記録するときに明示的に呼び出すことができるようにすることで、データベースのメンバーをいつどのように追跡するかを決定できるようになりました。
* **オプトアウト管理**：オプトアウト cookie ドメインを [!DNL Munchkin] トラッキング cookie ドメインと照合することで、オプトアウトを簡単に管理できます。
* **ドメインレベルの決定者パラメーター**：2 文字のドメイン（例：[website.io](https://website.io)）は、追加の設定要件なしで Marketo で自動的に追跡します。

## Marketo Sales Engage {#marketo-sales-engage}

* **[!DNL Salesforce]カスタムプロファイル**: Sales Engage は、無制限のカスタムプロファイルをサポートするようになりました。

* **[!DNL Salesforce]のカスタマイズ**：重要でないカスタムアクティビティフィールドを削除することで、ユーザーは CRM プラットフォームで Sales Engage をより効率的に設定できます。
* **メールサービス**:[!DNL Microsoft Outlook] に接続することで（Office365 を使用するか「メール接続」タブからオンプレミスで）、配信品質の向上に加え、返信トラッキング、スケジュールされたメール機能、一括メール機能が実現します。
* **新しい管理設定**：Sales Engage インスタンスを最適化するための 2 つの管理ページが追加されました。

   * _チーム管理_&#x200B;は、管理者が購読とチームを編集できるようにすることで、シームレスなアカウント設定プロセスをサポートします。
   * _Salesforce 管理設定_&#x200B;は、チームが SFDC 同期を以前よりも迅速かつ簡単に設定するのに役立ちます。

* **OWA Plugin for[!DNL Windows]**: 1 つのアドインで、すべての [!DNL Windows Office365] クライアントが Sales Engage でサポートされ、Outlook で Live Feed を使用できるようになります。 新しいプラグインは、Microsoft Store で使用できます。
* **アクティビティプッシャー**：Sales Engage をコア Marketo プラットフォームに同期して、リアルタイムのマーケティングインサイトを活用します。

## [!DNL Marketo Sky] {#marketo-sky}

>[!NOTE]
>
>[!DNL Marketo Sky] リリースは、より頻繁に行われます。 第 4 四半期後半／第 1 四半期初旬には、次の機能および機能強化がリリースされる予定です。詳細と更新については、[Sky ドキュメント](https://help.marketo.com/)を参照してください。

* **オプションのデフォルトエクスペリエンス**:Marketo ユーザーは、管理者からアクセス権を付与されている場合、[!DNL Marketo Sky] をデフォルトエクスペリエンスとして設定できます。

* **マイ Marketo**：最も頻繁に訪問する領域に重要な情報、通知、リンクを提供するウィジェットを追加して、エクスペリエンスをカスタマイズします。

* **デザインスタジオリストビューと詳細ページ**：メール、ランディングページ、フォームのフィルタリング可能で検索可能なリスト表示で、組織と正確性のレベルを高めます。アセットの詳細ページには、アセットが使用しているプログラム、使用しているスニペットの数など、各アセットに関する重要な情報が表示されます。

* **グローバル検索**：プラットフォーム全体でより高速でより堅牢なグローバル検索機能が提供されます。検索クエリが、アクセス可能なすべてのワークスペースで実行され、アセット（アクティブとアーカイブの両方）、ラベル、キャンペーン、プログラムを検索できるようになりました。検索結果はオーバーレイを介して提供され、各結果にはアセットの保存場所を指定するためのファイルの場所の追跡情報が含まれます。

* **改善されたユーザーインターフェイス**：新しいアイコン、モデル、ボタンに加えて、ブランドの刷新を反映し、より魅力的で機能的 [!DNL Marketo Sky] 新しいカラーパレットが追加されました。

* **メールプログラムのユーザビリティの強化**：従来のMarketo Lead Management プラットフォームと新しい [!DNL Marketo Sky] エクスペリエンスの間で、メールプログラム機能のパリティに引き続き移行します。
* **イベントとウェビナープログラム**：イベントとウェビナープログラムが [!DNL Marketo Sky] で利用できるようになりました（メモ：このリリースでは GoToWebinar のみがサポートされ、今後、さらなる統合が行われる予定です）。

## Account-Based Marketing {#account-based-marketing}

**[ABM ペルソナベースのセグメント化とフィルタリング](/help/marketo/product-docs/target-account-management/using-personas.md)**

重点顧客内の特定のペルソナに対して ABM キャンペーンをパーソナライズします。ABM ペルソナ機能は、リードのセグメント化に基づいてデフォルトの役職を作成し、追加のペルソナセグメント化を設定できます。

## アナリティクス {#analytics}

**[!DNL Bizible]**

* **カスタム計算フィールド**：任意の [!DNL Bizible] 属性を使用して、ダッシュボードレポートおよびセグメント化に使用できるカスタムフィールドを作成します。

* **SOC II タイプ II 証明書**：新しいセキュリティとプライバシーの認定は、今年初めから Type I の認定に基づいて構築されます。

## [!DNL Web Personalization] {#web-personalization}

**[アカウント設定にサブドメインを追加](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

ドメインとサブドメインをより効率的に管理するために、RTP アカウント設定にサブドメインを追加できるようになりました。

## Marketo モバイルエンゲージメント（MME） {#marketo-mobile-engagement-mme}

**Android 向けのソフトウェア開発キット（SDK）を更新しました**

Android 向け SDK を、より柔軟性と新しいエンジニアリング機能を含む、より新しく、安定した、拡張性の高いフレームワークに更新しました。この新しい SDK では、Android アプリデベロッパーが Google の [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/)（FCM）を直接使用できるようになりました。

* [デベロッパー向けの手順](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [デベロッパー向け FAQ](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>アプリデベロッパーは 2019 年 3 月 31 日より前に新しいバージョンに更新する&#x200B;**必要があります**。2019 年 3 月 31 日までに SDK を更新しない場合、この日以降にアプリをダウンロードした新しいユーザーは、最新バージョンの SDK に更新するまでプッシュ通知を受け取れません。SDK の更新では、現在のモバイルアプリユーザーが新しいバージョンのアプリを再ダウンロードする必要はありません。

## その他のアップデート {#additional-updates}

**拡張可能なウェビナープラットフォーム**

製品リリースに加えて、パートナーチームは、ウェビナープロバイダーが Marketo との独自の統合を構築および維持できる新しいフレームワークに取り組み、ソリューションの更新と強化をより柔軟に提供し、マーケターが選択した統合を最大限に活用できるようにします。

当社は、プロバイダーとの間で、ケースバイケースで新しいプラットフォームを展開する予定です。詳しくは、[プログラムの詳細](https://www.marketo.com/why-marketo/partners/technology/)または、Marketo の連絡先に問い合わせてください。
