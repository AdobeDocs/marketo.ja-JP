---
unique-page-id: 2949160
description: Adobe Analytics との連携 - Marketo ドキュメント - 製品ドキュメント
title: Adobe Analytics との連携
exl-id: 6ea35811-6f3d-4dc8-91aa-877d613f8e93
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '1059'
ht-degree: 87%

---

# Adobe Analytics との連携 {#integrate-with-adobe-analytics}

## はじめに {#intro}

Adobe Analytics アカウント内の組織、業界、[!DNL Marketo Real-Time Personalization] （RTP）キャンペーンデータを表示して、B2B の観点から web 分析を分析します。

このドキュメントでは、[!DNL Marketo Real-Time Personalization] （RTP）とAdobe Adobe Analytics間の統合について説明します。 RTP のデータを使用すると、サイトを訪問するすべての業界セグメントおよび組織のトレンドを検出および分析し、RTP キャンペーンの効果を測定し、最適な結果を得るためのインサイトと分析を提供できます。

これを実現するには、各セグメントの新規訪問者数と再訪問者数などの指標を調べ、キャンペーンのクリック率を分析し、最もコンバージョン率の高いリードを創出した業界やカスタマイズされたセグメント、リアルタイムキャンペーンを見つけます。この機能を活用して、RTP アカウントから最大限のメリットを得ます。

## RTP Audience Analytics {#rtp-audience-analytics}

RTP と AA の連携により、web 分析インターフェイス内に新しいディメンションが作成されます。RTP は、次の機能を使用して分析ダッシュボードを自動的に強化します。

1. 組織および業界データ
1. カスタマイズされた RTP セグメント
1. 重点顧客リスト（Account-Based Marketing）

これにより、B2B データが強化され、次の最適化によって関連する訪問者に焦点を当てることができます。

1. アウトバウンドチャネル
1. コンテンツ
1. リターゲティング

## チャネルレポート {#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

RTP ダッシュボードは、垂直線および RTP セグメントに従った訪問者の分類を理解するのに役立ちます。業界や、その業界に関連する様々なマーケティングキャンペーン（有料、オーガニック、ソーシャル）に従って、訪問者のパフォーマンスを確認できます。また、ダッシュボードには、訪問者が閲覧しているサイトセクションの概要が、業種別に表示されます。

## 行動レポート {#behavioral-report}

組織、業界、RTP のセグメントデータに基づいて、Adobe Analytics で異なる行動レポートを作成できます。これらのフローレポートでは、訪問者があるページまたはイベントから次へとたどるパスを視覚化します。このレポートは、訪問者がサイトに関与し続ける理由となるコンテンツを見つけるのに役立ちます。

## RTP パフォーマンス {#rtp-performance}

Adobe Analytics の「カスタムリンク」で、RTP キャンペーンのインプレッションとコンバージョンを表示します。

このカスタムリンクレポートでは、次の命名形式でキャンペーンのインプレッション数とコンバージョン数が表示されます。

* インプレッション ISegment：[RTP セグメント名]、ICampaign：[RTP キャンペーン名]
* コンバージョン ISegment：[RTP セグメント名]、ICampaign：[RTP キャンペーン名]

![](assets/custom-links-report.png)

## Adobe Analytics での設定 {#set-up-in-adobe-analytics}

この連携では、Adobe Analytics が提供する JavaScript API が使用されます。連携では、カスタムコンバージョン変数（eVar）、カスタムイベント（event）およびトラフィック変数が使用されます。すべては、AA 管理内で有効にする必要があります。AA ではコンバージョン変数、カスタムイベント、トラフィック変数を設定する必要があります。設定しないと、RTP で有効にしても、スイート内のデータを表示できなくなります。

AA でこれらの変数を設定するには、次の手順を実行します。

1. AA アカウントで&#x200B;**[!UICONTROL 管理ツール]**&#x200B;に移動します。
1. 連携で使用する&#x200B;**[!UICONTROL レポートスイート]**&#x200B;を選択します。
1. **[!UICONTROL 設定を編集]** で **[!UICONTROL コンバージョン]** に移動し、「**[[!UICONTROL コンバージョン変数 ]](https://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)**」を選択します。\
   [コンバージョン変数](https://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar)数を選択します。以下をおすすめします。

   1. Evar 20：業界カスタムコンバージョン
   1. Evar 21：組織のカスタムコンバージョン

   >[!NOTE]
   >
   >これらの番号がすでに使用されている場合は、別の使用可能な番号を選択します。この番号を RTP アカウント設定のスロット番号に合わせます。

   1. ステータスを_[!UICONTROL Enabled_] に変更します。

      1. 名前を&#x200B;**業界**&#x200B;および&#x200B;**組織**.に変更します。（レポートスイートでは次のように表示されます）。

      1. 「有効期限」フィールドを&#x200B;**[!UICONTROL 訪問]**&#x200B;に変更します。

1. **[!UICONTROL 設定を編集]** の **[!UICONTROL コンバージョン]** に移動し、「**[[!UICONTROL 成功イベント ]](https://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)**」を選択します。

   1. 「カスタム成功イベント」イベント番号を選択します。以下をおすすめします。

      1. イベント 20：RTP キャンペーン
      1. イベント 21：RTP セグメント

      >[!NOTE]
      >
      >これらの番号がすでに使用されている場合は、別の使用可能な番号を選択します。この番号を RTP アカウント設定のスロット番号に合わせます。

      1. 2 つのイベント名を&#x200B;**RTP キャンペーン**&#x200B;および **RTP セグメント**&#x200B;に変更します。これは、レポートスイートに表示される名前です。

   1. タイプフィールドで「**カウンター（下位関係なし）**」を選択します

1. **[!UICONTROL 設定を編集]**&#x200B;で、**[トラフィック](https://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable)**&#x200B;に移動して、「**[トラフィック変数](https://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)**」を選択します。.

   1. トラフィック変数プロパティ番号を選択します。以下をおすすめします。

      1. プロパティ 20 - 名前：RTP セグメント組織
      1. プロパティ 21 - 名前：RTP セグメント業界
      1. プロパティ 25 - 名前：キャンペーン組織
      1. プロパティ 26 - 名前：RTP キャンペーン業界

      >[!NOTE]
      >
      >これらの番号がすでに使用されている場合は、別の使用可能な番号を選択します。この番号を RTP アカウント設定のスロット番号に合わせます）

      1. 4 つのプロパティ名を変更します。これは、レポートスイートに表示される名前です。

   1. [!UICONTROL  有効 ] フィールドを **[!UICONTROL 有効]** に選択します。

   1. 「[!UICONTROL  パスレポート ]」フィールドを **[!UICONTROL 有効]** に選択します。

## [!DNL Marketo Real-Time Personalization] で設定（RTP） {#set-up-in-marketo-real-time-personalization-rtp}

1. RTP プラットフォームで、「**[!UICONTROL アカウント設定]**」に移動します。

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. 「**[!UICONTROL アカウント設定]**」で、「**[!UICONTROL ドメイン]**」をクリックします。
1. **[!UICONTROL Analytics]** で、**Adobe Analytics** をクリックします。
1. コンバージョン変数、カスタム変数、トラフィック変数を&#x200B;**[!UICONTROL オン]**&#x200B;にします。
1. コンバージョン変数、イベント変数、トラフィック変数の&#x200B;**スロット番号**&#x200B;を AA で作成されたスロット番号に一致させます
1. 「**[!UICONTROL 保存]**」をクリックします。

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>推奨されるスロット設定は次のとおりです。
>
>**コンバージョン変数**
>
>* [!UICONTROL  業界カスタムコンバージョン ] - スロット 20
>* [!UICONTROL  組織のカスタムコンバージョン ] - スロット 21
>
>**カスタムイベント**
>
>* [!UICONTROL Campaign カスタムイベント ] - スロット 20
>* [!UICONTROL  セグメントカスタムイベント ] - スロット 21
>
>**トラフィック変数**
>
>* [!UICONTROL  セグメント組織トラフィック変数 ] - スロット 20
>* [!UICONTROL  セグメント業界のトラフィック変数 ] - スロット 21
>* [!UICONTROL Campaign 組織トラフィック変数 ] - スロット 22
>* [!UICONTROL Campaign 業界トラフィック変数 ] - スロット 23
>
>**これらのスロット番号が、AA で作成された変数とイベント番号と一致していることを確認してください。**

## レポート {#reports}

組織名、業界、RTP セグメントおよびリアルタイムキャンペーンデータに従って、拡張された、サイトの Adobe Analytics レポートを作成します。

AA でカスタマイズされたレポートやダッシュボードの例を次に示します。

* 業界別または定義済みのセグメント別の効果（アカウントベースの重点顧客リスト）
* KPI 効果ごとの業界分類
* 組織ごとに表示されたページ数
* 組織、業界、セグメントに応じたマーケティングチャネルの効果

**- レポート例 -**

**上位の業界レポート**

![](assets/top-industries-report.png)

**組織レポート**

![](assets/image2014-11-29-12-3a29-3a42.png)

**RTP ダッシュボードの作成**

[RTP ダッシュボード](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html)と呼ばれる&#x200B;**新しいダッシュボード**&#x200B;を作成します。このダッシュボードは、垂直線および RTP セグメントに従った訪問者の分類を理解するのに役立ちます。

1. 「**[!UICONTROL ダッシュボード ]」をクリック**、「**[!UICONTROL ダッシュボードを追加]**」をクリックします。

1. ダッシュボードに **RTP ダッシュボード**&#x200B;という名前を付けます。

1. **ダッシュボードサイズ** 3 x 2、2 x 2 を選択します。

1. [レポートレット](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3)を作成して、[コンテンツをダッシュボードに追加](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard)します。

ダッシュボードへの業種レポートレットの追加

1. **[!UICONTROL カスタムコンバージョン]**&#x200B;に移動して、「**[!UICONTROL 業界]**」をクリックします。

1. グラフを&#x200B;**円グラフ**&#x200B;に設定します。

1. **[!UICONTROL ダッシュボード]**&#x200B;をクリックして、**[!UICONTROL レポートレット]**&#x200B;を追加します。

1. レポートに&#x200B;**上位の業界**&#x200B;という名前を付けます。

1. ダッシュボードに **RTP ダッシュボード**&#x200B;を配置します。

1. **新規作成**&#x200B;します。

ダッシュボードへのセグメントレポートレットの追加

1. **[!UICONTROL サイト指標]**&#x200B;に移動します。**[!UICONTROL カスタムイベント]**／**[!UICONTROL セグメント]**&#x200B;をクリックします。

1. グラフを&#x200B;**縦棒グラフ**&#x200B;に設定します。

1. **[!UICONTROL ダッシュボード]**&#x200B;をクリックして、**[!UICONTROL レポートレット]**&#x200B;を追加します。

1. レポートに&#x200B;**上位セグメント**&#x200B;という名前を付けます。

1. ダッシュボードに **RTP ダッシュボード**&#x200B;を配置します。

1. **新規作成**&#x200B;します。

レポートレットがダッシュボードに表示されます。

## Adobe Analytics でのインプレッション数とクリック数（コンバージョン）の表示 {#view-impressions-and-clicks-conversions-in-adobe-analytics}

1. **[!UICONTROL カスタム ] リンク** をクリックします。

   ![](assets/sitecatalyst1-1.png)

1. インプレッションを検索して、セグメントを表示し、キャンペーンのインプレッション数を表すキャンペーン名を表示します。\
   ![](assets/sitecatalyst1.png)

1. コンバージョンを検索して、キャンペーンのクリック数を表すセグメント名とキャンペーン名を表示します。

   ![](assets/sitecatalyst2.png)
