---
description: リリースノート - 2021年8月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2021年8月
source-git-commit: 366f1cac07c30b5f928d3d1b6a1c530011ca83d0
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 6%

---

# リリースノート：2021年8月 {#release-notes-aug-21}

8 月 22 日リリースには、次の機能が含まれています。 機能の可用性については、Marketo Engageのエディションを確認してください。

>[!AVAILABILITY]
>
>星印（![](assets/yellow-star.png)）がついている機能は有償オプションになります。詳しくは、AdobeMarketo Engage担当者にお問い合わせください。

**_四半期リリース_**

**2021 年 8 月 20 日** に、次の機能がリリースされます。

## エクスペリエンスの自動化 {#experience-automation}

* **Marketo EngageID を使用したAdobeユーザー認証**:近日中に、Enterprise パッケージを持つ新しいMarketo Engageユーザーが、Adobe IDのユーザー資格情報を使用してオンボーディングされます。現在のユーザーの統合 ID システムへの移行は、2022 年中頃までおこなわれず、追加の通知がおこなわれるまでは、何の操作も必要ありません。 AdobeID ユーザー認証を使用すると、IT/セキュリティ管理者は、他のMarketo Engageソリューションと共に複数のExperience Cloud製品インスタンスを管理したり、共通のコンソールを通じて SSO を設定したりできます。 管理者は、ユーザーグループとユーザーの使用権限を 1 か所で簡単に管理できます。

* **実行可能なキャンペーンのネスト**:実行可能なキャンペーンで、他の実行可能なキャンペーンを呼び出して、最大 3 レベルの深さまでネストできるようになりました。これにより、共通の運用フローをさらに統合し、Smart Campaign 管理を強化できます。

* **個人の詳細ページでの単一フローアクション** （9 月 9 日までに利用可能）:データベースのグリッド表示に切り替えずに、フローアクションメニューを使用して、個々の人に対する電子メールの送信、個人所有者の変更、その他のスマートキャンペーンアクションを実行できます。

* **[カスタムアクティビティのエクスポート](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)**:メタデータの書き出しで、すべてのオブジェクトとそれぞれのメタデータがサポートされ、サブスクリプションデータモデルの共有、分析、デザインに使用できます。

## API の機能強化 {#api-enhancements}

* **フォーム送信 API**:E メールアドレスが 2 つ以上のリードレコードで重複している場合、「最終更新日」レコードは完全にスキップするのではなく更新されます。Forms 2.0 API と同等です。

* **電子メール API**:チャンピオンまたはチャレンジャーの E メールアセットを取得します。日付範囲フィルターを使用して E メールアセットを取得します。

**_四半期を通した段階的リリース_**

以下の機能はリリース後約 1 ～ 2 か月の間に段階的にリリースされます。

## Sales Insight {#sales-insight}

![（星印）](assets/yellow-star.png)

* **Salesforce CRM ユーザー向けのリード、連絡先、アカウント、オポチュニティのアクティビティの可視性の向上**:Sales Insight のエンゲージメントレコード数が増えたため、長い販売サイクルの間の見込み客とのエンゲージメントは、より多くの情報を得られます。興味深い瞬間、Web アクティビティ、E メール、スコアの各タブには、リード、連絡先、アカウント、オポチュニティの各オブジェクトにわたって、最大 400 個のアクティビティが表示されます。

## Sales Connect {#sales-connect}

![（星印）](assets/yellow-star.png)

* **E メール接続のスロットリング（ベータ版）**:E メールの配信品質を向上し、Sales Connect 用の E メール接続のスロットリングを使用して、パーソナライズされた販売コミュニケーションを拡大/縮小します。この新しいテクノロジーは、E メールの送信タイミングを自動的に管理し、Exchange および Gmail ユーザーに対してシームレスなエクスペリエンスを作成します。 サードパーティの一括電子メール送信アプリケーションの使用を減らすか、減らすか、減らして、Sales Connect から確実にすべての電子メールを送信します。

>[!NOTE]
>
>ベータ版では、E メールのスロットリングを使用できます。 [詳細情報](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)

* **販売活動インサイトの強化**:セールスチームの事前の活動に基づいて、パーソナライズされたエンゲージメントをキャプチャし、アクティブ化します。Marketo Engageのスマートリストで、販売呼び出しの記録リンク、販売キャンペーン名、販売電子メールの件名などの新しい属性を使用できます。  これらのアクティビティは、Marketo Engageの REST API または一括書き出しを通じて書き出しおよびレポートでき、フィルターおよびトリガーで、スマートリストの追加の制約として使用できます。

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Bizible LinkedIn Lead Gen Formsの統合**:LinkedInがリードジェネレーションFormsの広告ユニットを通じてフォームを取り込む際に発生するコンバージョンに対して売上高アトリビューションを実行できるようになりました。これらのインサイトを使用して、フォームのパフォーマンスと有料メディアへの投資を最適化できます。 linkedIn Lead Gen Formsは、LinkedInで最も急速に成長している有料メディア製品の 1 つで、この新機能は、Bizible との既存のLinkedIn Ads 統合に含まれています。 
 
* **Velocity ダッシュボードの改善**:より深いインサイトを得るための新しい Velocity 指標とダッシュボードフィルターを追加しました。このダッシュボードは、マーケターが段階的なリードとオポチュニティの速度、および様々な形式のマーケティングと販売のエンゲージメントの効率を理解するために使用します。

* **新しいコホートウォーターフォールジャーニーダッシュボード**:これにより、マーケティング担当者は、従来の「デマンドウォーターフォール」段階セットを通じて、選択したコホートの進行状況を把握し、コンバージョン率と暗黙の段階的なコンバージョンの因果関係を段階的に把握できます。

## Bizible とAdobe Experience Cloudの統合 {#bizible-integration-with-adobe-experience-cloud}

この節では、AdobeIdentity Managementシステム (IMS) の移行を完了した Bizible ユーザー向けの新機能について説明します。 移行済みの場合は、新しいAdobe IDが「Adobe ID」タブの Bizible 設定に表示されます。 2021 年末までにすべてのアカウントを移行する必要があります。

* **Bizible とAdobePrivacy Serviceの統合** （2021 年 9 月から利用可能）:Bizible とAdobePrivacy Serviceの統合により、Adobe Experience Cloudアプリケーション全体の重要なデータプライバシー規制（GDPR など）へのコンプライアンスを一元化します。このサービスを利用してすべてのプライバシーリクエストを一元管理できるようになり、Bizible や他のAdobe製品に対する変更リクエストがアプリケーション間で反映されるようになりました。

* **Bizible のAdobe統合シェル**:Bizible のAdobe統合シェルの採用により、Bizible アプリケーションのヘッダーバーに表示される新しい機能と、より優れたリソースおよびアプリケーションの切り替えをサポートする機能がユーザーに提供されます。Adobe統合シェルは、Bizible と他のAdobe Experience Cloudアプリケーションとの間で一貫したエクスペリエンスを作成するのに役立ちます。

* **Bizible ドメインの所有権と自己管理**:Bizible ユーザーは、Adobe Admin Consoleを活用して、Bizible で追跡するドメインを管理できます。これにより、セルフサービスを以前に手動でおこなうことができ、ドメインの所有権と追跡をAdobe Experience Cloudアプリケーション全体で一貫した方法で管理できます。

## お知らせ {#announcements}

* **購読ユニバーサル ID 設定の更新**:今後のMarketo EngageとAdobeID の統合を既存のユーザーに対してサポートするために、ユニバーサル ID サポートの有効化ですべてのMarketo Engageの購読が統合されます。詳しくは[こちら](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)をご覧さい。
