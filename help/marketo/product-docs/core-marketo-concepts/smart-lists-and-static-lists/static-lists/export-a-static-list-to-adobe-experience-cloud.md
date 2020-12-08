---
unique-page-id: 37356194
description: 静的リストのAdobe Experience Cloudへのエクスポート — Marketto Docs — 製品ドキュメント
title: 静的リストのAdobe Experience Cloudへの書き出し
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 0%

---


# 静的リストのAdobe Experience Cloudへの書き出し {#export-a-static-list-to-adobe-experience-cloud}

>[!NOTE]
>
>MarketorインスタンスのHIPAA対応の展開では、この機能を使用できません。

>[!NOTE]
>
>**前提条件**
>
>[Adobe Experience Cloudオーディエンス共有の設定](http://docs.marketo.com/x/D4GMAg)

## サポートされる宛先アプリケーション {#supported-destination-applications}

* Adobe Advertising Cloud
* Adobe Analytics(**Adobe Audience Manager免許を持っている場合のみ** )
* Adobe Audience Manager
* Adobe Experience Manager
* Adobeリアルタイム顧客データプラットフォーム
* Adobe Target

## リストの書き出し方法 {#how-to-export-a-list}

1. Marketorで、エクスポートするリストを探して選択します。

   ![](assets/one.png)

1. 「 **リストアクション** 」ドロップダウンをクリックし、「Experience Cloudに **送信」を選択します**。

   ![](assets/two-1.png)

1. 「 **Audience Managerフォルダ** 」ドロップダウンをクリックし、Experience Cloud内の目的の保存先フォルダを選択します。

   ![](assets/three-1.png)

1. 新しいオーディエンスを作成するか、既存のフォルダを上書きするかを選択します（この例では、新しいを作成します）。 新しいオーディエンス名を入力し、「 **送信**」をクリックします。

   ![](assets/four.png)

1. 「 **OK**」をクリックします。

   ![](assets/five.png)

   >[!NOTE]
   >
   >オーディエンスのメンバーシップがAdobeに完全に設定されるまで、最大6 ～ 8時間かかる場合があります。

## 注意事項 {#things-to-note}

**Adobe Analyticsとの共有**

Adobe Audience ManagerとAdobe Analyticsの両方を所有するお客様の場合、この統合により、オーディエンスをMarketoからAdobe Analyticsのレポートスイートに共有できますが、これを有効にするにはAdobe Audience Managerで行う追加の設定手順がいくつかあります。 この設定方法の詳細については、Adobe Audience Managerのドキュメントを参照してください。 [https://docs.adobe.com/content/help/en/analytics/integration/audience-analytics/mc-audiences-aam.html](http://docs.adobe.com/content/help/en/analytics/integration/audience-analytics/mc-audiences-aam.html).

**Adobe Audience Managerのお客様の特徴使用**

Marketoでリストのエクスポートを開始すると、Adobe Audience Managerのインスタンスに次の変更が反映されています。

* エクスポートされたリスト内のすべてのリードに対して、Marketorは、リードのハッシュされた電子メールをCross-Device Identifierとして使用して、特性を記述します。 特性の名前は、エクスポート時に指定した宛先オーディエンス名と一致します。
* Marketoが管理しているすべてのECIDが、エクスポートされたリストのリードと一致するように、MarketorはECID Device Identifierを使用して特性を記述します。 特性の名前は、エクスポート時に指定した宛先オーディエンス名と一致します。
* また、ECID特性をセグメント化基準として使用し、Audience Managerインスタンスにセグメントを作成します。 セグメントの名前は、エクスポート時に指定した宛先オーディエンス名と一致します。

## FAQ {#faq}

**マーケティングツールのリストサイズがAdobeのサイズと異なるのはなぜですか。**

内部では、オーディエンス統合は、Marketo Munchkinのcookieと対応するAdobeECID cookieを同期することで機能します。 Marketorは、ECIDを同期したリードのメンバーシップデータのみを共有できます。 最良の結果を得るために、マーケティングの目的でトラッキングするすべてのページのAdobeの訪問者.jsトラッキングコードと並行して、Marketoのmunchkin.jsトラッキングスクリプトを読み込むことをお勧めします。

**cookieの同期はどのように行われますか。**

Marketo購読でCookieの同期が有効になっている場合、Marketoのmunchkin.jsは、統合の設定時に指定したAdobeIMS組織のAdobeECIDを取得して保存し、これらのECIDを対応するMarketoのCookie識別子に一致させようとします。 これにより、Marketorの匿名ユーザープロファイルは、AdobeECIDを使用して利用できるようになります。

匿名ユーザープロファイルをリードプロファイルに関連付けるには、さらに手順が必要です。リードユーザーは、テキスト形式の電子メールを使用して識別されます。 この機能については、以下で説明します。 [https://docs.marketo.com/display/public/DOCS/Tracking+Anonymous+Activity+and+People](http://docs.marketo.com/display/public/DOCS/Tracking+Anonymous+Activity+and+People).
