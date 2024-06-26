---
description: Agent Management - Marketo ドキュメント – 製品ドキュメント
title: エージェント管理
feature: Dynamic Chat
exl-id: 151d8cf2-a5b7-43c4-8418-cc22252108b2
source-git-commit: 5aaf7081bbe96ff49753a7e142b0f3b38a70ea10
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 9%

---

# エージェント管理 {#agent-management}

Agent Management で、Dynamic Chatインスタンス内のエージェントのリストを表示し、チームを管理し、フォールバックルールを設定します。

![](assets/agent-management-1.png)

## エージェント {#agents}

このタブには、Dynamic Chatインスタンス内のすべてのエージェントが一覧表示され、名前、メールアドレス、ライブチャットステータスなどの情報が含まれます。

![](assets/agent-management-2.png)

>[!NOTE]
>
>代理人は表示されません _のみ_ 追加された？ Adobe Admin Console に追加してから、ここに表示されるまでに最大 2 時間かかる場合があります。

## チーム {#teams}

管理者は、エージェントのチームを作成して、特定の販売エージェントのグループへのルーティングを容易にすることができます。

>[!AVAILABILITY]
>
>Teams にアクセスするにはDynamic Chatプライムサブスクリプションが必要です。 詳しくは、アドビのアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

![](assets/agent-management-3.png)

### チームの作成 {#create-a-team}

1. クリック **+ チームを作成**.

   ![](assets/agent-management-4.png)

1. チームに名前を付けます。

   ![](assets/agent-management-5.png)

1. 「」をクリックします **エージェントの追加** ドロップダウンから目的のエージェントを選択します。

   ![](assets/agent-management-6.png)

1. 「**作成**」をクリックします。

   ![](assets/agent-management-7.png)

## フォールバックルール {#fallback-rules}

### 会議のフォールバック {#meeting-fallback}

標準（システム） メッセージを選択するか、ミーティング予約が利用できないときに訪問者に表示するカスタム メッセージを作成します。

![](assets/agent-management-8.png)

### ライブチャットフォールバック {#live-chat-fallback}

標準（システム）メッセージを選択するか、訪問者がライブチャットを使用できないときに確認できるカスタムメッセージを作成します。

![](assets/agent-management-9.png)

>[!NOTE]
>
>の選択 **会議予約オプションを含める** チェックボックスをオンにすると、ライブチャットに使用できるエージェントがない場合に、チャット訪問者が会議を予約できるようになります。

>[!TIP]
>
>カスタムメッセージを作成する際に、フォントのスタイル設定、リンクの使用、絵文字の挿入を行うことができます。 `:)`
