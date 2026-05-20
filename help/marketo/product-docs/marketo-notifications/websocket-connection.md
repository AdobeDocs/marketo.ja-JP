---
description: 「Websocket Connectionを確立できません」という通知を受け取ったMarketo Engage ユーザーの通知の詳細
title: 通知 - Websocket 接続
hide: true
exl-id: 00c754f8-3850-4209-803d-5cdb108dc6dc
TQID: https://experienceleague.adobe.com/NpcRnxQPi03CF8z77Urrfs2P2phkuRbh2pd5J1UquFk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 123
ht-degree: 86%

---

# 通知：Websocket 接続 {#notification-websocket-connection}

このドキュメントは、Marketo インスタンスで次の通知を受け取った Marketo Engage ユーザを対象としています。`"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are currently connected to. Please work with your IT Team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

お客様またはお客様の組織が使用しているファイアウォールまたはプロキシサーバー設定に制限が設けられている場合、お客様またはネットワーク管理者は、Adobe Marketo Engage が期待通りに動作するように、特定のドメインおよび IP アドレス範囲を許可する必要が生じる場合があります。

Marketo サポートは、以下のプロトコルの実装については対応できません。 サポートが必要な場合は、このドキュメントを IT チームと共有してください。 IT チームが許可リストを使用して web アクセスを制限している場合は、次のドメイン（アスタリスクを含む）を追加して、すべての Marketo リソースと WebSocket を許可するよう依頼してください。

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
