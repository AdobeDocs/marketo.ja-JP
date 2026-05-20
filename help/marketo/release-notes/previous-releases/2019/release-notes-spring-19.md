---
unique-page-id: 17728380
description: リリースノート - 2019年春 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2019年春
exl-id: eb7a9ac4-5c3d-4d98-9b06-e3f11147bc6d
TQID: https://experienceleague.adobe.com/o63AwYraOGknprRVOS0i6gMRhp9JfFnVSmbK4wHOjgE
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: ffdd6159-0e10-4a57-8021-94e93bab8183
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: bbbea26f-9621-49eb-9ab8-e06fb3bbce8c
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 466
ht-degree: 100%

---

# リリースノート：2019年春 {#release-notes-spring}

2019年春リリースには、次の機能が含まれています。 機能の可用性についてはお使いの Marketo のエディションをご確認ください。

各機能の詳細な記事を表示するには、タイトルリンクをクリックしてください（ある場合）。

***四半期リリース_**

2019年3月15日に、次の機能がリリースされました。

## 主要プラットフォームの機能拡張 {#core-platform-enhancements}

* **待機リスト**：空きが出るまで[メンバーを保留にする](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md)ためにメンバーを待機リストに登録する新しいプログラム／イベントステータス これは、Marketo Classic のイベントプログラムに関連するチャネルと、[!DNL Marketo Sky] のイベントとウェビナー付きイベントの両方のプログラムに当てはまります。 デフォルトでは、待機リストは登録済みと同じステップ値を持ちます。
* **[カスタム通信制限](/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md)**：管理者は、1 日または 1 週間のカスタム通信制限を設定できるようになりました。
* **[スマートキャンペーンアセット API](https://developers.marketo.com/rest-api/assets/smart-campaigns/)**：更新された日付と ID によってスマートキャンペーンレコードを取得して、Marketo 外で分析をエンリッチメントします。
* **メール用 HTTPS トラッキングリンク**：「トラッキングリンクのセキュリティで保護されたドメイン」を購入した顧客の場合、ブランディングされたトラッキングリンクをメール内に HTTPS として表示できるようになりました。
* **メール到達率 PowerPack の更新**：特定のテスト結果にフラグを設定してコメントを付け、URL を通じて結果を関係者と共有し、変更を追跡して、関係者がコンテンツを編集したときにメールがどのように変化したかを確認する機能。

アカウントベースドマーケティング

**[アカウント AI](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md)** が一般に利用可能になりました。 アカウント AI は、人工知能を使用して ABM 戦略のターゲットとすべきアカウントを明確にします。

<br> 

**_四半期以外のリリース_**

2019年の第 1 四半期と第 2 四半期の初めにかけて、次の機能がリリースされる予定です。

## [!DNL Marketo Sky] {#marketo-sky}

* **完全なメールプログラム機能**：メールの送信、A/B テストの作成、結果の追跡を、ユーザにとってわかりやすいエクスペリエンスで行います。
* **スマートキャンペーン機能**：スマートキャンペーン機能が Sky で展開を続けるので、新しいユーザインターフェイスで安定性が向上します。
* **デザインスタジオアセットを管理**：テンプレート、画像、Forms、スニペット、ファイル、メール、ランディングページをデザインスタジオのリストビューから一括で管理する機能が追加されました。
* **受信者タイムゾーンダッシュボードで配信**：Sky の受信者タイムゾーン配信機能を使用して送信されたメールに関するレポートで、顧客の行動を把握します。

## Marketo Sales Engage {#marketo-sales-engage}

* **監査の強化**：他のユーザによって作成された[既存のキャンペーンを終了](/help/marketo/product-docs/marketo-sales-connect/campaigns/view-campaigns-list-as-another-user.md)する機能が追加された、インスタンス内のすべてのユーザ、メール、および[コンテンツ](/help/marketo/product-docs/marketo-sales-connect/templates/view-template-list-as-another-user.md)に対する新しい可視性。
* **[登録解除管理](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/marketo-unsubscribe-check.md)**：[メールドメインへの接続をブロック](/help/marketo/product-docs/marketo-sales-connect/admin/blocked-domains.md)する機能を使用して、メール到達率とコンプライアンスを最大化します。 また、Marketo は、メールを送信する前に、登録解除用のリードデータベースを相互参照します。

## Marketo による [!DNL Bizible] {#bizible-by-marketo}

* **[!DNL Bizible]Discover の機能強化**：新しいダッシュボードセグメント化機能により、マーケターはパフォーマンスをより深く理解できるようになります。
* **複数通貨のサポート**：CRM 通貨テーブルに組み込まれた [!DNL Bizible] の新しい自動通貨変換機能を使用して、企業通貨と現地通貨を切り替えます。
* **CRM キャンペーンコスト**：CRM キャンペーンオブジェクトからコストデータを自動的に取り込む機能を使用して、オフラインマーケティングアクティビティの費用と ROI を測定します。
