---
description: リリースノート - 2021年8月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2021年8月
exl-id: 4aec4e0b-520e-4786-a110-8e68f1bf9950
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 6%

---

# リリースノート：2021年8月 {#release-notes-aug-21}

2021 年 8 月リリースには、次の機能が含まれています。 Marketo Engageエディションの機能が使用できるかどうかを確認します。

>[!AVAILABILITY]
>
>星印（![](assets/yellow-star.png)）がついている機能は有償オプションになります。詳しくは、AdobeMarketo Engage担当者にお問い合わせください。

**_四半期リリース_**

以下の機能がにリリースされます。 **2021 年 8 月 21 日**.

## エクスペリエンスの自動化 {#experience-automation}

* **Marketo EngageID を使用したAdobeユーザー認証**:近日中に、Enterprise パッケージを持つ新しいMarketo Engageユーザーは、Adobe IDのユーザー資格情報を使用してオンボーディングされます。 統合 ID システムへの現在のユーザーの移行は、2022 年半ばまでおこなわれず、追加の通知がおこなわれるまでは、何の操作も必要ありません。 AdobeID のユーザー認証を使用すると、IT/セキュリティ管理者は、他のMarketo Engageソリューションと共に複数のExperience Cloud製品インスタンスを管理し、共通のコンソールを通じて SSO を設定できます。 管理者は、ユーザーグループとユーザーの使用権限を 1 か所で簡単に管理できます。

* **実行可能なキャンペーンのネスト**:実行可能なキャンペーンで、他の実行可能なキャンペーンを呼び出し、最大 3 レベルの深さまでネストできるようになりました。 これにより、共通の運用フローをさらに統合し、スマートキャンペーン管理を改善できます。

* **担当者詳細ページの単一フローアクション** （9 月 9 日まで）:データベースのグリッド表示に切り替えずに、フローアクションメニューを使用して、個人の担当者に対してメールの送信、担当者所有者の変更、その他のスマートキャンペーンアクションを実行できます。

* **[カスタムアクティビティのエクスポート](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)**:メタデータの書き出しで、すべてのオブジェクトとそれぞれのメタデータがサポートされ、サブスクリプションデータモデルの共有、分析およびデザインに使用できます。

## API の強化 {#api-enhancements}

* **フォーム API を送信**:2 つ以上のリードレコードで E メールアドレスが重複している場合、「最終更新日」レコードは完全にスキップする代わりに更新されます。 Forms 2.0 API と同等の機能を提供します。

* **メール API**:チャンピオンまたは挑戦者の E メールアセットを取得します。 日付範囲フィルターを使用して E メールアセットを取得します。

**_四半期を通した段階的リリース_**

以下の機能はリリース後約 1 ～ 2 か月の間に段階的にリリースされます。

## Sales Insight {#sales-insight}

![（星印）](assets/yellow-star.png)

* **Salesforce CRM ユーザーのリード、連絡先、アカウント、商談アクティビティの可視性の向上**:長いセールスサイクルの間の見込み客とのエンゲージメントは、Sales Insight のエンゲージメントレコード数が増えたため、より多くの情報を得られます。 注目のアクティビティ、Web アクティビティ、メール、スコアの各タブには、リード、連絡先、アカウント、商談の各オブジェクトにわたって最大 400 個のアクティビティが表示されます。

## Sales Connect {#sales-connect}

![（星印）](assets/yellow-star.png)

* **メール接続の制限（ベータ版）**:E メールの配信品質を向上し、Sales Connect 用の E メール接続のスロットリングを使用して、パーソナライズされたセールスコミュニケーションを拡大・縮小します。 この新しいテクノロジーは、Exchange および Gmail ユーザーに対してシームレスなエクスペリエンスを作成するために、E メールの送信タイミングを自動的に管理します。 サードパーティの一括電子メール送信アプリケーションの使用を減らすか、減らすか、減らすか、減らして、セールスコネクトから確実にすべての電子メールを送信します。

>[!NOTE]
>
>ベータ版では、E メールのスロットルを使用できるようになりました。 [詳細情報](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)

* **セールスアクティビティインサイトの強化**:セールスチームの以前の活動に基づいて、パーソナライズされたエンゲージメントをキャプチャし、アクティブ化します。 セールスコールの記録リンク、セールスキャンペーン名、セールスメールの件名などの新しい属性を、Marketo Engageのスマートリストで使用できます。  これらのアクティビティは、Marketo EngageREST API または一括書き出しを通じて書き出しおよび報告でき、スマートリストの追加の制約としてフィルターおよびトリガーで使用できます。

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Bizible LinkedIn Lead Gen Forms統合**:LinkedInがリードジェネレーションFormsの広告ユニットを通じてフォームの入力をキャプチャする際に発生するコンバージョンに対して売上高属性を実行できるようになりました。 これらのインサイトを使用して、フォームのパフォーマンスと有料メディアへの投資を最適化できます。 linkedInリードジェネレーションFormsは、LinkedInで最も急速に成長している有料メディア製品の 1 つで、この新機能は、Bizible との既存のLinkedIn広告統合に含まれています。   
* **Velocity ダッシュボードの改善**:より深いインサイトを得るための新しい Velocity 指標とダッシュボードフィルターを追加しました。 このダッシュボードは、マーケターが段階的なリードとオポチュニティの速度、および様々な形式のマーケティングとセールスエンゲージメントの効率を理解するために使用します。

* **新しいコホートウォーターフォールジャーニーダッシュボード**:これにより、マーケターは従来の「デマンドウォーターフォール」段階セットを通じて、選択したコホートの進行状況を表示でき、コンバージョン率と暗黙の段階的なコンバージョンの因果関係を段階的にすばやく把握できます。

## Adobe Experience Cloudとの Bizible 統合 {#bizible-integration-with-adobe-experience-cloud}

この節では、AdobeIdentity Management System(IMS) の移行を完了した Bizible ユーザー向けの新機能について説明します。 移行済みの場合は、新しいAdobe IDが「Adobe ID」タブの Bizible 設定に表示されます。 2021 年末までにすべてのアカウントを移行する必要があります。

* **Bizible とAdobePrivacy Service** （2021 年 9 月から利用可能）:Bizible とAdobePrivacy Serviceの統合により、Adobe Experience Cloudアプリケーション全体での重要なデータプライバシー規制（GDPR など）へのコンプライアンスを一元化します。 このサービスを活用し、すべてのプライバシーリクエストを一元的に管理できるようになり、Bizible や他のAdobe製品に対する変更リクエストがアプリケーション間で反映されるようになりました。

* **Bizible onAdobe統合シェル**:Bizible のAdobe統合シェルの採用により、Bizible アプリケーションヘッダーバーに表示される新しい機能と、サポートリソースおよびアプリケーションの切り替えへのより優れたアクセスをユーザーに提供します。 Adobe統合シェルは、Bizible と他のAdobe Experience Cloudアプリケーションとの間で一貫したエクスペリエンスを作成するのに役立ちます。

* **Bizible ドメインの所有権と自己管理**:Bizible ユーザーは、Adobe Admin Consoleを活用して、Bizible で追跡するドメインを管理できます。 これにより、セルフサービスを以前に手動でおこなうプロセスに移行し、Adobe Experience Cloudアプリケーションでドメインの所有と追跡をどのように管理するかで、一貫したエクスペリエンスを提供します。

## お知らせ {#announcements}

* **サブスクリプションユニバーサル ID 設定の更新**:今後のMarketo EngageとAdobeID の統合を既存のユーザーに対してサポートするために、ユニバーサル ID のサポートを有効にする際に、すべてのMarketo Engageの購読が統合されます。 詳しくは[こちら](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)をご覧さい。

**_製品リリースウェビナー_**

[2021 年 8 月のMarketo Engageリリースウェビナー](https://engage.marketo.com/August21_Release_Webinar.html)
