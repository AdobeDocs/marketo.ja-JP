---
description: Adobe Experience Cloudからのオーディエンスの同期 —Marketoドキュメント — 製品ドキュメント
title: Adobe Experience Cloudからのオーディエンスの同期
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# Adobe Experience Cloudからのオーディエンスの同期{#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>MarketoインスタンスのHIPAA対応の展開では、この統合を使用できません。

>[!PREREQUISITES]
>
>[Adobe Experience Cloudオーディエンス共有の設定](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-experience-cloud-audience-sharing.md)

## オーディエンスの同期方法{#how-to-sync-an-audience}

1. 「マイMarketo」で、**データベース**&#x200B;タイルをクリックします。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. 「**新規**」ドロップダウンをクリックし、「Experience Cloudオーディエンス&#x200B;**と同期」を選択します。**

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. 「**オーディエンスライブラリフォルダー**」ドロップダウンをクリックし、目的の接触チャネルーフォルダーを選択します。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. **オーディエンス名**&#x200B;を選択します。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. 宛先に対しては、既存のリストを選択するか、新しい名前を入力できます。 この例では、新しいものを作成します。 完了したら「**同期**」をクリックします。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. 「**OK**」をクリックします。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## FAQ {#faq}

**cookieの同期はどのように行われますか。**

Marketoのmunchkin.jsは、Marketo購読でcookie同期が有効になっている場合、統合の設定時に指定したAdobeIMS組織のAdobeECIDを取得して保存し、これらのECIDを対応するMarketocookie識別子に一致させようとします。 これにより、Marketoの匿名ユーザープロファイルは、AdobeECIDを使用してより多くの情報を得ることができます。

匿名ユーザープロファイルをリードプロファイルに関連付けるには、さらに手順が必要です。リードユーザーは、テキスト形式の電子メールを使用して識別されます。 [の正確な動作は](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md)に記載されています。

**MarketoのリストサイズとAdobeのサイズが異なるのはなぜですか。**

また、ECID cookie IDをMarketoの既知のユーザーに関連付けることができない場合、ユーザーは同期されません。

**これは1回限りの同期ですか？**

同期を開始する必要があるのは1回だけです。 その後、レコードは自動的に同期されます。 最初の同期には最大24時間かかる場合があります。今後、新しいレコードは2 ～ 3時間で同期されます。
