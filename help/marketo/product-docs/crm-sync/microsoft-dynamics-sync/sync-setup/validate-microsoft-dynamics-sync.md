---
unique-page-id: 8783322
description: Microsoft Dynamics同期の検証 —Marketoドキュメント — 製品ドキュメント
title: Microsoft Dynamics同期の検証
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---

# Microsoft Dynamics同期の検証{#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Dynamics SyncでMulti-Factor Authentication (MFA)が有効になっている場合、DynamicsがMarketoと正しく同期するには、これを無効にする必要があります。 詳しくは、[Marketoサポート](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。

## Marketoで同期の検証を実行{#run-validate-sync-in-marketo}

同期の検証ツールを実行して、Microsoft DynamicsとMarketoの同期が正しく設定されていることを確認してから、同期の検証ツールを実行することが非常に重要です。 このプロセスでは、問題が存在する場所を特定する7つの設定手順のチェックリストが生成されます。 これらが正しく行われたことを確認すると、後で多くの時間を節約できます。

1. [**管理者**]タブをクリックし、[統合]領域の[**Microsoft Dynamics**]リンクをクリックします。

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. 「**Microsoft**」を選択します。

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. 「**同期設定の検証**」タブをクリックします。

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. ユーザー名、パスワード、URLを入力します（クライアントIDとクライアントシークレットはオプションです）。 終了したら「**次へ**」をクリックします。

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >以前に同期したことがある場合、左のツリーの&#x200B;**CRM**&#x200B;は&#x200B;**Microsoft Dynamics**&#x200B;を読み取り、上記のフォームのデータが事前入力される場合があります。

1. すべてが問題ない場合、同期の検証では、緑色のチェックマークの入ったチェックリスト![—](assets/check.png)が生成されます。

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. ![—](assets/delete.png)が表示された場合は、その手順に問題があります。 [Dynamics検証の同期の問題を修正](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)を参照して、問題を特定し、修正してください。 次に、同期の検証手順を再実行して、上の画像のような結果にします。

   >[!CAUTION]
   >
   >現在、Marketoダイナミクス同期のサンドボックス更新をサポートしていません。 Dynamics CRMサンドボックスを更新する必要がある場合は、新しいMarketoサンドボックスが必要です。 詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

>[!MORELIKETHIS]
>
>[Dynamics検証の同期の問題を修正](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)
