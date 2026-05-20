---
unique-page-id: 4720125
description: dnl googleとrtpを統合を使用して、Marketo Engageでrtpとgoogle universal analyticsを統合する方法を説明します。 このガイドを使用して、次のステップを完了してください。
title: RTP を Google ユニバーサルアナリティクスに連携する
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
feature: Web Personalization
TQID: https://experienceleague.adobe.com/ozCazXzX-TzsUx61u7c30v2p-Z4k1b-kQbEsw9HvgPo
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 447
ht-degree: 94%

---

# RTP を [!DNL Google Universal Analytics] に統合 {#integrate-rtp-with-google-universal-analytics}

## はじめに {#intro}

[!DNL Marketo Real-Time Personalization]（RTP）の企業情報データやパーソナライゼーションデータと [!DNL Google Universal Analytics]（GUA）を併用すると、オンラインマーケティングの取り組みについて、測定と分析の精度が向上します。

ここでは、[!DNL Google Universal Analytics]（GUA）アカウントを設定して [!DNL Marketo Real-Time Personalization]（RTP）プラットフォームと統合する方法について説明します。 RTP データを GUA アカウントに追加すると、web サイト訪問者のパフォーマンスを組織、業種、ファーモグラフィック、RTP セグメント別に確認することができます。

**[!DNL Google Universal Analytics]**

[!DNL Google Universal Analytics] と RTP のデータを見ると、B2B のユーザがオンラインコンテンツをどう使っているかがよくわかり、パーソナライゼーションキャンペーンを測定して有効に活用できます。 [詳しくは、 [!DNL Google Universal Analytics] を参照してください。](https://support.google.com/analytics/answer/2790010/?hl=en&authuser=1)。

>[!NOTE]
>
>**Google タグマネージャーユーザーのみ**
>
>コーディングや特殊な設定は必要ありません。 次のチェックリストを確認してください。
>
>* RTP ディメンションは [!DNL Google Universal Analytics] で作成されている
>* [RTP のタグが、Google タグマネージャーで正しくインストールされている](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* [!DNL Google Universal Analytics] の統合が、RTP のアカウント設定で有効にされている
>* [[!DNL Google Universal Analytics]  のタグが、Google タグマネージャーで正しく設定されている](https://support.google.com/tagmanager/answer/6107124?hl=ja)
>* [Google タグマネージャーのタグが、Web サイトに適切にインストールされている](https://developers.google.com/tag-manager/quickstart)

## GUA でカスタムディメンションを設定する {#set-up-custom-dimensions-in-gua}

1. Google Analytics で、以下の手順を実行します。

   1. 「**[!UICONTROL 管理]**」に移動します
   1. 「**[!UICONTROL アカウント]」を選択します。**
   1. 「**[!UICONTROL プロパティ]」を選択します。**
   1. 「**[!UICONTROL カスタム定義]**」の「**[!UICONTROL カスタムディメンション]**」を選択します。
      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. 新しいカスタムディメンションを追加します。 「**[!UICONTROL +新規カスタムフィールド]**」をクリックします

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. 次の&#x200B;**[!UICONTROL カスタムディメンション]を追加します。**

<table>
 <tbody>
  <tr>
   <td><p><strong>カスタムディメンション名</strong></p></td>
   <td><p><strong>範囲</strong></p></td>
   <td><p><strong>アクティブ</strong></p></td>
  </tr>
  <tr>
   <td><p><strong>RTP-Organization</strong></p></td>
   <td><p>セッション</p></td>
   <td><p align="center">✓</p></td>
  </tr>
  <tr>
   <td><p><strong>RTP-Industry</strong></p></td>
   <td><p>セッション</p></td>
   <td><p align="center">✓</p></td>
  </tr>
  <tr>
   <td><p><strong>RTP-Category</strong></p></td>
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
>**カスタムディメンション名**&#x200B;は、上の表のとおりに正確に指定してください（さもないと、GUA でカスタム RTP のダッシュボードとレポートが正しく表示されません）。

1. 「**[!UICONTROL 名前]**」に名前を入力します。 「スコープ」で「**[!UICONTROL セッション]**」を選択します。 「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/image2014-11-29-11-3a12-3a51.png)

カスタムディメンションのリストは次のようになります。

![](assets/image2014-11-29-11-36-50-version-2.png)

GUA でカスタムディメンションをアクティブにしたら、RTP プラットフォームに移動して、作成したディメンションを RTP で有効にします。

## RTP アカウントで、GUA 連携を有効にする {#activate-the-gua-integration-in-your-rtp-account}

1. RTP プラットフォームで、「**[!UICONTROL アカウント設定]」に移動します。**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. 「**[!UICONTROL アカウント設定]**」で、「**[!UICONTROL ドメイン]**」をクリックします。
1. 「**[!UICONTROL Analytics]**」で、「**[!UICONTROL Google ユニバーサルアナリティクス]**」をクリックします。
1. 該当する「カスタムディメンション」と「イベント」を&#x200B;**[!UICONTROL オン]**&#x200B;にして、このデータを RTP から [!DNL Google Universal Analytics] に追加します。
1. GUA のインデックス番号に合わせたディメンションの&#x200B;**[!UICONTROL インデックス番号]**&#x200B;を入力します。
1. 「**[!UICONTROL 保存]**」をクリックします。

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>カスタムディメンションのインデックス番号は、GUA の「カスタムディメンション」で確認できます。
>
>例：「RTP-Industry」のインデックス番号は 1、「RTP-Organization」のインデックス番号は 2 です。

## Google Analytics で古いダッシュボードを削除する {#remove-old-dashboards-in-google-analytics}

1. Google Analytics で、以下の手順を実行します。 「**[!UICONTROL レポート]」に移動します。**
1. 「**[!UICONTROL ダッシュボード]」をクリックします。**
1. **[!UICONTROL ダッシュボード]**&#x200B;を選択します（「RTP B2B」または「RTP Performance」）。
1. 「**[!UICONTROL ダッシュボードを削除]**」をクリックします。

![](assets/image2014-11-29-11-3a42-3a55.png)
