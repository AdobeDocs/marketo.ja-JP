---
description: リリースノート - 2021 年 8 月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2021 年 8 月
exl-id: 4aec4e0b-520e-4786-a110-8e68f1bf9950
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 71%

---

# リリースノート：2021 年 8 月 {#release-notes-aug-21}

2021 年 8 月リリースには、以下の機能が含まれています。機能の可用性についてはお使いの Marketo Engage のエディションをご確認ください。

>[!AVAILABILITY]
>
>星印（![](assets/yellow-star.png)）がついている機能は有償オプションになります。詳しくは、Adobe Marketo Engage 担当営業にお問い合わせください。

**_四半期リリース_**

以下の機能は **2021 年 8 月 20 日**（PT）にリリースされます。

## エクスペリエンスの自動化 {#experience-automation}

* **Marketo EngageID を使用した Adobe ユーザー認証**：近日中に、Enterprise パッケージを持つ新しい Marketo Engage ユーザーは、Adobe ID のユーザー資格情報を使用してオンボーディングされます。統合 ID システムへの現在のユーザーの移行は、2022 年半ばまで行われず、追加の通知が行われるまでは、何の操作も必要ありません。Adobe ID のユーザー認証を使用すると、IT／セキュリティ管理者は、他の Marketo Engage ソリューションと共に複数の Experience Cloud 製品インスタンスを管理し、共通のコンソールを通じて SSO を設定できます。管理者は、ユーザーグループとユーザーの使用権限を 1 か所で簡単に管理できます。

* **実行可能なキャンペーンのネスト**：実行可能なキャンペーンで、他の実行可能なキャンペーンを呼び出し、最大 3 レベルの深さまでネストできるようになりました。これにより、共通の運用フローをさらに統合し、スマートキャンペーン管理を改善できます。

* **リード詳細ページの単一フローアクション**（9 月 9 日まで）：データベースのグリッド表示に切り替えずに、フローアクションメニューを使用して、個人の担当者に対してメールの送信、担当者所有者の変更、その他のスマートキャンペーンアクションを実行できます。

* **[カスタムアクティビティのエクスポート](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)**：メタデータの書き出しで、すべてのオブジェクトとそれぞれのメタデータがサポートされ、サブスクリプションデータモデルの共有、分析およびデザインに使用できます。

## API の強化 {#api-enhancements}

* **Submit Form API**：2 つ以上のリードレコードでメールアドレスが重複している場合、「最終更新日」レコードは完全にスキップする代わりに更新されます。Forms 2.0 API と同等の機能を提供します。

* **Email API**：チャンピオンまたは挑戦者のメールアセットを取得します。日付範囲フィルターを使用してメールアセットを取得します。

**_四半期を通した段階的リリース_**

以下の機能はリリース後約 1～2 か月の間に段階的にリリースされます。

## [!DNL Sales Insight] {#sales-insight}

![（星印）](assets/yellow-star.png)

* **Salesforce CRM ユーザーのリード、連絡先、アカウント、商談アクティビティに対する可視性の向上**:[!DNL Sales Insight] でのエンゲージメントレコード数が増加したため、ロングセールスサイクル中の見込み客とのエンゲージメントに関する情報が多くなりました。 「注目のアクティビティ」、「web アクティビティ」、「メール」、「スコア」の各タブには、リード、連絡先、アカウント、商談の各オブジェクトにわたって最大 400 個のアクティビティが表示されます。

## [!DNL Sales Connect] {#sales-connect}

![（星印）](assets/yellow-star.png)

* **メール接続スロットリング（ベータ版）**：Sales Connect 用のメール接続スロットリングを使用して、メールの配信可能性を向上させ、パーソナライズされた販売コミュニケーションを拡大します。この新しいテクノロジーは、メール送信のタイミングを自動的に管理し、[!DNL Exchange] と Gmail のユーザーにシームレスなエクスペリエンスを作成します。 サードパーティの一括電子メール送信アプリケーションの使用を減らすか排除し、[!DNL Sales Connect] からのすべての電子メールを自信を持って送信します。

>[!NOTE]
>
>ベータ版でメールのスロットルを使用できるようになりました。[詳細情報](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)

* **セールスアクティビティインサイトの強化**：セールスチームの以前の活動に基づいて、パーソナライズされたエンゲージメントをキャプチャし、アクティブ化します。セールスコールの記録リンク、セールスキャンペーン名、セールスメールの件名などの新しい属性を、Marketo Engage のスマートリストで使用できます。これらのアクティビティは、Marketo Engage REST API または一括書き出しを通じて書き出しおよび報告でき、スマートリストの追加の制約としてフィルターおよびトリガーで使用できます。

## [!DNL Bizible] {#bizible}

![](assets/yellow-star.png)

* **[!DNL Bizible][!DNL LinkedIn] Lead Gen Forms Integration**: マーケターは、フォームの入力をリード生成Forms広告ユニットを通じてキャプチャする際に発生するコンバージョンに対して、売上高アトリビューションを行 [!DNL LinkedIn] ことができるようになりました。 これらのインサイトを使用して、フォームのパフォーマンスと有料メディアへの投資を最適化できます。[!DNL LinkedIn] リード世代Formsは、[!DNL LinkedIn] で最も急速に成長している有料メディア製品の 1 つです。この新しい機能は、[!DNL Bizible] との既存の [!DNL LinkedIn] Ads 統合に含まれています。 
 
* **Velocity ダッシュボードの改善**：より深いインサイトを得るための新しい Velocity 指標とダッシュボードフィルターを追加しました。このダッシュボードは、マーケターが段階的なリードと商談の速度、および様々な形式のマーケティングとセールスエンゲージメントの効率を理解するために使用します。

* **新しいコホートウォーターフォールジャーニーダッシュボード**：これにより、マーケターは従来の「デマンドウォーターフォール」段階セットを通じて、選択したコホートの進行状況を表示でき、コンバージョン率と暗黙の段階的なコンバージョンの因果関係を段階的にすばやく把握できます。

## Adobe Experience Cloudとの [!DNL Bizible] の統合 {#bizible-integration-with-adobe-experience-cloud}

この節では、Adobe Identity Management System（IMS）の移行を完了した Bizible ユーザー向けの新機能について説明します。移行済みの場合は、「Adobe ID」タブの [!DNL Bizible] 設定に新しいAdobe IDが表示されます。 2021年末までにすべてのアカウントを移行する必要があります。

* **[!DNL Bizible]とAdobe Privacy Serviceとの統合** （2021 年 9 月に利用可能）:[!DNL Bizible] とAdobe Privacy Serviceとの統合により、Adobe Experience Cloud アプリケーション全体で重要なデータプライバシー規制（GDPR など）へのコンプライアンスが一元化されます。 このサービスを利用して、すべてのプライバシーリクエストを一元的に管理できるようになり、[!DNL Bizible] や他のAdobe製品に寄せられた変更リクエストがアプリケーション全体に反映されます。

* Adobe統合シェルに **[!DNL Bizible]いて**: [!DNL Bizible] でAdobe統合シェルが採用されたことにより、[!DNL Bizible] アプリケーションヘッダーバーに表示される新機能がユーザーに提供されます。この新機能には、リソースのサポートやアプリケーションの切り替えへのアクセス改善が含まれます。 Adobe統合シェルは、[!DNL Bizible] と他のAdobe Experience Cloud アプリケーション間で一貫したエクスペリエンスを作成するのに役立ちます。

* **[!DNL Bizible]Domain Ownership and Self-Management**: [!DNL Bizible] ユーザーは、Adobe Admin Consoleを利用して、トラッキング対象のドメインを管理 [!DNL Bizible] きます。 セルフサービスを以前に手動で行うプロセスに移行し、Adobe Experience Cloud アプリケーションでドメインの所有とトラッキングをどのように管理するかで、一貫したエクスペリエンスを提供できます。

## お知らせ {#announcements}

* **サブスクリプションユニバーサル ID 設定の更新**：今後の Marketo Engage と Adobe ID の統合を既存のユーザーに対してサポートするために、ユニバーサル ID のサポートが有効化されて、すべての Marketo Engage の購読が統合されます。詳しくは[こちら](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)でご覧ください。

**_製品リリースウェビナー_**

[2021 年 8 月の Marketo Engage リリースウェビナー](https://engage.marketo.com/August21_Release_Webinar.html)
