---
description: システムステータス通知の登録 – Marketo Engage ドキュメント – 製品ドキュメント
title: システムステータス通知のサブスクライブ
feature: Getting Started
hide: true
hidefromtoc: true
exl-id: f4404a26-3b86-4dc7-8ecb-52a24fdb09b4
source-git-commit: 700e1c62e00ce8d8f510637233de42636e5b90cb
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 2%

---

# システムステータス通知のサブスクライブ {#subscribe-to-system-status-notifications}

様々なステータス通知を登録して、現在のイシューに関する最新の情報を入手する方法を説明します。

>[!PREREQUISITES]
>
>サブスクリプションを作成する前に、まずサブスクリプションが配置されているデータセンターとポッド/サーバーを特定する必要があります。

## データセンターの特定 {#identify}

+++データセンターとポッド/サーバーの特定

1. Marketo Engageの「**管理者**」セクションで、「**マイアカウント**」をクリックします。

   ![](assets/subscribe-to-system-status-notifications-1.png)

1. 下にスクロールして、_サポート情報_&#x200B;を表示します。

   ![](assets/subscribe-to-system-status-notifications-2.png)

「_データセンター_」フィールドでは、文字がデータセンター、数字がポッドです。 上記の例では、ユーザーはポッド 49 上の Ashburn データセンターにあります。

[ サブスクリプションの作成 ](#create-a-subscription) の手順 7 では、地域の場所 **Marketo Ashburn** とポッド **ab49** を選択します。

<table style="width:300px;">
  <tr>
    <th colspan="2">データセンターの略語</th>
  </tr>
  <tr>
    <td style="width:25%;">ab</td>
    <td>アシュバーン</td>
  </tr>
  <tr>
    <td style="width:25%;">sj</td>
    <td>サンノゼ</td>
  </tr>
  <tr>
    <td style="width:25%;">sn</td>
    <td>シドニー</td>
  </tr>
  <tr>
    <td style="width:25%;">ロン</td>
    <td>ロンドン</td>
  </tr>
  <tr>
    <td style="width:25%;">nld</td>
    <td>アムステルダム</td>
  </tr>
</table>

>[!TIP]
>
>この手法は、サブスクリプションが含まれる Real Time Personalization（RTP）ポッド/サーバーを特定するためにも使用できます。

+++

## 購読を作成 {#create-a-subscription}

[ データセンターとポッド/サーバーを識別 ](#identify) した後、次の手順に従ってサブスクリプションを作成します。

1. [status.adobe.com](https://status.adobe.com/ja) で、「**購読を管理**」をクリックします。

   ![](assets/subscribe-to-system-status-notifications-3.png)

1. Adobeの資格情報を使用してログインします（まだログインしていない場合）。資格情報がない場合は、「**アカウントを作成**」をクリックします。

   ![](assets/subscribe-to-system-status-notifications-4.png)

1. 「_製品説明_」タブを開いたまま、「**サブスクリプションを作成**」をクリックします。

   ![](assets/subscribe-to-system-status-notifications-5.png)

1. ![2}Experience Cloud](assets/icon-plus-sign.png) の横にある「プラス記号アイコン _アイコンをクリックして、メニューを展開します。__Adobe Marketo Engage_ に対しても、同じ操作を行います。

   ![](assets/subscribe-to-system-status-notifications-6.png){width="800"}

1. 通知を受け取る製品/サービスを選択し、「**続行**」をクリックします。

   >[!TIP]
   >
   >「_Adobe Marketo Engage_」をオンにしてすべてを選択します。

   ![](assets/subscribe-to-system-status-notifications-7.png){width="800"}

1. 目的のイベントタイプを選択します。

   ![](assets/subscribe-to-system-status-notifications-8.png)

   <table style="width:500px;">
   <tr>
   <td style="width:35%;"><b>サービスの重大な問題</b></td>
   <td>実稼動システムで複数のユーザーが使用できない、またはパフォーマンスが大幅に低下する。</td>
   </tr>
   <tr>
   <td style="width:35%;"><b>軽微なサービス問題</b></td>
   <td>実稼動システムの複数のユーザーに対して、部分的なサービスが使用できない、またはパフォーマンスが若干低下する。</td>
   </tr>
   <tr>
   <td style="width:35%;"><b>サービス保守</b></td>
   <td>製品の可用性やパフォーマンスに影響を与える可能性のある製品メンテナンスを実行するためにスケジュールされたウィンドウ。</td>
   </tr>
   <tr>
   <td style="width:35%;"><b>お知らせ</b></td>
   <td>影響の大きいグローバル、製品ファミリまたは製品関連のメッセージ。</td>
   </tr>
   </table>

1. 地域の場所と環境を選択します。 「**続行**」をクリックします。

   ![](assets/subscribe-to-system-status-notifications-9.png){width="900"}

   >[!NOTE]
   >
   >この情報がどこにあるかを見落とした場合は、[ データセンターの特定 ](#identify) を参照してください。

1. サブスクリプションの環境設定 **メール** または **Slack** を選択し、「**続行**」をクリックします。

   ![](assets/subscribe-to-system-status-notifications-10.png)

1. 選択内容を確認し、「**環境設定を確認**」をクリックします。

   ![](assets/subscribe-to-system-status-notifications-11.png)
