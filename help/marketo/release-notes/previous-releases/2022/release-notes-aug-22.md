---
description: リリースノート - 2022 年 8 月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2022 年 8 月
exl-id: 7a224fa7-0aec-4d0d-9535-c35241a45654
source-git-commit: 85e04fb8a52a417982014bc4bb101b6044e53f84
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 13%

---

# リリースノート：2022 年 8 月 {#release-notes-aug-22}

2022 年 8 月リリースに含まれるすべての機能を以下に示します。 機能の可用性についてはお使いの Marketo Engage のエディションをご確認ください。

>[!AVAILABILITY]
>
>星（![星](assets/yellow-star.png)）で示す機能は有償オプションです。詳細は Marketo Engage 担当営業にお問い合わせください。

次の機能は、 **2022 年 8 月 27 日**.

## クロスチャネルオーケストレーション {#cross-channel-orchestration}

* **[Dynamic Chat のすべての公開済みダイアログを一度に有効化/無効化](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/dialogue-overview.md#disable-enable-all-dialogues){target=&quot;_blank&quot;}**:ボタンを押しながら、設定ページから一度にすべての公開済みダイアログをグローバルに有効化/無効化します。

* **[ダイナミックチャットのカスタムアバター](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md#agent-settings){target=&quot;_blank&quot;}**:カスタムチャットボットアバターをアップロードして、ブランドに合わせてパーソナライズできるようにします。

* **ダイナミックチャットのチャットのトランスクリプト**:各会話のチャット記録を表示して、各 Web 訪問者が興味を持っている内容に関する深いインサイトを得ます。

## 次世代のエクスペリエンス

* **Adobeのブランディング**:新しいAdobe Experience Cloudブランディングを使用して、編集者と担当者の詳細ページのルックアンドフィールを更新しました。

* **移動ダイアログで宛先フォルダのフォルダ階層を表示する**:各フォルダーのフォルダー階層を表示すると、アセットの移動が容易になり、誤ったフォルダーに配置される可能性が低くなります。

* **[次世代のエクスペリエンスの画面の更新](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md){target=&quot;_blank&quot;}**:次世代のエクスペリエンスで、トグルスイッチを介してアクセス可能な、最新のデザインと操作性の強化を提供する、新しい画面を追加で提供しています。

   * スニペットの詳細
   * 「画像とファイル」の詳細

>[!NOTE]
>
>例外は、マーケティングアクティビティのプログラム内のフォルダーにアセットを移動することです。 プログラム内のフォルダには名前が重複していないため、この移動アクションではフォルダ階層は表示されません。

## エクスペリエンスの自動化 {#experience-automation}

* **[セルフサービスフローステップ — プログラムインポートの強化](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/flow-step-service.md){target=&quot;_blank&quot;}**:同じサービスプロバイダーの複数のインスタンスを使用できるようになったカスタムフローステップを含むプログラムのインポートのサポートが改善されました。また、これらのサービスプロバイダーと互換性のあるフローステップを含むプログラムのインポートも可能です。

* **Munchkin — 拡張されたリンクトラッキング**:追跡のサポートを拡張 `tel` および `mailto` Munchkin とのリンクを使用して、拡張された一連の Web 動作を追跡します。

* **Webhook カスタムヘッダーの表示**:Webhook カスタムヘッダーが、可視性を高めるために、管理者/「Webhook」タブに表示されるようになりました。

* **CAPTCHA**:フォーム送信の有効性の評価 [reCAPTCHA v3 の使用](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target=&quot;_blank&quot;} で受信フォームトラフィックにスコアを付けます。 疑わしいボットトラフィックを自動的に除外、強制隔離、削除するマーケティングワークフローを構築します。

* **フォームを承認する権限**:フォームに対する変更を他の Design Studio アセットと合わせて承認できるデザイナーを制御する新しい権限。 これにより、他のデザイナーは、承認権限を持つユーザーがフォームをレビューしなくても、変更をフォームにプッシュできなくなります。

* **匿名結合後は常にキャンペーン再生を実行する**:匿名のリードマージはキャンペーン再生の前に発生するので、匿名キャンペーン再生がおこなわれると、カスタムフィールドフィルターは確実に動作します。

## マーケティングデータ環境 {#marketing-data-environment}

* **カスタムオブジェクト「使用者」フィールドの UI 切り捨てを修正しました**:「使用中」のカスタムオブジェクトフィールドを識別しやすくなり、必要に応じてカスタムオブジェクトからフィールドを削除できます。

## API の強化 {#api-enhancements}

* **一括プログラムメンバー抽出 API の新しいフィルタリング機能**:抽出したデータセットを絞り込むには、プログラムメンバーシップのステータス、updatedAt、cadence または exhusted コンテンツでフィルタリングします。

## Sales Insight {#sales-insight}

![（星印）](assets/yellow-star.png)

* **[Sales Insight と Dynamic Chat の統合](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target=&quot;_blank&quot;}**:Sales Insight パネルで Dynamic Chat のアクティビティを表示し、この新しいデータポイントを見込みの取り組みで活用します。

## お知らせ {#announcements}

**_製品リリースウェビナー_**

[2022年6月および8月の Marketo Engage リリースウェビナー](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target=&quot;_blank&quot;}
