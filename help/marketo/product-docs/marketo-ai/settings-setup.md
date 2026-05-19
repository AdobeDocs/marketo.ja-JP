---
description: Marketo AI権限を有効にする方法、組織ルールを設定する方法、統合や通知などの設定を管理する方法について説明します。
title: 設定と設定
badge: ベータ版
exl-id: faf642a1-25f0-4566-b35d-074b003835ed
source-git-commit: ff71b9e2a743056f8efd64d3debdf498ee3e43df
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 4%

---

# 設定と設定 {#settings-setup}

権限を有効にし、設定エリアを使用して接続の詳細を表示し、組織ルールを定義し、統合と通知を設定する方法を説明します。

>[!AVAILABILITY]
>
>この機能は限定的に利用できます。 サブスクリプションへのアクセスをリクエストするには、Adobe アカウントチーム（アカウントマネージャー）にお問い合わせください。

>[!PREREQUISITES]
>
>この機能を使用するには、まず[Core Gen-AI条件と補足条件](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}に同意する必要があります。 詳しくは、アカウントマネージャーにお問い合わせください。

## 権限と役割 {#permission-and-role}

AI _の権限を持つ_ アクセスのビルドと、AI ユーザー&#x200B;_の役割を持つ_ ビルドがあり、管理者はAI **機能を持つ** ビルドにアクセスできるユーザーをより詳細に制御できます。 権限はロールレベルで割り当てられます。 AI ユーザー&#x200B;_を使用したビルド_&#x200B;の役割には、デフォルトで有効になっている&#x200B;_AI_&#x200B;を使用したビルドへのアクセス権限が付与されています。

>[!IMPORTANT]
>
>AI _を使用した_ アクセスのビルド権限は、すべての役割に対してデフォルトで有効になっていません。 詳しくは、以下の表を参照してください。

| 役割 | デフォルトステータス |
| --- | --- |
| 管理 | 有効 |
| アドビ製品管理者 | 有効 |
| マーケティングユーザ | 無効 |
| 標準ユーザー | 利用できません |
| AI ユーザーによる構築 | 有効 |
| カスタム役割 | 無効 |

### AI権限を持ったビルドへのアクセス {#access-build-with-ai-permission}

次の手順に従って、AI _を使用して_ アクセス ビルドをまだ有効にしていない適格な役割に対して有効にします。

1. マイMarketoで、**管理者**、**ユーザーと役割**&#x200B;の順にクリックします。

   ![](assets/settings-setup-1.png)

1. 「_役割_」タブで、目的の役割を選択し、**役割を編集**&#x200B;をクリックします。

   ![](assets/settings-setup-2.png)

1. 下にスクロールして「_AIを使用してビルドにアクセス_」チェックボックスをオンにし、**保存**&#x200B;をクリックします。

   ![](assets/settings-setup-3.png)

   >[!NOTE]
   >
   >_AIを使用したビルドにアクセス_ チェックボックスをオンにして&#x200B;**実行**&#x200B;することで、同じ手順で権限を削除できます。

### AI ユーザーの役割で構築 {#build-with-ai-user-role}

次の手順に従って、特定のユーザーを&#x200B;_AI ユーザー付きビルド_&#x200B;の役割に割り当てます。

>[!NOTE]
>
>この役割&#x200B;**のみ**&#x200B;には、AI _権限を持つ_ アクセス ビルドが含まれています。

1. マイMarketoで、**管理者**、**ユーザーと役割**&#x200B;の順にクリックします。

   ![](assets/settings-setup-1.png)

1. 目的のユーザーを選択し、**ユーザーの編集**&#x200B;をクリックします。

   ![](assets/settings-setup-5b.png)

1. _役割とワークスペース_&#x200B;で、「_AI ユーザーで作成_」チェックボックスを選択します。 複数のワークスペースがある場合は、**+**&#x200B;署名ドロップダウンで、アクセスを取得するワークスペースを指定できます。 終了したら「**保存**」をクリックします。

   ![](assets/settings-setup-6b.png)

### カスタム役割 {#custom-role}

また、[新しい役割](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"}を作成し、その権限をカスタマイズして、_AIを使用してビルドにアクセス_&#x200B;を追加し、その他の任意の役割を[特定のユーザーに割り当てるオプションもあります。](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"}

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
