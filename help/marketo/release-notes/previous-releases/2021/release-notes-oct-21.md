---
description: リリースノート - 2021 年 10 月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2021 年 10 月
exl-id: 6b363c9b-7abe-4576-a362-0ad5cf515c02
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 77%

---

# リリースノート：2021 年 10 月 {#release-notes-oct-21}

2021 年 10 月リリースには以下の新機能が含まれています。機能の可用性についてはお使いの Marketo Engage のエディションをご確認ください。

>[!AVAILABILITY]
>
>星印（![](assets/yellow-star.png)）がついている機能は有償オプションになります。詳細は Marketo Engage 担当営業にお問い合わせください。

**_四半期リリース_**

以下の機能のリリースは、**2022 年 10 月 22 日**&#x200B;に始まり、（特に指定のない限り）次の週から各機能が段階的にロールアウトされます。

## AI 主導型イノベーション {#ai-driven-innovation}

* **予測オーディエンスの強化**：イベントやメールプログラムで使用される AI を活用した予測モデルに対する AI 予測に影響を与えている上位の行動を、より明確に把握できるようになりました。イベントの登録と出席率が高くなるキャンペーンメンバーの行動や、登録解除につながる要因を確認できます。AI を利用した類似モデルが、Marketo Engage のすべてのプログラムタイプで使用できるようになりました。

## 次世代のエクスペリエンス {#next-gen-experience}

* **独自のエクスペリエンスを選択**：Marketo Engage フォームの詳細やランディングページのリスト表示を操作しながら、コンテキスト、アセットの変更や環境設定を失うことなく、新しいスイッチで簡単に希望のエクスペリエンスに切り替えることができます。さらに、新しいランディングページのリスト表示でのフィルターと一括アクションの実行機能で、エクスペリエンスが強化します。

* **効率的に検索**：キーボードナビゲーションとラベルの説明の更新、結果の新しいスクロール機能、適用されたフィルターの表示などで、グローバル検索のアクセシビリティを改善しました。

* **タスクの監視**：グローバルナビゲーションバーの新しいタスク通知トレイを使用して、新しいエクスペリエンスのバックグラウンドで実行されているタスクのステータスを監視します。トレイは、フォームの詳細とランディングページのリストの新しいエクスペリエンス表示から開始されるタスクに関する通知をキャプチャします。これには、ランディングページのステータスの変更や、新しいエクスペリエンスを使用した一般的な一括操作が含まれます。

## エクスペリエンスの自動化 {#experience-automation}

* **フォーム API プログラムメンバーのカスタムフィールドサポートの送信**：Submit Form API エンドポイントが、プログラムメンバーカスタムフィールドをサポートするようにアップグレードされ、カスタムフォームの統合でプログラム固有のデータを収集できるようになりました。

**_四半期を通した段階的リリース_**

以下の機能はリリース後約 1～2 か月の間に段階的にリリースされます。

* **オーディエンスを Marketo Engage に共有するためのネイティブ Adobe Experience Platform Connector**：ネイティブの宛先コネクタを介して Adobe Experience Platform で作成されたオーディエンスセグメントに対して、Marketo Engage でのマルチチャネルのキャンペーンオーケストレーションを有効にします。コネクタは、メールアドレスまたは ECID を使用して、Adobe Experience Platform プロファイルを Marketo Engage 人物レコードと照合し、アプリケーション間でセグメントを共有します。Marketo Engage の静的リストは自動的に入力され、マーケターは、高度にパーソナライズされたメッセージングやワークフローを使用してターゲットオーディエンスにリーチできます。顧客オーディエンスをアクティブ化し、自分の顧客と商談のコンテキスト、および Experience Platform でのより完全なリアルタイム統合プロファイルを活用できます。

* **Adobe Experience Platform Marketo Data Source Connector**：Adobe Experience Platform と Marketo Engage の両方のユーザーが、Marketo Source Connector を利用して Marketo から AEP にデータを取り込むことができます。AEP 内で Marketo からデータ（およびその変更）をストリーミングして、2 つの製品間のデータの一貫性を維持できます。Marketo コネクタは、ソースカタログ（「アドビアプリケーション」の下）で確認できます。

## [!DNL Sales Insight] {#sales-insight}

![（星印）](assets/yellow-star.png)

[!DNL Microsoft Dynamics 365] セールス向け **[!DNL Sales Insight]ール**

* **[!UICONTROL ベストベット ] 機能強化**:[!DNL Sales Insight] の [!UICONTROL  ベストベット ] タブには、品質と緊急度に基づいて優先度が付けられた、最もホットな連絡先とリードのリアルタイムビューが表示されます。 担当者がスコアの確認、メールの送信、[!DNL Best Bets] ールページから直接指定されたMarketo Engage キャンペーンへの見込み客の追加などのアクションを実行する機能が追加され、効率が向上し、応答時間が短縮されました。

* **新規メール、web アクティビティ、匿名 web アクティビティダッシュボード**：新しいセールスダッシュボードを追加し、販売者にリードや連絡先の最新のメールおよび web アクティビティについて知らせるようにしました。新しいフィルタリング機能により、ダッシュボードで、メールの開封数、クリック数、web ページへの訪問回数に関するインサイトが得られ、完全な顧客リストや特定の顧客が得られます。Marketo Engage は、すべての web アクティビティを追跡し、セールスに重要な情報を提供し、匿名トラフィックをリードに変えます。販売者は、リード行動に関するより深い情報を得て、すべてのタッチポイントの関連度に基づいて行動し、エンゲージメントをパーソナライズし、リードをより速く販売に変換できます。

**[!DNL Sales Insight]for[!DNL Salesforce]**

* **アカウントおよび商談レベル [!UICONTROL  おすすめコンテンツ]**:[!DNL Sales Insight] は、販売担当者が所有するアカウントまたは商談のすべての連絡先に関して、連絡先が別のチームメンバーに割り当てられている場合でも、おすすめコンテンツを確認できるようになりました。 これにより、顧客と商談の所有者は、関連する連絡先のアクティビティを完全に可視化し、顧客と商談のより包括的な視点に基づいて行動できるようになります。

## [!DNL Sales Connect] {#sales-connect}

![（星印）](assets/yellow-star.png)

* **セールスアクティビティインサイトの強化**：新しいメール返信追跡アクティビティ「返信済みセールスメール」は、Marketo Engage と自動的に同期された電子メールでの受信者のインタラクションを追跡します。さらに、ソース属性が「Tout」から「Sales App」に更新されました。このアクティビティは、Marketo Engage REST API または一括書き出しを通じて書き出しおよびレポートでき、スマートリストの追加の制約としてフィルターやトリガーで使用し、スマートキャンペーンのパーソナライゼーションオプションを拡張できます。

* **ユーザーエクスペリエンスの効率化**：このアップデートでは、Adobe Spectrum デザインシステムに基づいた [!DNL Sales Connect] ーザー向けの新しいフォント、カラー、ボタン、モーダルが導入されました。 これらのアップデートにより、より効率的なエクスペリエンスを提供しています。販売者は、必要なときに必要なものに焦点を当てることができます。

## [!DNL Bizible] {#bizible}

![](assets/yellow-star.png)

* Adobe Privacy Service（GA）との **[!DNL Bizible]統合**:Adobe Privacy Serviceとの [!DNL Bizible] 統合により、Adobe Experience Cloud アプリケーション全体で GDPR （EU 一般データプライバシー規則）や CCPA （カリフォルニア州消費者プライバシー法）などの重要なデータプライバシー規則へのコンプライアンスが一元化されます。 このサービスを利用して、Adobe Privacy Serviceを通じてすべてのプライバシーリクエストを一元的に管理し、他のAdobe製品に [!DNL Bizible] まれる変更リクエストがアプリケーション全体に反映されるようになりました。

## お知らせ {#announcements}

* **リード廃止／Munchkin ベータ版 161 アップデートの関連付け**：2021 年 9 月 7 日に、Munchkin のバージョン 161 は、Munchkin ベータ版を有効にしてサブスクリプションの 10%に展開し始め、次いで 9 月 16 日に 50%、9 月 30 日に 100%に展開しました。この変更は、Marketo Engage のランディングページと、最近のバージョンがロールアウトされたサブスクリプションから読み込まれる外部のランディングページに提供されるファイル munchkin-beta.js のバージョンに影響します。このバージョンでは、[!DNL Munchkin] Associate Lead メソッドは完全に廃止されています。このメソッドは、人物のデータをMarketo Engage サブスクリプションに送信し、関連する web ブラウジング履歴を既知の人物レコードと関連付けることができる機能です。 Forms JS API、フォーム送信 API、Associate Lead REST API など、より最新でセキュアな代替手段のために、「リードの関連付け」は削除されています。この廃止について詳しくは、[こちら](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)を参照してください。

* **[!DNL Sales Connect]Update**:[!DNL Sales Connect] の最近の UI 変更により、[!DNL Salesforce] の一部のモーダルが中断されました。 この問題を修正するには、[パッケージを更新](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/sales-connect-customizations-for-crm.md)してください。

**_製品リリースウェビナー_**

[2021 年 10 月の Marketo Engage リリースウェビナー](https://engage.marketo.com/October_Release_Webinar_On-Demand.html)
