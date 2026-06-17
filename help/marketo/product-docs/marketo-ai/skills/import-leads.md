---
description: リードの読み込みエージェントを使用して、CSVのアップロード、ビジネスルールの適用、フィールドのマッピング、リードのMarketo Engage データベースへの直接読み込みを行う方法について説明します。
title: リードの読み込み
exl-id: 6583b93c-71eb-4a07-b25d-11eca834a3ba
badge: Beta
source-git-commit: 408923e529bdfb2aa23f7d6acfb229cd7ee4c9d8
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 1%

---

# リードの読み込み {#import-leads}

フィールドマッピング機能を利用すれば、リードリストをMarketo Engageデータベースにインポートして重複を排除できます。

>[!AVAILABILITY]
>
>この機能は現在オープンベータ版です。 アクセスをリクエストするには、アカウントマネージャーにお問い合わせください。 また、[&#x200B; コア生成AIの利用条件および補足条件](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}に同意する必要があります。

## 使用方法 {#how-to-use}

1. マイMarketoで、**Marketo AI** タイルをクリックします。

   ![](assets/import-leads-1.png)

1. **リードの読み込み** エージェントをクリックします。

   ![](assets/import-leads-2.png)

   会話型AI画面が表示されます。 左側のペインには、ガイダンス、応答、使用可能なデータの正規化オプションが表示されます。

   ![](assets/import-leads-3.png)

1. リードの読み込みを開始するには、添付ファイルアイコンをクリックし、.CSV ファイルを介してアップロードします。

   ![](assets/import-leads-4.png)

1. 「リストの読み込み」と入力し、**送信**&#x200B;をクリックします。

   ![](assets/import-leads-5.png)

   リストがセンターコンソールでプレビューされます。

   ![](assets/import-leads-6.png)

1. 目的のビジネスルールを入力し、**送信**&#x200B;をクリックします。

   ![](assets/import-leads-7.png)

   結果はセンターコンソールに表示されます。

   ![](assets/import-leads-8.png)

   必要に応じて、追加のビジネスルールを入力します。

1. マッピングされたフィールドを表示するには、「**マッピング**」タブをクリックします。

1. フィールドが正しくマッピングされていない場合は、ここで修正します。

   ![](assets/import-leads-9.png)

1. リストを読み込む準備ができたら、「**Marketoに読み込み**」タブをクリックします。

1. 宛先フォルダーを選択し、名前を入力します。 各同意ボックスにチェックを入れ、**承認してMarketoに読み込む**&#x200B;をクリックします。

   ![](assets/import-leads-10.png)

読み込みが完了すると、検証概要が表示され、処理されたリード、失敗した行、警告が表示されます。

