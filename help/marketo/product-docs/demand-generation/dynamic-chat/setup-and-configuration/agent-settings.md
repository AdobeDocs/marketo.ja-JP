---
description: Dynamic Chatでエージェントのカレンダーとミーティングまたはライブチャットの可用性を設定する方法について説明します。 OutlookまたはGmailと連携して予定を設定できます。
title: エージェント設定
feature: Dynamic Chat
exl-id: a782ef9b-6a89-448a-8bd9-f127ceea3bf5
TQID: https://experienceleague.adobe.com/ahFQ2s-DqjnDhtCLIJwOG7Z6vlH5fQVGLBS9FibW7I8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 634
ht-degree: 69%

---

# エージェント設定 {#agent-settings}

カレンダーを設定して、会議／ライブチャットの可用性を設定します。

>[!PREREQUISITES]
>
>エージェントに適切な[権限](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"}が付与されていることを確認します。

![](assets/agent-settings-1.png)

## カレンダーを接続 {#connect-calendar}

「カレンダー設定」タブで、Outlook または Gmail のカレンダーを接続して、チャットボットでの予定スケジュール設定に使用します。

![](assets/agent-settings-2.png)

ユーザのカレンダーが動的チャットに接続されると、そのユーザはキューに追加され、web サイトの訪問者が予定をスケジュールする際に使用できるようになります。

>[!NOTE]
>
>1 ユーザにつき 1 つのカレンダーを接続できます。 複数のカレンダーで会議を受け取る場合は、複数のユーザを追加し、各ユーザにカレンダーを連携させる必要があります。

また、カレンダーに予定をスケジュールするときに訪問者に送信される、招待の本文をカスタマイズすることもできます。 下部のチェックボックスを選択して、「Google Meet」リンクまたは「Microsoft Teams」リンクを含めることもできます（接続されたカレンダーに応じて異なります）。

![](assets/agent-settings-3.png)

>[!TIP]
>
>トークンアイコン（波括弧）を使用して、ユーザ属性または会社属性を使用して会議予約確認メールをパーソナライズします。

### 権限 {#permissions}

Outlook で設定すると、Dynamic Chat に対して次の権限が付与されます。

* カレンダーへの完全なアクセス
* サインインしてプロファイルを読む
* アクセス権を付与したデータへのアクセスを維持する
* メールボックスの設定を読み取る

Google で設定すると、Dynamic Chat に対して次の権限が付与されます。

* カレンダーを作成、変更または削除する
* 個々のカレンダーイベントを更新する
* イベントを表示できるユーザなど、設定を変更する
* カレンダーを共有するユーザを変更する
* 名前、メールアドレス、言語設定、プロファイル画像へのアクセス

## 会議予約の空き時間 {#meeting-booking-availability}

会議予約を受け取るためのタイムゾーンおよび時刻／曜日の空き時間を設定します。

![](assets/agent-settings-4.png)

<table>
 <tbody>
  <tr>
   <td><b>ミーティング期間</b></td>
   <td>訪問者に表示される、空いている会議時間枠の長さを決定します。</td>
  </tr>
  <tr>
   <td><b>ミーティング間のバッファ時間</b></td>
   <td>会議後のバッファーとして設定した時間。 30 分に設定すると、カレンダーで予定されている会議の終了から 30 分後まで、誰も会議を予約できません。</td>
  </tr>
 </tbody>
</table>

>[!TIP]
>
>右側の「**+**」記号をクリックして、同じ日の複数の時間ブロック（例：午前 8 時から正午&#x200B;_および_&#x200B;午後 1 時から午後 5 時）を選択できます。

## ライブチャットの可用性 {#live-chat-availability}

ライブチャットを受け取るためのタイムゾーンおよび時刻／曜日の空き時間を設定します。

![](assets/agent-settings-5.png)

アプリにログインすると、チャットの着信に関するアプリ内通知が届きます。 ログインしていない場合は、ブラウザー通知が届きます（[設定した場合](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}）。

>[!IMPORTANT]
>
>* エージェントの受信トレイ **の[可用性トグル ](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#availability-toggle){target="_blank"}は、_ライブチャットの可用性_ タブに入力された内容**&#x200B;を上書きします。 そのため、エージェントが1pから5pの間に利用可能にスケジュールされていても、3pでクイックブレークを取る必要がある場合は、エージェントの設定を変更する必要はありません。 可用性トグルステータスは、手動で変更されるまで、エージェントの可用性の次の時間ブロックに達するまで、またはエージェントの指定されたタイムゾーンの深夜まで保持されます（詳しくは次の箇条書きを参照してください）。
>
>* エージェントが可用性トグルを使用してステータスを「使用可能」に変更すると、可用性スケジュールで指定されたタイムゾーンの深夜に、ステータスが自動的にリセットされます（使用不可に切り替わります）。 タイムゾーンが指定されていない場合、デフォルトはUTC （協定世界時）になります。

>[!TIP]
>
>右側の「**+**」記号をクリックして、同じ日の複数の時間ブロック（例：午前 8 時から正午&#x200B;_および_&#x200B;午後 1 時から午後 5 時）を選択できます。

## エージェントプロファイル写真

エージェントは自分のプロファイル写真をアップロードできますが、そのアクションは Dynamic Chat では実行されません。 `account.adobe.com/profile` に移動する必要があります。 詳細情報はこちら：[アカウントプロファイルの更新](https://helpx.adobe.com/jp/manage-account/using/edit-adobe-account-personal-profile.html)。

>[!NOTE]
>
>`experience.adobe.com` に表示されるプロファイル画像はサポートされて&#x200B;**いません**。
