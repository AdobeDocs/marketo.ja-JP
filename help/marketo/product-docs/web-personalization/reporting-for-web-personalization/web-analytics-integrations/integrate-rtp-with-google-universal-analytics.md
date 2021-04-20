---
unique-page-id: 4720125
description: RTPをGoogle Universal Analyticsと統合 —Marketoドキュメント — 製品ドキュメント
title: RTPとGoogle Universal Analyticsの統合
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 1%

---

# RTPとGoogle Universal Analytics {#integrate-rtp-with-google-universal-analytics}の統合

## 導入{#intro}

Google Universal Analytics(GUA)とMarketoリアルタイムパーソナライゼーション(RTP)のファーストグラフィックおよびパーソナライゼーションデータを活用して、オンラインマーケティング活動をより良く測定および分析できます。

この投稿では、Marketoリアルタイムパーソナライゼーション(RTP)プラットフォームをGoogle Universal Analytics(GUA)アカウントと組み合わせる方法を説明します。 RTPデータをGUAアカウントに追加して、Webサイトを訪問する組織、業界、ファームグラフィック、RTPセグメントのパフォーマンスを表示し、確認できるようにすることができます。

**Google ユニバーサルアナリティクス**

Google Universal Analytics with RTP’s dataを使用すると、B2Bユーザーがオンラインコンテンツをどのように操作するかについてより深く理解し、パーソナライズキャンペーンからより良い結果を測定して得ることができます。 [Google Universal Analyticsについて詳しくは](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1)、

>[!NOTE]
>
>**Google Tag Managerユーザーのみ**
>
>コーディングや特別な設定を行う必要はありません。 次のチェックリストを必ず完成させてください。
>
>* RTPディメンションは、Google Universal Analyticsで作成されます
>* [RTPタグがGoogle Tag Managerに適切にインストールされている](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* Google Universal Analytics Integrationは、「RTPのアカウント設定」で有効になります。
>* [Google Universal AnalyticsタグがGoogle Tag Managerで適切に設定されている](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [Google Tag ManagerタグがWebサイトに適切にインストールされている](https://developers.google.com/tag-manager/quickstart)


## GUAでのカスタムDimensionの設定{#set-up-custom-dimensions-in-gua}

1. Google Analyticsでは、

   1. **管理者**&#x200B;に移動
   1. **アカウントを選択します。**
   1. **プロパティを選択します。**
   1. 「**カスタムDimension**」と「**カスタム定義**」を選択します。
      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. 追加新しいカスタムディメンション。 「**+新しいカスタムDimension**」をクリックします

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. 追加次の&#x200B;**カスタムDimension:**

<table> 
 <tbody> 
  <tr> 
   <td><p><strong>カスタムDimension名</strong></p></td> 
   <td><p><strong>範囲</strong></p></td> 
   <td><p><strong>アクティブ</strong></p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP組織</strong></p></td> 
   <td><p>セッション</p></td> 
   <td><p align="center">kid</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Industry</strong></p></td> 
   <td><p>セッション</p></td> 
   <td><p align="center">kid</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTPカテゴリ</strong></p></td> 
   <td><p>セッション</p></td> 
   <td><p align="center">kid</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Group</strong></p></td> 
   <td><p>セッション</p></td> 
   <td><p align="center">kid</p></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**カスタムDimension** 名は、上の表で定義したとおりにする必要があります(そうしないと、GUA内のカスタムRTPダッシュボードとレポートが正しく表示されません)。

1. 追加&#x200B;**名前**。 範囲を&#x200B;**セッション**&#x200B;として選択します。 「**作成**」をクリックします。

   ![](assets/image2014-11-29-11-3a12-3a51.png)

カスタムDimensionリストは、次のようになります。

![](assets/image2014-11-29-11-36-50-version-2.png)

GUAでカスタムDimensionをアクティブ化したら、RTPプラットフォームに移動し、RTP内でこれらのディメンションを有効にします。

## RTPアカウントでGUA統合をアクティブ化{#activate-the-gua-integration-in-your-rtp-account}

1. RTPプラットフォームで、**「アカウント設定」に移動します。**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. 「**アカウント設定**」で、「**ドメイン**」をクリックします。
1. 「**解析**」で、「**Google Universal Analytics**」をクリックします。
1. **関連するカスタムDimensionとイベントを**&#x200B;オンにして、RTPからのこのデータをGoogle Universal Analyticsに追加します。
1. GUAのインデックス番号と整列したディメンションの&#x200B;**インデックス番号**&#x200B;を入力します。
1. 「**保存**」をクリックします。

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>カスタムDimensionのインデックス番号は、GUAの「カスタムDimension」の下にあります。
>
>例：「RTP-Industry Index Number」は1、「RTP-Organization Index Number」は2です。

## Google Analyticsの古いダッシュボードを削除{#remove-old-dashboards-in-google-analytics}

1. Google Analytics。 **レポート**&#x200B;に移動
1. **ダッシュボードをクリックします。**
1. **ダッシュボード**&#x200B;を選択（RTP B2BまたはRTPパフォーマンス）
1. 「**ダッシュボード**&#x200B;を削除」をクリックします。

![](assets/image2014-11-29-11-3a42-3a55.png)
