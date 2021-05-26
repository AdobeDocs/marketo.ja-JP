---
unique-page-id: 37356194
description: リストのAdobe Experience Cloudへの送信 — Marketoドキュメント — 製品ドキュメント
title: Adobe Experience Cloudへのリストの送信
exl-id: 770eefe1-05f9-409d-8e7c-b3f1e6ba8139
source-git-commit: c225facfb3fce2d9e03ca1db5aa1ce0fee4f686c
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 1%

---

# リストをAdobe Experience Cloudに送信{#send-a-list-to-adobe-experience-cloud}

>[!NOTE]
>
>MarketoインスタンスのHIPAA対応のデプロイメントでは、この機能を使用できません。

>[!PREREQUISITES]
[Adobe Experience Cloudオーディエンス共有のセットアップ](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-experience-cloud-audience-sharing.md)>
>

## サポートされる宛先アプリケーション{#supported-destination-applications}

* Adobe Advertising Cloud
* Adobe Analytics(Adobe Audience Managerライセンスを所有している場合は&#x200B;**のみ**)
* Adobe Audience Manager
* Adobe Experience Manager
* Adobeのリアルタイム顧客データプラットフォーム
* Adobe Target

## 静的リストの送信方法{#how-to-send-a-static-list}

静的リストは、静的リストに過ぎません。 手動で変更しない限り、Adobe Experience Cloudのリストは変更されません。

1. Marketoで、書き出すリストを探して選択します。

   ![](assets/send-a-list-to-adobe-experience-cloud-1.png)

1. **リストアクション**&#x200B;ドロップダウンをクリックし、「**Experience Cloudに送信**」を選択します。

   ![](assets/send-a-list-to-adobe-experience-cloud-2.png)

1. 「**Audience Managerフォルダー**」ドロップダウンをクリックし、Experience Cloudで目的の宛先フォルダーを選択します。

   ![](assets/send-a-list-to-adobe-experience-cloud-3.png)

1. 新しいオーディエンスを作成するか、既存のオーディエンスを上書きするかを選択します（この例では、新しいオーディエンスを作成します）。 新しいオーディエンス名を入力し、「**送信**」をクリックします。

   ![](assets/send-a-list-to-adobe-experience-cloud-4.png)

1. 「**OK**」をクリックします。

   ![](assets/send-a-list-to-adobe-experience-cloud-5.png)

   >[!NOTE]
   オーディエンスメンバーシップがAdobeに完全に入力されるまで、最大6 ～ 8時間かかる場合があります。

## 同期リストの送信方法{#how-to-send-a-synced-list}

リストの同期とは、Marketoでリストを更新するたびに、その変更がAdobe Experience Cloudのオーディエンスに自動的に同期されることを意味します。

1. Marketoで、同期するリストを探して選択します。

   ![](assets/send-a-list-to-adobe-experience-cloud-6.png)

1. **リストアクション**&#x200B;ドロップダウンをクリックし、「**Experience Cloudに送信**」を選択します。

   ![](assets/send-a-list-to-adobe-experience-cloud-7.png)

1. **オーディエンスライブラリフォルダー**&#x200B;ドロップダウンをクリックし、Experience Cloudで目的の宛先フォルダーを選択します。

   ![](assets/send-a-list-to-adobe-experience-cloud-8.png)

1. 新しいオーディエンスを作成するか、既存のオーディエンスを上書きするかを選択します（この例では、新しいオーディエンスを作成します）。 新しいオーディエンス名を入力し、「**オーディエンスのメンバーシップを同期に保つ**」ボックスをオンにして、「**送信**」をクリックします。

   ![](assets/send-a-list-to-adobe-experience-cloud-9.png)

1. 「**OK**」をクリックします。

   ![](assets/send-a-list-to-adobe-experience-cloud-10.png)

## リストの同期を停止する方法{#how-to-stop-a-list-sync}

リストの同期はいつでも停止できます。

1. Marketoで、同期を停止するリストを探して選択します。

   ![](assets/send-a-list-to-adobe-experience-cloud-11.png)

1. **リストアクション**&#x200B;ドロップダウンをクリックし、「**リストの同期を停止**」を選択します。

   ![](assets/send-a-list-to-adobe-experience-cloud-12.png)

1. 同期を停止するオーディエンスを選択し、「**停止**」をクリックします。

   ![](assets/send-a-list-to-adobe-experience-cloud-13.png)

1. 「**停止**」をクリックして確定します。

   ![](assets/send-a-list-to-adobe-experience-cloud-14.png)

## 注意事項{#things-to-note}

**Adobe Analyticsへの共有**

Adobe Audience ManagerとAdobe Analyticsの両方を所有しているお客様は、この統合により、MarketoからAdobe Analyticsレポートスイートにオーディエンスを共有できますが、これを有効にするためにAdobe Audience Managerで実行する必要がある追加の設定手順があります。 この設定方法の詳細については、Adobe Audience Managerのドキュメントを参照してください。[https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html).

**Adobe Audience Managerのお客様の特性の使用**

Marketoでリストの書き出しを開始すると、Adobe Audience Managerインスタンスに次の変更が反映されます。

* 書き出されたリスト内のすべてのリードに対して、Marketoは、リードのハッシュ化された電子メールをクロスデバイス識別子として使用して特性を書き込みます。 特性の名前は、エクスポート時に指定したDestination Audience Nameと一致します。
* Marketoが書き出したリストのリードと照合するために管理しているすべてのECIDに対して、MarketoはECIDデバイス識別子を使用して特性を書き込みます。 特性の名前は、エクスポート時に指定したDestination Audience Nameと一致します。
* また、Marketoは、ECID特性を唯一のAudience Manager条件として使用して、セグメントインスタンスにセグメントを作成します。 セグメントの名前は、エクスポート時に指定した「宛先オーディエンス名」に一致します。

## FAQ {#faq}

**MarketoのリストサイズがAdobeのリストサイズと異なるのはなぜですか？**

内部で、オーディエンス統合は、Marketo MunchkinのCookieを対応するAdobeECID Cookieと同期することで機能します。 Marketoは、MarketoがECIDを同期したリードのメンバーシップデータのみを共有できます。 可能な限り最良の結果を得るには、Marketoのmunchkin.jsトラッキングスクリプトを、マーケティング目的でトラッキングしたいすべてのページのAdobeのvisitor.jsトラッキングコードと並行して読み込むことをお勧めします。

**Cookieの同期はどのように機能しますか。**

お使いのMarketoサブスクリプションに対してCookieAdobeが有効になっている場合、Marketoのmunchkin.jsは、統合の設定時に指定したAdobeIMS組織のCookie IDを取得して保存し、対応するMarketoのCookie IDと照合します。 これにより、Marketoの匿名ユーザープロファイルがAdobeECIDで強化されます。

匿名ユーザープロファイルをリードプロファイルに関連付けるには、さらに手順が必要です。リードプロファイルは、プレーンテキストのEメールで識別されます。 [ここでは](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md)と説明します。

**どのような情報が共有されますか。**

この統合は、MarketoからAdobeにリストメンバーシップ情報のみを共有します（例えば、リードXがリストYのメンバーであるという知識）。 この統合を介して、追加のリード属性はAdobeに共有されません。
