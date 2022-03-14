---
unique-page-id: 17727823
description: リリースノート - 19 年冬 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 19 年冬
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: ht
source-wordcount: '1109'
ht-degree: 100%

---

# リリースノート：19 年冬 {#release-notes-winter}

19 年冬リリースには、次の機能が含まれています。機能の可用性についてはお使いの Marketo のエディションをご確認ください。

各機能の詳細な記事を表示するには、タイトルリンクをクリックしてください（ある場合）。

>[!NOTE]
>
>カスタムオーディエンスの統合を活用するために、Facebook に Business Manager アカウントが必要になりました。Facebook LaunchPoint サービスは Business Manager アカウントに関連付けられている&#x200B;*必要*&#x200B;があります。さもないと、統合は **2019 年 1 月 15 日**&#x200B;以降機能しなくなります。Business Manager アカウントを設定するには、[Facebook Help](https://www.facebook.com/business/help/1710077379203657) を参照してください。

>[!NOTE]
>
>Microsoft は、すべてのオンラインユーザーに対して、Microsoft Dynamics の最新バージョンへのアップグレードを求めています。Marketo インスタンスを DynamicsOnline と統合する場合は、統合が引き続き機能するように、**2019 年 1 月 31 日**&#x200B;までに [Marketo ソリューションの最新バージョンにアップグレード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)する必要があります。

>[!NOTE]
>
>Marketo は、GoToWebinar の OAuth バージョンを 1.0 から 2.0 にアップグレードしています。OAuth 1.0 のサポートは、2019 年 1 月に廃止されます。統合が引き続き機能するようにするためには、GoToWebinar の顧客は、**2019 年 1 月 31 日**&#x200B;までに LaunchPoint（管理領域内）を介してログインを再認証する必要があります。詳細は、[コミュニティページ](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019)を参照してください。

## 主要プラットフォームの機能拡張 {#core-platform-enhancements}

**[Marketo メールのメール CC](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Marketo を通じて送信するメールは、受信者あたり 5 件までの CC アドレスを含めることができます。

**API**

* **アセット API のマルチブランディングドメインサポート**：アセットの承認と複製により、API と UI 内で同じ結果が得られます。
* **アセット API のメール CC サポート**：API を使用したメールの複製、承認、処理をおこなうユーザーは、UI 設定と同等の性能を維持します。

**[Munchkin v155（ベータ版）](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **API のみのモード**：Marketo の自動追跡に頼るのではなく、単一ページの Web アプリが Web ページへのアクセスを記録するときに明示的に呼び出すことができるようにすることで、データベースのメンバーをいつどのように追跡するかを決定できるようになりました。
* **オプトアウト管理**：オプトアウト Cookie ドメインを Munchkin トラッキング Cookie ドメインと照合することで、オプトアウトを簡単に管理できます。
* **ドメインレベルの決定者パラメーター**：2 文字のドメイン（例：[website.io](https://website.io)）は、追加の設定要件なしで Marketo で自動的に追跡します。

## Marketo Sales Engage {#marketo-sales-engage}

* **Salesforce カスタムプロファイル**：Sales Engage は、無制限のカスタムプロファイルをサポートするようになりました。

* **Salesforce カスタマイズ**：重要でないカスタムアクティビティフィールドを削除すると、CRM プラットフォームで Sales Engage をより効率的に設定できます。
* **メールサービス**：Microsoft Outlook に（Office365 または「メール接続」タブを使用してオンプレミス）接続することで、メール到達率の向上に加え、返信追跡機能、スケジュール済みメール機能の強化、および一括メール機能を利用できます。
* **新しい管理設定**：Sales Engage インスタンスを最適化するための 2 つの管理ページが追加されました。

   * _チーム管理_&#x200B;は、管理者が購読とチームを編集できるようにすることで、シームレスなアカウント設定プロセスをサポートします。
   * _Salesforce 管理設定_&#x200B;は、チームが SFDC 同期を以前よりも迅速かつ簡単に設定するのに役立ちます。

* **Windows 用 OWA プラグイン**：1 つのアドインで、すべての Windows Office365 クライアントが Sales Engage でサポートされ、Outlook でライブフィードを使用できます。新しいプラグインは、Microsoft Store で使用できます。
* **アクティビティプッシャー**：Sales Engage をコア Marketo プラットフォームに同期して、リアルタイムのマーケティングインサイトを活用します。

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Marketo Sky のリリースは、より頻繁におこなわれます。第 4 四半期後半／第 1 四半期初旬には、次の機能および機能強化がリリースされる予定です。詳細と更新については、[Sky ドキュメント](https://help.marketo.com/)を参照してください。

* **オプションのデフォルトエクスペリエンス**：Marketo ユーザーは、Marketo Sky が管理者からアクセス権を付与されている場合、ユーザーをデフォルトエクスペリエンスに設定できます。

* **マイ Marketo**：最も頻繁に訪問する領域に重要な情報、通知、リンクを提供するウィジェットを追加して、エクスペリエンスをカスタマイズします。

* **デザインスタジオリストビューと詳細ページ**：メール、ランディングページ、フォームのフィルタリング可能で検索可能なリスト表示で、組織と正確性のレベルを高めます。アセットの詳細ページには、アセットが使用しているプログラム、使用しているスニペットの数など、各アセットに関する重要な情報が表示されます。

* **グローバル検索**：プラットフォーム全体でより高速でより堅牢なグローバル検索機能が提供されます。検索クエリが、アクセス可能なすべてのワークスペースで実行され、アセット（アクティブとアーカイブの両方）、ラベル、キャンペーン、プログラムを検索できるようになりました。検索結果はオーバーレイを介して提供され、各結果にはアセットの保存場所を指定するためのファイルの場所の追跡情報が含まれます。

* **ユーザーインターフェイスの改善**：新しいアイコン、モデル、ボタン、および新しいカラーパレットを追加して、当社のブランドのリフレッシュを反映し、Marketo Sky をより印象深く機能的にします。

* **メールプログラムのユーザビリティの強化**：従来の Marketo リード管理プラットフォームと新しい Marketo Sky でのメールプログラムの機能の同等化に引き続き努めていきます。
* **Event-With-Webinar プログラム**：Event-With-Webinar プログラムが Marketo Sky で利用できるようになりました（注意：このリリースでは、GoToWebinar のみがサポートされています。その他の統合は時間の経過と共に確立されます）。

## Account-Based Marketing {#account-based-marketing}

**[ABM ペルソナベースのセグメント化とフィルタリング](/help/marketo/product-docs/target-account-management/using-personas.md)**

重点顧客内の特定のペルソナに対して ABM キャンペーンをパーソナライズします。ABM ペルソナ機能は、リードのセグメント化に基づいてデフォルトの役職を作成し、追加のペルソナセグメント化を設定できます。

## アナリティクス {#analytics}

**Bizible**

* **カスタム計算フィールド**：任意の Bizible 属性を使用して、ダッシュボードのレポートとセグメント化に使用できるカスタムフィールドを作成します。

* **SOC II タイプ II 証明書**：新しいセキュリティとプライバシーの認定は、今年初めから Type I の認定に基づいて構築されます。

## Web パーソナライズ機能 {#web-personalization}

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
