---
description: エージェントの設定 — Marketo Docs — 製品ドキュメント
title: エージェント設定
feature: Dynamic Chat
source-git-commit: 9a8f6fe57b585ba0eac6a577bf99e0419d8818a1
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 27%

---

# エージェント設定 {#agent-settings}

カレンダーを設定し、会議/ライブチャットの可用性を設定します。

![](assets/agent-settings-1.png)

## カレンダーの接続 {#connect-calendar}

[ 予定表の構成 ] タブで、Outlook または Gmail の予定表を接続して、Chatbot で予定のスケジュールに使用します。

![](assets/agent-settings-2.png)

ユーザのカレンダーが動的チャットに接続されると、そのユーザはキューに追加され、web サイトの訪問者が予定をスケジュールする際に使用できるようになります。

>[!NOTE]
>
>1 ユーザにつき 1 つのカレンダーを接続できます。複数のカレンダーで会議を受け取る場合は、複数のユーザを追加し、各ユーザにカレンダーを連携させる必要があります。

また、カレンダーに予定をスケジュールするときに訪問者に送信される、招待の本文をカスタマイズすることもできます。下部のチェックボックスを選択して、「Google Meet」リンクまたは「Microsoft Teams」リンクを含めることもできます（接続されたカレンダーに応じて異なります）。

![](assets/agent-settings-3.png)

>[!TIP]
>
>トークンアイコン（波括弧）を使用して、ユーザ属性または会社属性を使用して会議予約確認メールをパーソナライズします。

### 権限 {#permissions}

Outlook での設定では、次の権限をDynamic Chatに付与します。

* カレンダーへのフルアクセス
* ログインしてプロファイルを読む
* アクセス権を付与したデータへのアクセスを維持する
* メールボックス設定を読み取る

Googleでの設定では、次の権限をDynamic Chatに付与します。

* カレンダーの作成、変更、削除
* 個々のカレンダーイベントの更新
* イベントを表示できるユーザーを含め、設定を変更します
* カレンダーの共有先の変更
* 名前、メールアドレス、言語設定、プロフィール画像へのアクセス

## 会議予約の可用性 {#meeting-booking-availability}

会議の予約を受け取るタイムゾーンと利用可能な時間/曜日を設定します。

![](assets/agent-settings-4.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>会議期間</b></td>
   <td>使用可能な会議スロットに訪問者が表示される時間の長さを指定します。</td>
  </tr> 
  <tr> 
   <td><b>会議間のバッファ時間</b></td>
   <td>会議後にバッファとして設定した時間。 30 分に設定した場合、予定されているカレンダーの会議終了の 30 分後まで、誰もあなたとの会議を予約することができません。</td>
  </tr>
 </tbody> 
</table>

>[!TIP]
>
>同じ日に複数の時間ブロックを選択できます（金曜日の 8a～12p など）。 _および_ 1p～5p) をクリックし、 **+** 右側にサインします。

## ライブチャットの利用可否 {#live-chat-availability}

ライブチャットを受け取るためのタイムゾーンと利用可能な時間/曜日を設定します。

![](assets/agent-settings-5.png)

アプリにログインしている場合は、着信チャットのアプリ内通知が届きます。 ログインしていない場合は、ブラウザーに通知が届きます ( [それを設定する](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}) をクリックします。

>[!IMPORTANT]
>
>The [可用性の切り替え](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#availability-toggle){target="_blank"} エージェントインボックス内 **上書きします** [ ライブチャットの可用性 ] タブに入力した内容。 したがって、1p～5p から利用可能にスケジュールされているが、3p ですぐに休憩する必要がある場合は、エージェント設定を変更する必要はありません。 可用性の切り替えステータスは、手動で変更するか、使用可能な状態の次のブロックに達するまで保持されます。

>[!TIP]
>
>同じ日に複数の時間ブロックを選択できます（金曜日の 8a～12p など）。 _および_ 1p～5p) をクリックし、 **+** 右側にサインします。
