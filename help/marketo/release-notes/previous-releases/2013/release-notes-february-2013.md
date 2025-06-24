---
unique-page-id: 2951103
description: リリースノート - 2013年2月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2013年2月
exl-id: 9adfa676-09ea-497a-bcce-42300848b9d8
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 46%

---

# リリースノート：2013年2月 {#release-notes-february}

2 月のリリースには、強い要望がある機能や、[!DNL Apple Safari] のサポート、その他の小規模な機能強化が含まれています。

## [!DNL Apple Safari] の公式サポート {#official-support-for-apple-safari}

Macおよび [!DNL Windows] 用の [!DNL Apple Safari] の最新バージョンは、Marketo Lead Management での使用が完全にサポートされています。 メモ：iOSの [!DNL Safari] は完全な互換性はありません。

## Web フックの機能強化 {#webhooks-enhancements}

Webhook は、URL/ペイロード内のトークンをエスケープするように強化され、サードパーティシステムからの XML/JSON 応答を解析することでMarketoのリードフィールドを更新することもできます（[!DNL Spark SMB Edition] では利用できません）。

## 更新されたSOAP API エンドポイント {#updated-soap-api-endpoint}

推奨のSOAP API エンドポイントが更新されました。このエンドポイントについては、[!UICONTROL  管理者 ]/SOAP API を参照してください。 この新しいエンドポイントを使用するには、呼び出しを更新してください。古いエンドポイントに対する API 呼び出しは非推奨ですが、引き続き機能します。（SOAP API は [!DNL Spark SMB Edition] では使用できません）

## [!DNL Facebook] タブのモバイルサポート {#mobile-support-for-facebook-tabs}

Marketoから公開された [!DNL Facebook] タブは、モバイルデバイスを検出し、ランディングページにルーティングします。 これにより、タブがサポートされていない（[!DNL Spark]、[!DNL Standard]、[!DNL Select SMB Editions] および [!DNL Marketo Social Marketing] で利用可能な）モバイルデバイスで [!DNL Facebook] ユーザーが適切なコンテンツを取得できるようになります。

## 準備中：複数モデルのサポート {#coming-soon-support-for-multiple-models}

アドビは、コミュニティでの RCA に対するアイデアとして得票数が最も多かった、複数の収益サイクルモデルを将来のリリースでサポートしようと取り組んでいます。このリリースでは、モデルとステージの選択をサポートする[スマートリストフィルターやフローステップへの選択肢の追加](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/find-all-leads-in-a-revenue-cycle-model.md)など、いくつかの変更が加えられています。また、「スマートリストリードグリッド」タブから「リード収益ステージ」フィールドと「リード収益サイクルモデル」フィールドを移動します。
