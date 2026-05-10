---
description: Marketo ランディングページに会話フローを埋め込む方法を説明します。 訪問者はフォームに入力することなく、Dynamic Chatでミーティングのスケジュールを設定できます。
title: 対話型フローランディングページの使用
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 689773f0d6f87b65d5299ecc11f3de11f7e66775
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 2%

---

# 対話型フローランディングページの使用{#use-a-conversational-flow-landing-page}

Dynamic Chat会話フローをMarketo Engageランディングページに直接埋め込むことで、訪問者はフォームに入力したりチャットボットと対話したりすることなく、Dynamic Chatを通じてミーティングをスケジュールすることができます。

>[!PREREQUISITES]
>
>**会議予約** カードのみを含むシンプルな[会話フロー](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-conversational-flow.md)を作成します。

## ガイド付きランディングページ {#guided-landing-pages}

ガイド付きランディングページ テンプレートに次のコードを埋め込みます：`<div class="mktoConversation" id="exampleConversation" mktoName= "Example Conversation"></div>`。

ガイド付きランディングページテンプレートをエディターで開き、会話フローのプレースホルダーを選択します。

「会話フロー」ドロップダウンをクリックし、手順1で作成したCFを選択します。

配信タイプは常に&#x200B;**インライン**&#x200B;のままにします。 「**挿入**」をクリックします。

入力したばかりの会話フローは、右側に要素として表示されます。

スクリーンショット

>[!NOTE]
>
>現時点では、会話フローはメインプレビューウィンドウに表示されません。

## フリーフォームのランディングページ {#free-form-landing-pages}

テキスト

STEVE MEETINGからのメモ

ガイド付きlp、テンプレート用の新しいdiv id、変換フローを選択

freeform lp、bring over icon – 注意事項：メモを追加 – cfをエディターに配置すると、プレビューが表示されない（プレースホルダーも表示されない） – 「プレビューが表示されない」 – サイドバーにcfがページにあることが表示されます – ガイド付きlpは要素としてリストします – 説明する際に「現時点で」を使用 – 機能が公開されるのは22週目の可能性があります
