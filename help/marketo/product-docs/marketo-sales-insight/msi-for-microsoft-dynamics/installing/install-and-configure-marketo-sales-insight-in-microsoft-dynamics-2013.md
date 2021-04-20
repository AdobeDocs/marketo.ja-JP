---
unique-page-id: 3571737
description: Microsoft Dynamics 2013 -Marketoドキュメント — 製品ドキュメントで、Marketo販売インサイトをインストールおよび構成します
title: Microsoft Dynamics 2013でのMarketo販売インサイトのインストールと構成
exl-id: 290db451-47a6-4cfa-a36f-bc12ef7d3482
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 1%

---

# Microsoft Dynamics 2013でのMarketo販売インサイトのインストールと構成{#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo・セールス・インサイトは、マーケティング・チームが持つ豊富なデータをセールス・チームに「窓口」として提供する素晴らしいツールです。 以下に、インストールおよび設定の方法を示します。

>[!PREREQUISITES]
>
>Marketoとマイクロソフトの統合を完了します。
>
>[お使いのバージョンのMicrosoft Dynamics CRMに適した](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) ソリューションをダウンロードしてください。

## ソリューションのインポート{#import-solution}

では、MarketoのSales InsightソリューションをMicrosoft Dynamicsにインポートする時間です。

1. **Microsoft Dynamics CRM**&#x200B;の下の&#x200B;**設定**&#x200B;をクリックします。

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. 「**設定**」で、「**カスタマイズ**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. 「**ソリューション**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >次に進む前に、既にMarketoをインストールし、設定しておく必要があります

1. 「**インポート**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. 新しいウィンドウで、**参照**&#x200B;をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. 上記でダウンロードしたソリューションを探して選択します。

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. 「**次へ**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. ソリューションがアップロードされます。 必要に応じて、パッケージの内容を表示できます。 「**次へ**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. チェックボックスをオンのままにして、「**読み込み**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. ログファイルは自由にダウンロードできます。 「**閉じる**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. やりましたね！解決策を今すぐ見てみましょう。 表示されていない場合は、画面を更新します。

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## MarketoとSales Insightを接続{#connect-marketo-and-sales-insight}

MarketoインスタンスをDynamicsのSales Insightに結び付けます。

>[!NOTE]
>
>管理者権限が必要です。

1. Marketoにログインし、**管理者**&#x200B;セクションに移動します。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 「**Sales Insight**」セクションで、「**Edit API Configuration**」をクリックします。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 後の手順で使用する&#x200B;**Marketoホスト**、**API URL**、**APIユーザーID**&#x200B;をコピーします。 任意の&#x200B;**API秘密キー**&#x200B;を入力し、「**保存**」をクリックします。

   >[!CAUTION]
   >
   >API秘密鍵にアンパサンド(&amp;)を使用しないでください。

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Sales Insightを機能させるには、次のフィールドをMarketoと同期して、_リードと連絡先_&#x200B;の両方を行う必要があります。
   >
   >* 優先順位
   >* 緊急度
   >* 相対スコア

   >
   >これらのフィールドのいずれかが見つからない場合は、Marketoに、見つからないフィールドの名前のエラーメッセージが表示されます。 この問題を修正するには、[この手順](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)を実行します。

1. Microsoft Dynamicsに戻り、**設定**&#x200B;に戻ります。

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. 「**設定**」で、「**MarketoAPI設定**」をクリックします。

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. 「**新規**」をクリックします。

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. 先ほどMarketoから取得した情報を入力し、[**保存**]をクリックします。

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## ユーザーアクセスの設定{#set-user-access}

最後に、特定のユーザーにMarketo販売インサイトへのアクセスを提供できます。

1. **設定**&#x200B;に移動します。

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. 「**ユーザー**」をクリックします。

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. Sales Insightへのアクセス権を付与するユーザーを選択し、**ロールの管理**&#x200B;をクリックします。

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. **Marketo販売インサイト**&#x200B;のロールを選択し、「**OK**」をクリックします。

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   お前は全部終わらなきゃ！ 最後に、テストを行うには、Dynamicsに、Marketoセールスインサイトにアクセスし、リードや連絡先を調べるユーザーとしてログインします。

   ![](assets/image2014-12-12-9-3a9-3a31.png)

これで、営業チームのMarketoセールス・インサイトの力を解除しました。

>[!MORELIKETHIS]
>
>[リード/接触レコードの星と炎の設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
