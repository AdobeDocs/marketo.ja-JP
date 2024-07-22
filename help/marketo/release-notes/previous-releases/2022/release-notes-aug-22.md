---
description: リリースノート - 2022 年 8 月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2022 年 8 月
exl-id: 7a224fa7-0aec-4d0d-9535-c35241a45654
feature: Release Information
source-git-commit: 206952c2aaa9b568a9312def6d36b15f699791b3
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 16%

---

# リリースノート：2022 年 8 月 {#release-notes-aug-22}

以下に、2022 年 8 月リリースに含まれるすべての機能を示します。 機能の可用性についてはお使いの Marketo Engage のエディションをご確認ください。

>[!AVAILABILITY]
>
>星（![星](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

次の機能は、**2022 年 8 月 26 日（PT）** に段階的にロールアウトを開始しました。

## クロスチャネルオーケストレーション {#cross-channel-orchestration}

* **[Dynamic Chat用にすべての公開済みダイアログを一度に有効/無効にする](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/dialogue-overview.md#disable-enable-all-dialogues){target="_blank"}**：ボタンを押しながら、設定ページから一度にすべての公開済みダイアログをグローバルに有効/無効にします。

* **[Dynamic Chat用のカスタムアバター](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/configuration.md#agent-settings){target="_blank"}**：カスタムチャットボットアバターをアップロードして、ブランドにパーソナライズできるようにします。

* **Dynamic Chat向けのチャットトランスクリプト**：すべての会話のチャットトランスクリプトを表示して、各 web 訪問者が何に興味を持っているかについて深いインサイトを得ます。

## 次世代のエクスペリエンス

* **Adobeのブランディング**：新しいAdobe Experience Cloud ブランディングにより、編集者およびユーザーの詳細ページのルックアンドフィールが更新されました。

* **移動ダイアログでの保存先フォルダーのフォルダー階層の表示**：各フォルダーのフォルダー階層を表示すると、アセットの移動が容易になり、誤ったフォルダーに入れられる可能性が低減されます。

* **[次世代エクスペリエンスのための画面の更新](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md){target="_blank"}**：次世代のエクスペリエンスで、トグルスイッチを介してアクセス可能な、最新のデザインと操作性の強化を備えた新しい画面を追加しました。

   * スニペット詳細
   * 「画像とファイル」の詳細

>[!NOTE]
>
>例外は、マーケティングアクティビティのプログラム内のフォルダーにアセットを移動することです。 プログラム内のフォルダーの名前が重複する可能性があるため、この移動アクションではフォルダー階層が表示されません。

## エクスペリエンスの自動化 {#experience-automation}

* **[セルフサービスフローステップ – プログラムのインポートの機能強化](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/flow-step-service.md){target="_blank"}**：カスタムフローステップを使用したプログラムのインポートのサポートが改善されました。これにより、同じサービスプロバイダーの複数のインスタンスを使用して、これらのサービスプロバイダーと互換性のあるフローステップを持つプログラムをインポートできるようになりました。

* **Munchkin – 拡張リンクトラッキング**:Munchkin を使用して `tel` および `mailto` リンクのトラッキングのサポートを拡張し、web 動作の拡張されたセットを追跡します。

* **Webhook カスタムヘッダーの表示**:Webhook カスタムヘッダーが管理者/「Webhook」タブに表示され、可視性が向上しました。

* **CAPTCHA**：受信フォームトラフィックにスコアを付けるため、フォーム送信の有効性を評価します [reCAPTCHA v3 を使用 ](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"}。 疑わしいボットトラフィックを自動的に除外、強制隔離または削除するマーケティングワークフローを作成します。

* **フォームの承認権限**：他の Design Studio アセットと連動して、フォームの変更を承認できる設計者を制御する新しい権限が追加されました。 これにより、他のデザイナーが、承認の権限を持つ他のユーザーがレビューすることなくフォームに変更をプッシュすることを防ぎます。

* **匿名結合後に常にキャンペーン再生を実行**：匿名のリード結合はキャンペーン再生の前に行われるので、匿名キャンペーン再生が行われるとカスタムフィールドフィルターが確実に動作します。

## マーケティングデータ環境 {#marketing-data-environment}

* **カスタムオブジェクトの「Used By」フィールドの UI 切り捨てを修正**：必要に応じてカスタムオブジェクトからフィールドを削除できるように、「使用中」のカスタムオブジェクトフィールドを識別しやすくなりました。

## API の強化 {#api-enhancements}

* **Bulk Program Member Extract API の新しいフィルタリング機能**：プログラムメンバーシップステータス、updatedAt、ケイデンスまたは使い果たしたコンテンツでフィルタリングして、抽出したデータセットを絞り込みます。

## Sales Insight {#sales-insight}

![（星印）](assets/yellow-star.png)

* **[Sales Insight とDynamic Chatの統合](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}**: Sales Insight パネルのDynamic Chatからアクティビティを表示し、この新しいデータポイントを見込み客調査に活用します。

## お知らせ {#announcements}

**_製品リリースウェビナー_**

[2022 年 6 月および 8 月のMarketo Engageリリースウェビナー ](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
