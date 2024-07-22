---
unique-page-id: 8783322
description: Microsoft Dynamics 同期の検証 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 同期の検証
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 84%

---

# Microsoft Dynamics 同期の検証 {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Dynamics 同期で多要素認証（MFA）を有効にしている場合、Dynamics が Marketo と正しく同期するには、無効にする必要があります。詳しくは、[Marketo サポート ](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"} にお問い合わせください。

## Marketo で同期検証を実行する {#run-validate-sync-in-marketo}

同期の検証ツールを実行して、Microsoft Dynamics と Marketo の同期が正しく設定されていることを確認してから、同期の最終的な接続を確立することが非常に重要です。このプロセスでは、7 つのセットアップ手順のチェックリストが生成され、問題が存在する場所を特定します。これらが正しく行われたことを確認すると、後で多くの時間を節約できます。

1. **[!UICONTROL 管理者]** タブをクリックしてから、統合領域の **[!DNL Microsoft Dynamics]** リンクをクリックします。

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. 「**[!DNL Microsoft]**」を選択します。

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. 「**[!UICONTROL 同期設定の検証]**」タブをクリックします。

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. ユーザー名、パスワード、URL を入力します（クライアント ID とクライアントシークレットはオプションです）。終了したら「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >以前に同期したことがある場合、左側のツリーの **[!UICONTROL CRM]** が **[!DNL Microsoft Dynamics]** を読み取り、上記のフォームのデータが事前入力される可能性があります。

1. すべて問題ない場合、同期の検証で、すべてが緑のチェックマークがついたチェックリストが生成されます。![-](assets/check.png)

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. ![-](assets/delete.png) が表示された場合は、その手順に問題があります。詳しくは、[Dynamics 検証同期に対する問題の修正](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md){target="_blank"}を参照して、問題を特定して修正してください。次に、上記の画像のような結果になるまで同期検証手順を再実行します。

   >[!CAUTION]
   >
   >現在、Marketo Dynamics Sync のサンドボックス更新はサポートされていません。Dynamics CRM サンドボックスを更新する必要がある場合は、新しい Marketo サンドボックスが必要です。詳しくは、アドビアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

>[!MORELIKETHIS]
>
>[Dynamics 検証同期に対する問題の修正](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md){target="_blank"}
