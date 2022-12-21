---
unique-page-id: 2951103
description: リリースノート - 2013年2月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2013年2月
exl-id: 9adfa676-09ea-497a-bcce-42300848b9d8
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 100%

---

# リリースノート：2013年2月 {#release-notes-february}

2月のリリースには、要望が多かった機能、Apple Safari のサポートおよびその他の小規模な機能強化が含まれています。

## Apple Safari に対する正式なサポート {#official-support-for-apple-safari}

Mac 版 Apple Safari および Windows 版の最新バージョンでは、Marketo リード管理での使用が完全にサポートされています。注釈：iOS 上の Safari は完全には互換していません。

## Web フックの機能強化 {#webhooks-enhancements}

Web フックは、URL／ペイロード内のトークンをエスケープするように拡張され、サードパーティシステムからの XML／JSON 応答を解析することで、Marketo リードフィールドを更新することもできます（Spark SMB エディションでは利用できません）。

## SOAP API エンドポイントの更新 {#updated-soap-api-endpoint}

優先する SOAP API エンドポイントが更新されました（管理／SOAP API に表示されます）。この新しいエンドポイントを使用するには、呼び出しを更新してください。古いエンドポイントに対する API 呼び出しは非推奨ですが、引き続き機能します。（Spark SMB エディションでは SOAP API は使用できません）

## Facebook タブのモバイルサポート {#mobile-support-for-facebook-tabs}

Marketo から公開された Facebook タブは、モバイルデバイスを検出してランディングページにルーティングします。これにより、Facebook タブがサポートされていないモバイルデバイス（Spark、Standard、Select SMB エディションおよび Marketo ソーシャルマーケティングで利用可能）で適切なコンテンツをユーザーが取得できます。

## 準備中：複数モデルのサポート {#coming-soon-support-for-multiple-models}

アドビは、コミュニティでの RCA に対するアイデアとして得票数が最も多かった、複数の収益サイクルモデルを将来のリリースでサポートしようと取り組んでいます。このリリースでは、モデルとステージの選択をサポートする[スマートリストフィルターやフローステップへの選択肢の追加](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/find-all-leads-in-a-revenue-cycle-model.md)など、いくつかの変更が加えられています。また、「スマートリストリードグリッド」タブから「リード収益ステージ」フィールドと「リード収益サイクルモデル」フィールドを移動します。
