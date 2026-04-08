---
description: Marketo AI権限を有効にする方法、組織ルールを設定する方法、統合や通知などの設定を管理する方法について説明します。
title: 設定と設定
hide: true
hidefromtoc: true
exl-id: d6f37214-65b9-48c1-bf9f-d64b4eda87b9
source-git-commit: e137d417f7ba9440b9d3d68a985fa38694e1c157
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 3%

---

# 設定と設定 {#settings-setup}

権限を有効にし、設定エリアを使用して接続の詳細を表示し、組織ルールを定義し、統合と通知を設定する方法を説明します。

## 権限 {#permissions}

Marketo AIにアクセスするには、管理者が最初にロール権限を有効にする必要があります。

1. マイMarketoで、**管理者**、**ユーザーと役割**&#x200B;の順にクリックします。

   ![](assets/settings-setup-1.png)

1. 「_役割_」タブで、目的の役割を選択し、**役割を編集**&#x200B;をクリックします。

   ![](assets/settings-setup-2.png)

1. 下にスクロールして「**AIを使用したビルドにアクセス**」チェックボックスを選択し、**保存**&#x200B;をクリックします。

   ![](assets/settings-setup-3.png)

## 設定 {#settings}

1. マイMarketoで、**AIでビルド** タイルをクリックします。

   ![](assets/settings-setup-4.png)

1. 歯車アイコンをクリックします。

   ![](assets/settings-setup-5.png)

### 接続 {#connection}

このタブには編集可能なフィールドが含まれていません。 Munchkin IDやIMS組織などのアカウント情報が表示されます。

![](assets/settings-setup-6.png)

### 組織ルール {#organizational-rules}

Marketo Engage アセットを作成または修正する際に、Marketo AIが従う組織ガイドラインと制約を定義します。

![](assets/settings-setup-7.png){width="800" zoomable="yes"}

>[!NOTE]
>
>ルールは、YAML frontmatterでMarkdown形式を使用します。 グローバルルールはすべてのワークスペースに適用されます。 Workspace ルールは、グローバル設定を上書きします。

### 統合（近日公開予定） {#integrations}

外部サービスおよびAPIへの接続を設定します。

_このタブはUIに表示されますが、まだ使用できません。 更新プログラム_&#x200B;を確認してください。

### 通知（近日リリース予定） {#notifications}

アラートの環境設定と通知チャネルを管理します。

_このタブはUIに表示されますが、まだ使用できません。 更新プログラム_&#x200B;を確認してください。
