---
unique-page-id: 9437340
description: Tealium タグマネージャーを使用した RTP の実装 — Marketo ドキュメント — 製品ドキュメント
title: Tealium タグマネージャーを使用した RTP の実装
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '219'
ht-degree: 100%

---

# Tealium タグマネージャーを使用した RTP の実装 {#implementing-rtp-using-tealium-tag-manager}

RTP タグを実装するには、次のインストール手順に従います。

1. Tealium タグマネージャーアカウントにログインします。

1. 「タグ」タブに移動し、タグマーケットプレイスの「その他」タブにある「Tealium カスタムコンテナタグ」を追加します。

1. 「タイトル」フィールドに、「**Marketo RTP**」と入力して「**完了**」をクリックします。

1. 変更を保存します。

   >[!NOTE]
   >
   >まだ新しいコンテナを公開する必要はありません。

1. プロファイルを保存したら、Tealium iQ コンソールの右上隅にある名前／メールアドレスをクリックします。

1. 管理者メニューの「アカウント管理者」で「**テンプレートを管理**」をクリックします。

1. ドロップダウンリストから「**Tealium カスタムコンテナ：Marketo RTP**」を選択して、タグテンプレートを開きます。

1. RTP アカウントにログインします。

1. 「アカウント設定」に移動します。

   >[!NOTE]
   >
   >サポートから既に JavaScript タグを受け取っている場合は、手順 11 に進みます。

1. ドメインで、該当するドメインを選択し、「**タグの生成**」をクリックします。

1. RTP JavaScript タグをコピーし、Tealium プロファイルテンプレートの「Start Tag Library Code」と「End Tag Library Code」の間に貼り付けます。

   >[!NOTE]
   >
   >**重要な手順**
   >
   >このファイルに配置するコードから `<!-- RTP tag -->` タグと `<!-- End of RTP tag -->` タグを削除します。
   >
   >このファイルに配置するコードから `<script type='text/javascript'>` タグと `</script>` タグを削除します。

1. 「**プロファイルテンプレートを保存**」をクリックすると、新しいプロファイルが公開されます。
