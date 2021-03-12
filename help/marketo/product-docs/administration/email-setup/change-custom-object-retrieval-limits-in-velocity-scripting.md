---
description: Velocityスクリプティング — Marketto Docs — 製品ドキュメントでのカスタムオブジェクト取得制限の変更
title: Velocityスクリプティングでのカスタムオブジェクト取得制限の変更
translation-type: tm+mt
source-git-commit: cfefff241b34571b9778cbd827f45d1b468d121e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---


# Velocityスクリプティング{#change-custom-object-retrieval-limits-in-velocity-scripting}でのカスタムオブジェクト取得制限の変更

Velocityスクリプトを使用して電子メールでカスタムオブジェクトデータを表示する場合、この機能はユーザーにとって役立つ場合があります。 デフォルトでは、Velocityスクリプトから10個の親カスタムオブジェクトにアクセスできます。 詳細情報にアクセスする必要がある場合は、以下を参照してください。

## 速度{#what-is-velocity}とは

[Apache Velocity](https://velocity.apache.org/)は、HTMLコンテンツのテンプレート化とスクリプティングを行うために設計された、Javaに基づいて構築された言語です。Marketorは、[スクリプティングトークン](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)を使用して、電子メールのコンテキストでMarketorを使用できます。 特に、カスタムオブジェクトに保存されたデータにアクセスできます。

リードまたは連絡先に直接接続されているが、第3レベルのカスタムオブジェクトではない親および子のカスタムオブジェクトを参照できます。 各カスタムオブジェクトについて、個人または連絡先ごとに最も新しく更新された10個のレコードが実行時に使用でき、最も新しい(0)～最も古い(9)の順に並べられます。

## 制限の変更方法{#how-to-change-the-limit}

1. **管理者**&#x200B;セクションに移動します。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. 「**電子メール**」をクリックします。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. 「Custom Object Retrieval Limits」テーブルで、新しい親取得制限を入力し、「**変更の保存**」をクリックします。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>親の取得制限の値は、10 ～ 100の範囲にする必要があります。 子の取得制限は自動的に設定されます。 これは、1,000を親の取得制限で割って行います。 例えば、親の制限を50に設定した場合、子の制限は20になります(1000÷ 50 = 20)。

甘い！ Velocityスクリプトから、より多くのカスタムオブジェクトにアクセスできるようになりました。
