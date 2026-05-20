---
description: Dynamic ChatのAgent Managementについて説明します。 エージェントの表示、チームの管理、フォールバックルールの設定、ミーティングやライブチャットの割り当て方法の制御を可能にします。
title: エージェント管理
feature: Dynamic Chat
exl-id: 151d8cf2-a5b7-43c4-8418-cc22252108b2
TQID: https://experienceleague.adobe.com/WZgOsCc5-8oEKLPhj6ziYMIhrYKHxHjrqhLp73mirSU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 362
ht-degree: 66%

---

# エージェント管理 {#agent-management}

エージェント管理では、Dynamic Chat インスタンスのエージェントのリストを表示し、チームを管理し、フォールバックルールを設定します。

![](assets/agent-management-1.png)

## エージェント {#agents}

このタブには、Dynamic Chat インスタンスのすべてのエージェントがリストされ、名前、メールアドレス、ライブチャットのステータスなどの情報が含まれます。

![](assets/agent-management-2.png){width="800" zoomable="yes"}

>[!NOTE]
>
>最近追加したエージェントがここに表示されない場合、Adobe Admin Consoleで追加してから最大2時間かかる場合があります。

## チーム {#teams}

管理者は、エージェントのチームを作成して、特定のセールスエージェントのグループへのルーティングを簡単に行うことができます。

>[!AVAILABILITY]
>
>チームにアクセスするには、Dynamic Chat Prime サブスクリプションが必要です。 詳しくは、アドビのアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

![](assets/agent-management-3.png)

### チームの作成 {#create-a-team}

1. 「**+ チームを作成**」をクリックします。

   ![](assets/agent-management-4.png)

1. チームに名前を付けます。

   ![](assets/agent-management-5.png)

1. **エージェントを追加**&#x200B;ドロップダウンをクリックし、目的のエージェントを選択します。

   ![](assets/agent-management-6.png)

1. 「**作成**」をクリックします。

   ![](assets/agent-management-7.png)

## フォールバックルール {#fallback-rules}

### ミーティングのフォールバック {#meeting-fallback}

ミーティング予約が利用できない場合に訪問者に表示される標準（システム）メッセージを選択するか、カスタムメッセージを作成します。

![](assets/agent-management-8.png)

### ライブチャットのフォールバック {#live-chat-fallback}

ライブチャットが利用できない場合に訪問者に表示される標準（システム）メッセージを選択するか、カスタムメッセージを作成します。

![](assets/agent-management-9.png)

>[!NOTE]
>
>* 「_ミーティング予約オプションを含める_」チェックボックスをオンにすると、ライブチャットに対応できるエージェントがいない場合、チャット訪問者にはミーティングを予約するオプションが提供されます。
>
>* **ライブチャットカードとしてのカスタムルール／チームの場合**：エージェントの確認中に、エージェントが使用できない場合や接続できない場合は、「使用可能なエージェント」（ストリームに配置されたルーティングロジック／ルールに関係なく、その時点で使用可能なすべてのエージェント）を試すためにラウンドロビンにフォールバックします。

>[!TIP]
>
>カスタムメッセージを作成する場合、フォントのスタイルを設定したり、リンクを使用したり、絵文字を挿入したりできます。

## 設定 {#settings}

### 同時ライブチャット制限 {#concurrent-live-chat}

エージェントが一度に実行できる同時アクティブチャットの数を設定します。 1 ～ 10の範囲で設定できます。

![](assets/agent-management-10.png)

### 訪問者の待機時間の制限 {#visitor-wait-time}

訪問者がフォールバックメッセージを受信するまでに、訪問者がライブエージェントに接続されるのを待つ最大時間（秒単位）を制御します。 10 ～ 500秒の範囲で設定できます。

![](assets/agent-management-11.png)
