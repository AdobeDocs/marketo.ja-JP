---
description: Notification - Websocket Connection - Marketo ドキュメント – 製品ドキュメント
title: 通知 – Websocket 接続
hide: true
hidefromtoc: true
exl-id: 00c754f8-3850-4209-803d-5cdb108dc6dc
source-git-commit: eb3e7983f7521d025dff1f5d79b8caeaeb0f622c
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 33%

---

# 通知：Websocket 接続 {#notification-websocket-connection}

このドキュメントは、Marketo インスタンスで次の通知を受け取ったMarketo Engageユーザーを対象としています：`"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are currently connected to. Please work with your IT Team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

お客様またはお客様の組織が制限的なファイアウォールまたはプロキシサーバー設定を使用している場合、お客様またはネットワーク管理者は、Adobe Marketo Engage が期待通りに動作するように、特定のドメインおよび IP アドレス範囲を許可する必要が生じる場合があります。

Marketo サポートは、以下のプロトコルの実装を支援するように設定されていません。 サポートが必要な場合は、このドキュメントを IT チームと共有してください。 許可リストを使用して web アクセスを制限する場合は、すべてのMarketo リソースと web ソケットを許可するために、次のドメイン（アスタリスクを含む）を追加するように依頼します。

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
