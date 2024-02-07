---
description: 通知 — Websocket 接続 — Marketoドキュメント — 製品ドキュメント
title: 通知 — Websocket 接続
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 10fe526c672867b93b54e99e492e59c0541c3f36
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 30%

---

# 通知：Websocket 接続 {#notification-websocket-connection}

この記事は、Marketo EngageのMarketoインスタンスで次の通知を受け取ったユーザー向けです。 `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are connected to now on March 3, 2024. Please work with your IT team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

お客様またはお客様の組織が制限的なファイアウォールまたはプロキシサーバー設定を使用している場合、お客様またはネットワーク管理者は、Adobe Marketo Engage が期待通りに動作するように、特定のドメインおよび IP アドレス範囲を許可する必要が生じる場合があります。

Marketoサポートは、以下のプロトコルの実装を支援するようには設定されていません。 サポートが必要な場合は、この記事を IT チームと共有してください。 を使用して Web アクセスを制限する場合許可リストに加えるは、次のドメイン（アスタリスクを含む）を追加して、すべてのMarketoリソースおよび Web ソケットを許可するように依頼します。

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
