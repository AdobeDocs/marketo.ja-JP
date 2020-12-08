---
unique-page-id: 8783322
description: Microsoft Dynamics Syncの検証 — Marketto Docs — 製品ドキュメント
title: Microsoft Dynamics同期の検証
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---


# Microsoft Dynamics同期の検証 {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Dynamics SyncでMulti-Factor Authentication(MFA)が有効になっている場合、DynamicsがMarketoと正しく同期されるように、これを無効にする必要があります。 詳しくは、マー [ケティング担当者にお問い合わせください](http://nation.marketo.com/community/support_solutions)。

## マーケティングでの検証の同期の実行 {#run-validate-sync-in-marketo}

同期の検証ツールを実行して、Microsoft Dynamics SyncとMarketorの最終的な接続を確立する前に、Microsoft Dynamics Syncが正しく設定されていることを確認することが非常に重要です。 このプロセスでは、問題が存在する場所を特定する7つの設定手順のチェックリストが生成されます。 これらが正しく行われたことを確認すると、後で多くの時間を節約できます。

1. 「 **管理者** 」タブをクリックし、「統合」領域の「 **Microsoft Dynamics** 」リンクをクリックします。

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. 「 **Microsoft**」を選択します。

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. 「 **同期セットアップの** 検証」タブをクリックします。

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. ユーザー名、パスワード、URLを入力します（クライアントIDとクライアントシークレットはオプションです）。 終了したら **「次へ** 」をクリックします。

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >以前に同期したことがある場合、左のツリーの **CRM** は **Microsoft Dynamics**&#x200B;を読み取り、上記のフォームのデータが事前に入力されている可能性があります。

1. すべてが問題ない場合、同期の検証では、緑色のチェックマーク ![— がいっぱいのチェックリストが生成され](assets/check.png)ます。

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. 「 ![— 」が表示された場合](assets/delete.png)は、その手順に問題があります。 問題を特定して修正するには、 [「Dynamics検証の同期の問題を](validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) 修正」を参照してください。 次に、同期の検証手順を再実行して、上の画像のような結果にします。

   >[!CAUTION]
   >
   >現在、Marketo Dynamics Syncのサンドボックス更新をサポートしていません。 Dynamics CRMサンドボックスを更新する必要がある場合は、新しいMarketo Sandboxが必要になります。 詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

>[!NOTE]
>
>**関連記事**
>
>[Dynamics検証の同期の問題を修正](validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)

