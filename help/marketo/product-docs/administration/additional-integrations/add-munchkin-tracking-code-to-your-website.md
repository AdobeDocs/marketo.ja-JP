---
unique-page-id: 2360354
description: Munchkin追加追跡コードをWebサイト —Marketoドキュメント — 製品ドキュメント
title: Munchkin追加追跡コードをWebサイトに送信
exl-id: a03a7f11-8d5e-4325-b975-8fc350711da0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# 追跡コード追加をWebサイトにマンチキンする{#add-munchkin-tracking-code-to-your-website}

MarketoのカスタムのJavaScriptトラッキングコードMunchkinは、Webサイトを訪問するすべての個人を追跡するので、自動マーケティングキャンペーンを使用して訪問に反応できます。 匿名訪問者でも、そのIPアドレスやその他の情報と共に追跡されます。 **このトラッキングコードがないと、Webサイト上の訪問や他のアクティビティを追跡できません**。

>[!PREREQUISITES]
>
>経験豊富なJavaScript開発者にアクセスできることを確認してください。 Marketoテクニカルサポートは、カスタムJavaScriptのトラブルシューティングを支援するために設定されていません。

## Webサイト追加へのトラッキングコード{#add-tracking-code-to-your-website}

>[!NOTE]
>
>また、Adobe Experience Cloudのお客様は、MarketoのAdobe開始統合機能を使用して、Munchkinスクリプトをウェブページに含めることもできます。 アプリ[を取得します。](https://www.adobeexchange.com/experiencecloud.details.101054.html)

1. **管理者**&#x200B;に移動し、左のツリーで&#x200B;**マンチキン**&#x200B;をクリックします。

   ![](assets/image2015-8-25-16-3a21-3a14.png)

   「追跡コードタイプ」で「非同期」を選択します。

   ![](assets/image2015-8-25-16-3a24-3a33.png)

   >[!NOTE]
   >
   >ほとんどの場合は、非同期コードを使用する必要があります。 [詳細はこちらをご覧ください。](#types-of-munchkin-tracking-codes)

   をクリックし、JavaScriptトラッキングコードをコピーしてWebサイトに配置します。

   ![](assets/image2015-8-25-16-3a26-3a12.png)

   >[!CAUTION]
   >
   >このスクリーンショットに示すコードは使用しないでください。アカウントに表示される一意のコードを使用する必要があります。

   >[!TIP]
   >
   >追跡するWebページにトラッキングコードを設定します。 これは、小規模なサイトではすべてのページに当てはまり、多くの動的に生成されたウェブページやユーザーフォーラムなどを持つサイトでは主要ページに過ぎません。

   最良の結果を得るには、非同期Munchkinコードを使用し、ページの`<head>`要素内に配置します。 単純なコードを使用している場合（非推奨）、これは`</body>`タグの直前にあります。
   ![](assets/image2015-8-25-16-3a5-3a20.png)

>[!TIP]
>
>トラフィック量の多いサイト（1か月に何十万回もの訪問など）の場合は、匿名ユーザーを追跡しないようにすることをお勧めします。 [詳細](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/).

## 追加複数のワークスペースを使用した場合のトラッキングコード{#add-tracking-code-when-using-multiple-workspaces}

MarketoアカウントでWorkspacesを使用している場合は、ワークスペースに対応する個別のWebプレゼンスも存在する可能性があります。 この場合、マンチキン追跡JavaScriptを使用して、匿名ユーザーを正しいワークスペースとパーティションに割り当てることができます。

1. **管理者**&#x200B;に移動し、左のツリーで&#x200B;**マンチキン**&#x200B;をクリックします。

![](assets/image2015-8-25-16-3a28-3a41.png)

1. 追跡するWebページに適したワークスペースを選択します。

   ![](assets/image2015-8-25-16-3a30-3a32.png)

>[!NOTE]
>
>特別なWorkspace Munchkinコードを使用しない場合、アカウントの設定時に作成された既定のパーティションにユーザーが割り当てられます。 最初は「デフォルト」という名前ですが、自分のMarketoアカウントで変更した可能性があります。

1. 「追跡コードタイプ」で「**非同期**」を選択します。

   ![](assets/image2015-8-25-16-3a32-3a42.png)

1. をクリックし、JavaScriptトラッキングコードをコピーしてWebサイトに配置します。

   ![](assets/image2015-8-25-16-3a34-3a7.png)

   >[!CAUTION]
   >
   >このスクリーンショットに示すコードは使用しないでください。アカウントに表示される一意のコードを使用する必要があります。

1. Webページの`<head>`要素にトラッキングコードを配置します。 このページを訪問した新しいユーザーが、このパーティションに割り当てられます。

   ![](assets/image2015-8-25-16-3a5-3a20.png)

>[!CAUTION]
>
>ページ上の単一のパーティションとワークスペースに対して使用できるMunchkin追跡スクリプトは1つだけです。 Webサイト上の複数のパーティション/ワークスペースに対するトラッキングスクリプトを含めないでください。

>[!NOTE]
>
>Marketoで作成されたランディングページには自動的にトラッキングコードが含まれるので、このコードを記述する必要はありません。

## マンチキントラッキングコードのタイプ{#types-of-munchkin-tracking-codes}

マンチキントラッキングコードには3種類あり、選択できます。 Webページの読み込み時間は、それぞれ異なる影響を与えます。

1. **シンプル**:はコード行が最も少ないが、webページの読み込み時間に対しては最適化を行わない。このコードは、Webページが読み込まれるたびにjQueryライブラリを読み込みます。
1. **非同期**:webページの読み込み時間を短縮します。
1. **非同期jQuery**:webページの読み込み時間を短縮し、システムパフォーマンスも向上します。このコードは、既にjQueryがあると想定し、読み込みの確認は行いません。

## Munchkinコードが動作しているかどうかをテストする{#test-if-your-munchkin-code-is-working}

追加後にMunchkinコードが動作していることを確認するには：

1. Webページにアクセスします。

1. **Analytics**&#x200B;に移動します。

   ![](assets/mainnav-analytics-hand.png)

1. 「**Webページアクティビティ**」をクリックします。

   ![](assets/webanalytics.png)

1. 「**セットアップ**」タブをクリックし、重複が「**アクティビティソース**」をクリックして、**匿名訪問者（ISPを含む）**&#x200B;に変更します。

   ![](assets/analytics-activity-source.png)

   ![](assets/activitysource.png)

1. 「**レポート**」タブをクリックします。 データが表示されない場合は、数分待ってから、下部の更新アイコンをクリックします。
