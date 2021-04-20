---
unique-page-id: 9437340
description: Tealium Tag Managerを使用したRTPの実装 —Marketoドキュメント — 製品ドキュメント
title: Tealium Tag Managerを使用したRTPの実装
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Tealium Tag Managerを使用したRTPの実装{#implementing-rtp-using-tealium-tag-manager}

RTPタグを実装するには、次のインストール手順に従ってください。

1. Tealium Tag Managerアカウントにログインします。

1. 「タグ」タブに移動し、タグマーケットプレイスの「その他」タブの下にある「カスタムコンテナタグ」を追加します。

1. 「タイトル」フィールドに&#x200B;**MarketoRTP**&#x200B;と入力し、「**完了**」をクリックします。

1. 変更を保存します。

   >[!NOTE]
   >
   >新しいコンテナをまだ公開する必要はありません。

1. プロファイルを保存したら、Tealium iQコンソールの右上隅にある名前/電子メールアドレスをクリックします。

1. [管理]メニューの[アカウント管理]で[**テンプレートの管理**]をクリックします。

1. **Tealium Customコンテナを選択：ドロップダウンリストからMarketoRTP**&#x200B;を呼び出し、タグテンプレートを開きます。

1. RTPアカウントにログインします。

1. 「アカウント設定」に移動します。

   >[!NOTE]
   >
   >サポートからJavaScriptタグを既に受け取っている場合は、手順11に進みます。

1. 「Domain」で、関連するドメインを探し、「**Generate Tag**」をクリックします。

1. RTP JavaScriptタグをコピーして、Teliumプロファイルテンプレート内の開始タグライブラリコードと終了タグライブラリコードの間に貼り付けます。

   >[!NOTE]
   >
   >**重要な手順**
   >
   >このファイルに配置するコードから`<!-- RTP tag -->`タグと`<!-- End of RTP tag -->`タグを削除します。
   >
   >このファイルに配置するコードから`<script type='text/javascript'>`タグと`</script>`タグを削除します。

1. **「プロファイルテンプレートを保存」をクリックし、新しいプロファイルを公開し** ます。
