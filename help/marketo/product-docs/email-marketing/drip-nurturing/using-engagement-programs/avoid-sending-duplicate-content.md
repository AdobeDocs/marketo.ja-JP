---
unique-page-id: 10096409
description: エンゲージメントプログラムでメールの重複を防止または許可するシナリオについて説明します。 繰り返しを避けるために、プログラムメンバーシップとCEE ルールを使用します。
title: 重複コンテンツ送信の回避
exl-id: fd7118e8-6e34-4973-8aa5-effb774447fd
feature: Engagement Programs
TQID: 'https://experienceleague.adobe.com/vJ0HguG6ad182v-Jkf-0DF6zAosaJG5B-me3ghxnYIM'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: fc5011cf-5b46-40b1-a5de-d7f042f85633
    internal-label: Engagement programs
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 57%
---
# 重複コンテンツ送信の回避 {#avoid-sending-duplicate-content}

エンゲージメントプログラムで同じメッセージが 2 回送信されるのを防ぐために考慮すべき 7 つのシナリオと結果を次に示します。

## シナリオ {#scenarios}

| メールの送信元 | 人物 | 人物はメールを受け取る |
|---|---|---|
| 個別のスタンドアロンのデフォルトプログラム内のキャンペーン | デフォルトプログラムのメンバーでない | はい |
| 個別のスタンドアロンのデフォルトプログラム内のキャンペーン | デフォルトプログラムのメンバー | いいえ |
| **same** CEE プログラム内のキャストからトリガーされるデフォルトプログラム内のキャンペーン | デフォルトプログラムのメンバー | いいえ |
| **same** CEE プログラム内のキャストからトリガーされるデフォルトプログラム内のキャンペーン | デフォルトプログラムのメンバーでない | はい |
| **different** CEE プログラム内のキャストからトリガーされるデフォルトプログラム内のキャンペーン | デフォルトプログラムのメンバー | いいえ |
| **different** CEE プログラム内のキャストからトリガーされるデフォルトプログラム内のキャンペーン | デフォルトプログラムのメンバーでない | はい |
| スマートストリームを使用する&#x200B;**異なる** CEE プログラム | 両方の CEE プログラムのメンバー | いいえ |
