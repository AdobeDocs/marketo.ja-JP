---
description: Marketo AI権限を有効にする方法、組織ルールを設定する方法、統合や通知などの設定を管理する方法について説明します。
title: 設定と設定
exl-id: faf642a1-25f0-4566-b35d-074b003835ed
source-git-commit: 7e869a7a66badbb274355a676d9950068bb8b68e
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 4%

---

# 設定と設定 {#settings-setup}

権限を有効にし、設定エリアを使用して接続の詳細を表示し、組織ルールを定義し、統合と通知を設定する方法を説明します。

>[!AVAILABILITY]
>
>この機能は限定的に利用できます。 アクセスをリクエストするには、[このフォーム ](https://forms.cloud.microsoft/Pages/ResponsePage.aspx?id=Wht7-jR7h0OUrtLBeN7O4Y-uSf63sAxCmWyqMJg8eMFUMVZSVExSNDA3T0I4SEcwRDFSVTBGWU01Uy4u&origin=QRCode){target="_blank"}に入力してください。 サブスクリプションのMunchkin IDの準備が整っていることを確認します。

>[!PREREQUISITES]
>
>この機能を使用するには、まず[Core Gen-AI条件と補足条件](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}に同意する必要があります。 詳しくは、アカウントマネージャーにお問い合わせください。

## 権限と役割 {#permission-and-role}

_Marketo AI_&#x200B;へのアクセス権限と&#x200B;_Marketo AI User_&#x200B;のロールがあり、管理者は&#x200B;**Marketo AI**&#x200B;機能にアクセスできるユーザーをより詳細に制御できます。 権限はロールレベルで割り当てられます。 _Marketo AI ユーザー_ ロールには、デフォルトで有効になっている&#x200B;_Marketo AI_&#x200B;へのアクセス権限が付与されています。

>[!IMPORTANT]
>
>_Marketo AI_&#x200B;へのアクセス権限は、すべてのロールに対してデフォルトで有効になっていません。 詳しくは、以下の表を参照してください。

| 役割 | デフォルトステータス |
| --- | --- |
| 管理 | 有効 |
| アドビ製品管理者 | 有効 |
| マーケティングユーザ | 無効 |
| 標準ユーザー | 利用できません |
| Marketo AI ユーザー | 有効 |
| カスタム役割 | 無効 |

### Marketo AI権限へのアクセス {#access-marketo-ai-permission}

次の手順に従って、まだ有効になっていない適格なロールに対して&#x200B;_Marketo AI_&#x200B;へのアクセスを有効にします。

1. マイMarketoで、**管理者**、**ユーザーと役割**&#x200B;の順にクリックします。

   ![](assets/settings-setup-1.png)

1. 「_役割_」タブで、目的の役割を選択し、**役割を編集**&#x200B;をクリックします。

   ![](assets/settings-setup-2.png)

1. 下にスクロールして「_Marketo AIにアクセス_」チェックボックスをオンにし、**保存**&#x200B;をクリックします。

   ![](assets/settings-setup-3.png)

   >[!NOTE]
   >
   >これらの同じ手順を使用して、**実行**&#x200B;で「_Marketo AIにアクセス_」チェックボックスをオンにして、権限を削除できます。

### Marketo AIのユーザーロール {#marketo-ai-user-role}

次の手順に従って、特定のユーザーを&#x200B;_Marketo AI User_ ロールに割り当てます。

>[!NOTE]
>
>このロール **のみ**&#x200B;には、_アクセス Marketo AI_&#x200B;権限が含まれています。

1. マイMarketoで、**管理者**、**ユーザーと役割**&#x200B;の順にクリックします。

   ![](assets/settings-setup-4.png)

1. 目的のユーザーを選択し、**ユーザーの編集**&#x200B;をクリックします。

   ![](assets/settings-setup-5.png)

1. _役割とワークスペース_&#x200B;で、_Marketo AI User_ チェックボックスを選択します。 複数のワークスペースがある場合は、**+**&#x200B;署名ドロップダウンで、アクセスを取得するワークスペースを指定できます。 終了したら「**保存**」をクリックします。

   ![](assets/settings-setup-6.png)

### カスタム役割 {#custom-role}

また、[新しいロール ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"}を作成して権限をカスタマイズし、_必要な他のロールと共に_ Marketoにアクセスし、[そのロール ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"}を特定のユーザーに割り当てるオプションもあります。

## 設定 {#settings}

1. マイMarketoで、**Marketo AI** タイルをクリックします。

   ![](assets/settings-setup-7.png)

1. 歯車アイコンをクリックします。

   ![](assets/settings-setup-8.png)

### 接続 {#connection}

このタブには編集可能なフィールドが含まれていません。 Munchkin IDやIMS組織などのアカウント情報が表示されます。

![](assets/settings-setup-9.png)

### 組織ルール {#organizational-rules}

Marketo Engage アセットを作成または修正する際に、Marketo AIが従う組織ガイドラインと制約を定義します。

![](assets/settings-setup-10.png){width="800" zoomable="yes"}

>[!NOTE]
>
>ルールは、YAML frontmatterでMarkdown形式を使用します。 グローバルルールはすべてのワークスペースに適用されます。 Workspace ルールは、グローバル設定を上書きします。

### 統合（近日公開予定） {#integrations}

外部サービスおよびAPIへの接続を設定します。

_このタブはUIに表示されますが、まだ使用できません。 更新プログラム_&#x200B;を確認してください。

### 通知（近日リリース予定） {#notifications}

アラートの環境設定と通知チャネルを管理します。

_このタブはUIに表示されますが、まだ使用できません。 更新プログラム_&#x200B;を確認してください。
