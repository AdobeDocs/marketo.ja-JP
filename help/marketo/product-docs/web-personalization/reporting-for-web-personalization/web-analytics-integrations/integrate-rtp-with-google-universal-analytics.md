---
unique-page-id: 4720125
description: RTP を Google ユニバーサルアナリティクスに連携する — Marketo ドキュメント — 製品ドキュメント
title: RTP を Google ユニバーサルアナリティクスに連携する
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '456'
ht-degree: 100%

---

# RTP を Google ユニバーサルアナリティクスに連携する {#integrate-rtp-with-google-universal-analytics}

## はじめに {#intro}

Marketo リアルタイムパーソナライズ（RTP）の企業情報データやパーソナライズデータと Google ユニバーサルアナリティクス（GUA）を併用すると、オンラインマーケティングの取り組みについて、測定と分析の精度が向上します。

ここでは、Google ユニバーサルアナリティクス（GUA）アカウントを設定して Marketo リアルタイムパーソナライズ（RTP）プラットフォームと連携する方法について説明します。RTP データを GUA アカウントに追加すると、Web サイト訪問者のパフォーマンスを組織、業種、ファーモグラフィック、RTP セグメント別に確認することができます。

**Google ユニバーサルアナリティクス**

Google ユニバーサルアナリティクスと RTP のデータを見ると、B2B のユーザーがオンラインコンテンツをどう使っているかがよくわかり、パーソナライズキャンペーンを測定して有効に活用できます。Google ユニバーサルアナリティクスの詳細は、[こちら](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1)をご覧ください。

>[!NOTE]
>
>**Google タグマネージャーユーザーのみ**
>
>コーディングや特殊な設定は必要ありません。次のチェックリストを確認してください。
>
>* RTP のディメンションが、Google ユニバーサルアナリティクスで作成されている
>* [RTP のタグが、Google タグマネージャーで正しくインストールされている](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* Google ユニバーサルアナリティクスの連携が、RTP のアカウント設定で有効にされている
>* [Google ユニバーサルアナリティクスのタグが、Google タグマネージャーで適切に設定されている](https://support.google.com/tagmanager/answer/6107124?hl=ja)
>* [Google タグマネージャーのタグが、Web サイトに適切にインストールされている](https://developers.google.com/tag-manager/quickstart)


## GUA でカスタムディメンションを設定する {#set-up-custom-dimensions-in-gua}

1. Google Analytics で、以下の手順を実行します。

   1. 「**管理**」に移動します
   1. 「**アカウント**」を選択します
   1. 「**プロパティ**」を選択します
   1. 「**カスタム定義**」の「**カスタムディメンション**」を選択します。
      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. 新しいカスタムディメンションを追加します。「**+新規カスタムフィールド**」をクリックします

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. 追加する&#x200B;**カスタムディメンション**&#x200B;は次のとおりです。

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

1. 「**名前**」に名前を入力します。「スコープ」で「**セッション**」を選択します。「**作成**」をクリックします。

   ![](assets/image2014-11-29-11-3a12-3a51.png)

カスタムディメンションのリストは次のようになります。

![](assets/image2014-11-29-11-36-50-version-2.png)

GUA でカスタムディメンションをアクティブにしたら、RTP プラットフォームに移動して、作成したディメンションを RTP で有効にします。

## RTP アカウントで、GUA 連携を有効にする {#activate-the-gua-integration-in-your-rtp-account}

1. RTP アカウントで、「**アカウント設定**」に移動します。

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. 「**アカウント設定**」で、「**ドメイン**」をクリックします。
1. 「**Analytics**」で、「**Google ユニバーサルアナリティクス**」をクリックします。
1. 該当する「カスタムディメンション」と「イベント」を&#x200B;**オン**&#x200B;にして、このデータを RTP から Google ユニバーサルアナリティクスに追加します。
1. GUA のインデックス番号に合わせたディメンションの&#x200B;**インデックス番号**&#x200B;を入力します。
1. 「**保存**」をクリックします。

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>カスタムディメンションのインデックス番号は、GUA の「カスタムディメンション」で確認できます。
>
>例：「RTP-Industry」のインデックス番号は 1、「RTP-Organization」のインデックス番号は 2 です。

## Google Analytics で古いダッシュボードを削除する {#remove-old-dashboards-in-google-analytics}

1. Google Analytics で、以下の手順を実行します。「**レポート**」に移動します。
1. 「**マイレポート**」をクリックします。
1. **マイレポート**&#x200B;を選択します（「RTP B2B」または「RTP Performance」）。
1. 「**マイレポートを削除**」をクリックします。

![](assets/image2014-11-29-11-3a42-3a55.png)
