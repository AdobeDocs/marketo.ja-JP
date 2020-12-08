---
unique-page-id: 4720125
description: RTPとGoogle Universal Analyticsの統合 — Marketto Docs — 製品ドキュメント
title: RTPとGoogle Universal Analyticsの統合
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---


# RTPとGoogle Universal Analyticsの統合 {#integrate-rtp-with-google-universal-analytics}

## 導入 {#intro}

Google Universal Analytics(GUA)とMarketo Real-Time Personalization(RTP)のファーストグラフィックおよびパーソナライゼーションデータを活用して、オンラインマーケティング活動をより良く測定および分析できます。

この投稿では、Marketto Real-Time Personalization(RTP)プラットフォームをGoogle Universal Analytics(GUA)アカウントと組み合わせる方法を説明します。 RTPデータをGUAアカウントに追加して、Webサイトを訪問する組織、業界、ファームグラフィック、RTPセグメントのパフォーマンスを表示し、確認できるようにすることができます。

**Google Universal Analytics**

Google Universal Analytics with RTP’s dataを使用すると、B2Bユーザーがオンラインコンテンツをどのように操作するかについてより深く理解し、パーソナライズキャンペーンからより良い結果を測定して得ることができます。 [Google Universal Analyticsについて詳しくは](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1)、

>[!NOTE]
>
>**`For Google Tag Manager Users Only`**
>
>コーディングや特別な設定を行う必要はありません。 次のチェックリストを必ず完成させてください。
>
>* `RTP dimensions are created in Google Universal Analytics`
>* [RTPタグがGoogle Tag Managerに適切にインストールされている](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* `Google Universal Analytics Integration is enabled in the RTP's Account Settings`
>* [Google Universal AnalyticsタグがGoogle Tag Managerで適切に設定されている](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [Google Tag ManagerタグがWebサイトに適切にインストールされている](https://developers.google.com/tag-manager/quickstart)

>



## GUAでのカスタムDimensionの設定 {#set-up-custom-dimensions-in-gua}

1. Google Analyticsでは、

   1. 「 **管理者」に移動**
   1. 「 **アカウント」を選択します。**
   1. 「 **プロパティ」を選択します。**
   1. 「**カスタム定義**」および「 **カスタムDimension」を選択します。**

      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. 追加新しいカスタムディメンション。 クリック **+新規カスタムDimension**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. 追加次の **カスタムDimension:**

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
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Industry</strong></p></td> 
   <td><p>セッション</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTPカテゴリ</strong></p></td> 
   <td><p>セッション</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Group</strong></p></td> 
   <td><p>セッション</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**カスタムDimension名は** 、上の表で定義したとおりに指定する必要があります(そうしないと、GUA内のカスタムRTPダッシュボードとレポートが正しく表示されません)。

1. *追加*Name。 **「Scope as **Session」を選択します。** 「 **作成」をクリックします。**

   ![](assets/image2014-11-29-11-3a12-3a51.png)

カスタムDimensionリストは、次のようになります。

![](assets/image2014-11-29-11-36-50-version-2.png)

GUAでカスタムDimensionをアクティブ化したら、RTPプラットフォームに移動し、RTP内でこれらのディメンションを有効にします。

## RTPアカウントでGUA統合をアクティブ化します。 {#activate-the-gua-integration-in-your-rtp-account}

1. RTPプラットフォームで、「 **アカウント設定」に移動します。**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. 「 **アカウント設定**」で、「 **ドメイン」をクリックします。**
1. 「**Analytics」で、「 **Google Universal Analytics**」を**クリックします。
1. 関連するカスタムDimension **とイベントをオンにし** 、RTPからのこのデータをGoogle Universal Analyticsに追加します。
1. GUAのインデックス番号に合わせた **ディメンションのインデックス番号** (Index number)を入力します。
1. 「 **保存**」をクリックします。

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>カスタムDimensionのインデックス番号は、GUAの「カスタムDimension」の下にあります。
>
>例：「RTP-Industry Index Number」は1、「RTP-Organization Index Number」は2です。

## Google Analyticsの古いダッシュボードを削除 {#remove-old-dashboards-in-google-analytics}

1. Google Analytics。 「 **レポート」に移動。**
1. 「 **ダッシュボード」をクリックします。**
1. **ダッシュボード**（RTP B2BまたはRTPパフォーマンス）を選択
1. 「 **ダッシュボードを削除**」をクリックします。

![](assets/image2014-11-29-11-3a42-3a55.png)

